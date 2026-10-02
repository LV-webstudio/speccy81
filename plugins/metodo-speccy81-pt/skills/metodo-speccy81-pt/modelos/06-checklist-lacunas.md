# Análise de lacunas · «o que falta para fazer isto com qualidade?»

Pergunta orientadora: *o que determina a qualidade do resultado final que o cliente vê, e está coberto
com dados concretos que um motor possa aplicar?*

Para cada tema: pesquisar em `conhecimento/` (grep dos termos-chave) e marcar.

| Tema | Termos a pesquisar | Docs que o cobrem | Suficiente para calcular? | Ação |
|---|---|---|---|---|
| Como se executa o trabalho passo a passo (técnica) | | | | |
| Parâmetros numéricos (velocidades, tempos, tamanhos, margens) | | | | |
| O que se pode e não se pode controlar nas ferramentas/equipamento | | | | |
| Simulação ou validação antes de o fazer a sério | | | | |
| Condições externas (meteorologia, luz, hora do dia, estação) | | | | |
| Segurança, emergências e incidentes | | | | |
| Casos-limite (ambientes difíceis, falhas) | | | | |
| Pós-processamento e entrega (formatos, controlo de qualidade) | | | | |
| Automatização do pós-processamento | | | | |
| Exemplos reais (ficheiros, amostras) | | | | |
| Formação da equipa | | | | |
| Riscos laborais e legais específicos | | | | |
| **Testes com dados reais ou uso real** (há uma bancada mínima? já foi experimentado?) | | | | |
| **Privacidade e dados mínimos** (o que se lê, guarda e envia; RGPD) | | | | |
| **Implantação e sistemas existentes** (onde vive, a que se liga, o que acontece se mudar de sítio) | | | | |

Só as lacunas reais geram um novo bloco de investigação. Repetir até não restarem lacunas
importantes. O que depender de condições (meteorologia, luz, dados do cliente) deve
acabar num **seletor** com regras, não em texto solto.
