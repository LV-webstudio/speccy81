# Método Speccy81

![Speccy81 Method](assets/banner.jpg)

**Da ideia ao lançamento.** Um método da LV-Webstudio (Speccy81) para montar qualquer projeto — produto, serviço, módulo ou aplicação — com o mesmo rigor: investigar primeiro, decidir com dados, transformar o que se aprende em conhecimento verificado, auditá-lo, desenhar antes de programar, testar no terreno e publicar sem surpresas. Tem duas edições construídas a partir do mesmo método, cada uma como marketplace de plugins do Claude Code.

Esta é a **edição básica**: livre e pública, com uma skill, um guia curto e 8 modelos em cada idioma.

**Languages · Idiomas:** [English](README.md) · [Español](README.es.md) · [Català](README.ca.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Português](README.pt.md) · [Français](README.fr.md) · [Italiano](README.it.md) · [Deutsch](README.de.md)

## Edições

| | Básica | Completa |
|---|---|---|
| Licença | Pública: CC BY 4.0 (guia, SKILL e modelos) + MIT (scripts); ver `NOTICE` | Proprietária, da LV-Webstudio |
| Percurso | Um percurso leve de cinco passos para extensões e projetos pequenos | Fases 0–9 mais a 8 bis |
| Modelos | 8 (01, 06, 09, 10, 13, 15, 20 e 21) | 21 |
| Regras de ouro | As 13, em versão curta | As 13 completas, mais as melhorias de eficiência E1–E15 |
| Investigação e auditoria | — | Vagas de investigação em paralelo e uma auditoria única |
| Validador de conhecimento | — | Sim |
| Implementação e lançamento | — | Implementação e QA noutro dispositivo, e publicação |
| Governo e segurança | Regra 13 em curto, «Prova:» em todo o resultado, incidentes (20) e prestação de contas (21) | Além disso: governo de várias equipas (19), transferir um segredo e rodar uma chave exposta |
| Várias máquinas | Uma só sessão ou máquina; para várias sessões com regras mínimas, Wassup Básica | Governo completo e coordenação opcional com o Wassup |

## Os cinco passos

| Passo | O que se faz | Modelo |
|---|---|---|
| 1 · Fase 0 | Ficha de contexto; se o projeto já está em curso, regista-se o que existe (código, documentos, decisões) | 01 |
| 2 | Checklist de lacunas e factos canónicos, antes de investigar ou desenhar | 06, 10 |
| 3 · Fase 7 | Desenho curto, aprovado pelo utilizador antes de programar | 09 |
| 4 · Fase 8 | Construção com testes reais e de terreno | 13 |
| 5 | Memória idempotente ao fechar cada passo | 15 |
| Sempre | Prestação de contas com «Prova:» ao fechar cada encargo; incidente se se expõe uma chave ou um dado | 21, 20 |

A numeração das fases (0, 7 e 8) é a do método completo, para que o projeto possa crescer sem renumerar nada. A edição completa acrescenta o resto: as fases 1 a 6, a 8 bis e a 9.

## O que contém

Um plugin por idioma, cada um com a skill, o guia e os 8 modelos: `speccy81-method` (English), `metodo-speccy81` (Español), `metode-speccy81-ca` (Català), `metodo-speccy81-pt` (Português), `methode-speccy81-fr` (Français), `metodo-speccy81-it` (Italiano), `speccy81-methode-de` (Deutsch), `speccy81-methode-nl` (Nederlands) e `metoda-speccy81-pl` (Polski).

Todos os plugins trazem o mesmo método; instala o do idioma que preferires.

## Instalação

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

Depois pede ao Claude Code para «aplicar o método Speccy81», também para um projeto já em curso. A skill carrega o guia e os modelos quando são precisos.

O [Wassup](https://github.com/LV-webstudio/wassup) é um complemento opcional quando várias máquinas ou sessões trabalham no mesmo projeto.

## Como obter a edição completa

A edição completa tem licença da LV-Webstudio. Pede acesso através de [lv-webstudio.com](https://lv-webstudio.com/).

## Licença

A edição básica é oferecida com duas licenças: **CC BY 4.0** para o guia, o SKILL.md e os modelos (uso livre, também comercial, com atribuição de autoria) e **MIT** para scripts e código. Atribuição sugerida: «Método Speccy81 · LV-Webstudio · lv-webstudio.com». A edição completa não está coberta por estas licenças. Consulta [LICENSE](LICENSE).
