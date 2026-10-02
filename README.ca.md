# Mètode Speccy81

![Speccy81 Method](assets/banner.jpg)

**De la idea al llançament.** Un mètode de LV-Webstudio (Speccy81) per plantejar qualsevol projecte — producte, servei, mòdul o app — amb el mateix rigor: investigar primer, decidir amb dades, convertir el que s'aprèn en coneixement verificat, auditar-lo, dissenyar abans de programar, provar al camp i publicar sense sorpreses. Té dues edicions construïdes des del mateix mètode, cadascuna com a marketplace de plugins de Claude Code.

Aquesta és l'**edició bàsica**: lliure i pública, amb una skill, una guia curta i 8 plantilles en cada idioma.

**Languages · Idiomas:** [English](README.md) · [Español](README.es.md) · [Català](README.ca.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Português](README.pt.md) · [Français](README.fr.md) · [Italiano](README.it.md) · [Deutsch](README.de.md)

## Edicions

| | Bàsica | Completa |
|---|---|---|
| Llicència | Pública: CC BY 4.0 (guia, SKILL i plantilles) + MIT (scripts); vegeu `NOTICE` | Propietària, de LV-Webstudio |
| Recorregut | Un recorregut lleuger de cinc passos per a ampliacions i projectes petits | Fases 0–9 més la 8 bis |
| Plantilles | 8 (01, 06, 09, 10, 13, 15, 20 i 21) | 21 |
| Regles d'or | Les 13, en curt | Les 13 senceres, més les millores d'eficiència E1–E15 |
| Recerca i auditoria | — | Onades de recerca en paral·lel i una auditoria única |
| Validador de coneixement | — | Sí |
| Desplegament i llançament | — | Desplegament i QA en un altre dispositiu, i publicació |
| Govern i seguretat | Regla 13 en curt, «Prova:» en tot resultat, incidents (20) i rendició de comptes (21) | A més: govern de diverses màquines (19), traslladar un secret i rotar una clau exposada |
| Diverses màquines | Una sola sessió o màquina; per a diverses sessions amb regles mínimes, Wassup Bàsica | Govern complet i coordinació opcional amb Wassup |

## Els cinc passos

| Pas | Què es fa | Plantilla |
|---|---|---|
| 1 · Fase 0 | Fitxa de context; si el projecte ja està començat, s'hi recull el que existeix (codi, documents, decisions) | 01 |
| 2 | Checklist de buits i fets canònics, abans d'investigar o dissenyar | 06, 10 |
| 3 · Fase 7 | Disseny curt, aprovat per l'usuari abans de programar | 09 |
| 4 · Fase 8 | Construcció amb proves reals i de camp | 13 |
| 5 | Memòria idempotent en tancar cada pas | 15 |
| Sempre | Rendició de comptes amb «Prova:» en tancar cada encàrrec; incident si s'exposa una clau o una dada | 21, 20 |

La numeració de les fases (0, 7 i 8) és la del mètode complet, perquè el projecte pugui créixer sense renumerar res. L'edició completa hi afegeix la resta: les fases 1 a 6, la 8 bis i la 9.

## Què hi ha a dins

Un plugin per idioma, cadascun amb la skill, la guia i les 8 plantilles: `speccy81-method` (English), `metodo-speccy81` (Español), `metode-speccy81-ca` (Català), `metodo-speccy81-pt` (Português), `methode-speccy81-fr` (Français), `metodo-speccy81-it` (Italiano), `speccy81-methode-de` (Deutsch), `speccy81-methode-nl` (Nederlands) i `metoda-speccy81-pl` (Polski).

Tots els plugins porten el mateix mètode; instal·la el de l'idioma que prefereixis.

## Instal·lació

```
claude plugin marketplace add LV-webstudio/speccy81
claude plugin install speccy81-method@speccy81      # English
claude plugin install metodo-speccy81@speccy81      # Español
claude plugin install metode-speccy81-ca@speccy81   # Català
claude plugin install metodo-speccy81-pt@speccy81   # Português
claude plugin install methode-speccy81-fr@speccy81  # Français
claude plugin install metodo-speccy81-it@speccy81   # Italiano
claude plugin install speccy81-methode-de@speccy81  # Deutsch
claude plugin install speccy81-methode-nl@speccy81  # Nederlands
claude plugin install metoda-speccy81-pl@speccy81   # Polski
```

Després demana a Claude Code que «apliqui el mètode Speccy81», també per a un projecte ja començat. La skill carrega la guia i les plantilles sota demanda.

[Wassup](https://github.com/LV-webstudio/wassup) és un complement opcional quan diverses màquines o sessions treballen en el mateix projecte.

## Com aconseguir l'edició completa

L'edició completa té llicència de LV-Webstudio. Demana accés a través de [lv-webstudio.com](https://lv-webstudio.com/).

## Llicència

L'edició bàsica s'ofereix amb dues llicències: **CC BY 4.0** per a la guia, SKILL.md i les plantilles (ús lliure, també comercial, citant l'autoria) i **MIT** per als scripts i el codi. Atribució suggerida: «Método Speccy81 · LV-Webstudio · lv-webstudio.com». L'edició completa no està coberta per aquestes llicències. Consulta [LICENSE](LICENSE).
