# Incident de sécurité (clé, donnée ou canal exposés)

On l'ouvre dès qu'on le soupçonne, sans attendre d'en être sûr. Sans secrets ni données personnelles dans ce document :
des clés, seulement leur nom interne et leur empreinte ; des personnes, seulement leur rôle.

## Étapes
1. **Contenir** l'urgent : désactiver la clé, couper l'accès ou le canal. S'il s'agit d'une clé, avec la règle de la
   clé exposée : la clé de remplacement d'abord ; si elle est publique et urgente, on la désactive tout de suite en disant d'abord ce qui cesse de
   fonctionner et pour qui. On ne la réactive jamais.
2. **Diagnostiquer en lisant seulement :** ce qui a été exposé, depuis quand, où et qui a pu le voir. On mesure (règle 2) :
   chiffre, requête ou commande, date.
3. **Décider et prévenir :** c'est l'utilisateur qui décide. S'il y a des données personnelles d'un client, le client est le **responsable**
   et vous le **sous-traitant** : vous le prévenez par écrit **dans les meilleurs délais** (art. 33.2 RGPD) en indiquant ce qui s'est passé, depuis
   quand, ce qui a été fait et ce qui ne peut pas être écarté. Le responsable évalue s'il notifie l'autorité de contrôle
   dans les **72 heures** (art. 33). Si les données sont les vôtres, le responsable, c'est vous.
4. **Consigner** tout incident, même s'il n'est pas notifié (art. 33.5) : faits, effets et mesures.
5. **Leçon :** la nouvelle règle ou l'amélioration de la méthode qui évite que cela se répète.

## Fiche
```markdown
# Incident <n> · ouvert <date heure> · état : ouvert | contenu | clos
Quoi : <ce qui a été exposé, par nom interne et empreinte ; jamais la valeur>
Où et depuis quand : <canal, fichier ou service · première date possible>
Qui a pu le voir : <public | clients | personnel | personne hors de l'équipe> — Preuve : <journal ou commande>
Confinement : <ce qui a été désactivé ou coupé, quand> — Preuve : <…>
Ce qui cesse de fonctionner et pour qui : <…>
Données personnelles concernées : oui | non | ne peut pas être écarté — pourquoi
Responsable des données : <client | nous> · avis envoyé ? : <date, par qui> | brouillon dans <chemin>
Notification à l'autorité (décidée par le responsable) : oui | non — motif
Mesures : <…>
Leçon : <nouvelle règle ou amélioration>
```

## Exemple
Un jeton d'API apparaît dans un fichier de configuration qui a été publié dans un dépôt. Contenir : on génère
un nouveau jeton, on le met partout où il est utilisé et on révoque l'ancien. Diagnostiquer : le journal du
fournisseur dit si quelqu'un a utilisé le jeton et depuis quand. Consigner : fiche remplie même s'il n'y a pas de données personnelles.
Leçon : le fichier de configuration va dans `.gitignore` et le dépôt est examiné avant de publier.
