# Anàlisi de buits · «què falta per fer-ho amb qualitat?»

Pregunta guia: *què determina la qualitat del resultat final que veu el client, i està cobert
amb dades concretes que un motor pugui aplicar?*

Per a cada tema: cerca a `coneixement/` (grep de termes clau) i marca.

| Tema | Termes a cercar | Documents que ho cobreixen | N'hi ha prou per calcular? | Acció |
|---|---|---|---|---|
| Com es porta a terme el treball pas a pas (tècnica) | | | | |
| Paràmetres numèrics (velocitats, temps, mides, marges) | | | | |
| Què es pot i què no es pot controlar a les eines/equips | | | | |
| Simulació o validació abans de fer-ho de debò | | | | |
| Condicions externes (meteorologia, llum, hora del dia, estació) | | | | |
| Seguretat, emergències i incidents | | | | |
| Casos límit (entorns difícils, fallades) | | | | |
| Postprocessat i lliurament (formats, control de qualitat) | | | | |
| Automatització del postprocessat | | | | |
| Exemples reals (fitxers, mostres) | | | | |
| Formació de l'equip | | | | |
| Riscos laborals i legals específics | | | | |
| **Proves amb dades reals o ús real** (hi ha un banc mínim? ja s'ha provat?) | | | | |
| **Privacitat i dades mínimes** (què es llegeix, s'emmagatzema i s'envia; RGPD) | | | | |
| **Desplegament i sistemes existents** (on viu, a què es connecta, què passa si es mou) | | | | |

Només els buits reals generen un nou bloc de recerca. Repeteix fins que no quedin
buits importants. Tot allò que depengui de condicions (meteorologia, llum, dades del client) ha
d'acabar en un **selector** amb regles, no en text solt.
