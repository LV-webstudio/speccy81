# Incidente de segurança (chave, dado ou canal expostos)

Abre-se assim que se suspeita, sem esperar por ter certeza. Sem segredos nem dados pessoais neste documento:
das chaves, só o nome interno e a impressão digital; das pessoas, só o papel.

## Passos
1. **Conter** o urgente: desativar a chave, cortar o acesso ou o canal. Se for uma chave, com a regra da
   chave exposta: a substituta primeiro; se for pública e urgente, desativa-se já, dizendo antes o que deixa de
   funcionar e para quem. Nunca se reativa.
2. **Diagnosticar só a ler:** o que ficou exposto, desde quando, onde e quem o pôde ver. Mede-se (regra 2):
   número, consulta ou comando, data.
3. **Decidir e avisar:** decide o utilizador. Se houver dados pessoais de um cliente, o cliente é o **responsável**
   e tu o **subcontratante**: avisas-o por escrito **sem demora injustificada** (art. 33.º, n.º 2, RGPD) com o que aconteceu, desde
   quando, o que foi feito e o que não se pode excluir. O responsável avalia se notifica a autoridade de
   proteção de dados em **72 horas** (art. 33.º). Se os dados forem teus, o responsável és tu.
4. **Registar** todo o incidente, mesmo que não se notifique (art. 33.º, n.º 5): factos, efeitos e medidas.
5. **Lição:** a regra nova ou a melhoria do método que evita que se repita.

## Ficha
```markdown
# Incidente <n> · aberto <data hora> · estado: aberto | contido | fechado
O quê: <o que ficou exposto, por nome interno e impressão digital; nunca o valor>
Onde e desde quando: <canal, ficheiro ou serviço · primeira data possível>
Quem o pôde ver: <público | clientes | pessoal | ninguém fora da equipa> — Prova: <registo ou comando>
Contenção: <o que se desativou ou cortou, quando> — Prova: <…>
O que deixa de funcionar e para quem: <…>
Dados pessoais afetados: sim | não | não se pode excluir — porquê
Responsável pelos dados: <cliente | nós> · aviso enviado?: <data, por quem> | rascunho em <caminho>
Notificação à autoridade (decide-a o responsável): sim | não — motivo
Medidas: <…>
Lição: <regra nova ou melhoria>
```

## Exemplo
Um token de uma API aparece num ficheiro de configuração que foi publicado num repositório. Conter: gera-se
um token novo, põe-se em todos os sítios que o usam e revoga-se o velho. Diagnosticar: o registo do
fornecedor diz se alguém usou o token e desde quando. Registar: ficha preenchida mesmo que não haja dados pessoais.
Lição: o ficheiro de configuração vai no `.gitignore` e o repositório revê-se antes de publicar.
