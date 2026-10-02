# Incident de seguretat (clau, dada o canal exposats)

S'obre tan bon punt se sospita, sense esperar a estar-ne segur. Sense secrets ni dades personals en aquest document:
de les claus, només el seu nom intern i la seva empremta; de les persones, només el seu paper.

## Passos
1. **Contenir** l'urgent: desactivar la clau, tallar l'accés o el canal. Si és una clau, amb la regla de la
   clau exposada: la substituta primer; si és pública i urgent, es desactiva ja dient abans què deixa de
   funcionar i per a qui. Mai no es reactiva.
2. **Diagnosticar només llegint:** què va quedar exposat, des de quan, on i qui ho va poder veure. Es mesura (regla 2):
   xifra, consulta o ordre, data.
3. **Decidir i avisar:** decideix l'usuari. Si hi ha dades personals d'un client, el client és el **responsable**
   i tu l'**encarregat**: l'avises per escrit **sense dilació indeguda** (art. 33.2 RGPD) amb què va passar, des de
   quan, què s'ha fet i què no es pot descartar. El responsable valora si notifica a l'autoritat de
   protecció de dades en **72 hores** (art. 33). Si les dades són teves, el responsable ets tu.
4. **Registrar** tot incident, encara que no es notifiqui (art. 33.5): fets, efectes i mesures.
5. **Lliçó:** la regla nova o la millora del mètode que evita que es repeteixi.

## Fitxa
```markdown
# Incident <n> · obert <data hora> · estat: obert | contingut | tancat
Què: <què va quedar exposat, per nom intern i empremta; mai el valor>
On i des de quan: <canal, fitxer o servei · primera data possible>
Qui ho va poder veure: <públic | clients | personal | ningú fora de l'equip> — Prova: <registre o ordre>
Contenció: <què es va desactivar o tallar, quan> — Prova: <…>
Què deixa de funcionar i per a qui: <…>
Dades personals afectades: sí | no | no es pot descartar — per què
Responsable de les dades: <client | nosaltres> · avís enviat?: <data, per qui> | esborrany a <ruta>
Notificació a l'autoritat (la decideix el responsable): sí | no — motiu
Mesures: <…>
Lliçó: <regla nova o millora>
```

## Exemple
Un token d'una API apareix en un fitxer de configuració que es va publicar en un repositori. Contenir: es genera
un token nou, es posa a tots els llocs que l'usen i es revoca el vell. Diagnosticar: el registre del
proveïdor diu si algú va usar el token i des de quan. Registrar: fitxa omplerta encara que no hi hagi dades personals.
Lliçó: el fitxer de configuració va a `.gitignore` i el repositori es revisa abans de publicar.
