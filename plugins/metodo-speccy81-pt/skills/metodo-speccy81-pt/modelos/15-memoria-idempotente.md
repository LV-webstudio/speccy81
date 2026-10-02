# Memória idempotente (regra 11)

## Princípios
- **Um tema por ficheiro** e um **índice curto** (`MEMORY.md`: uma linha por ficheiro).
- **Ficheiros de estado** (o que muda): **reescritos por inteiro** com «Estado a <data e hora>», nunca com texto
  acrescentado no fim. **Ficheiros de decisão** (o que é estável): não se tocam, a não ser que a decisão mude.
- **Um `retomar.md`** como porta de entrada. É reescrito no fecho de cada fase ou bloco, e sempre antes de
  reiniciar uma sessão longa (em vez de compactar).
- Ligações entre ficheiros com `[[nome]]`. Nada do que o repositório já guarda (código, histórico do git).
- **Sem segredos nem dados de terceiros.** Os dados do próprio utilizador, só na memória local.
- **Compactar só ao fechar um bloco**, com a memória já guardada; se chegar sozinha, retoma-se a partir de `retomar.md`.

## Modelo de `retomar.md`
```markdown
---
name: retomar
description: COMECE AQUI ao abrir uma nova sessão sobre <projeto>: onde ficaram as coisas, fios em aberto e o que verificar primeiro
metadata:
  type: project
---

**Estado a <data hora>.** Ficheiro idempotente: reescrito por inteiro no fecho de cada bloco.

## O que verificar primeiro (5 minutos)
1. <último commit / árvore limpa>
2. <caixa de correio ou estado das outras máquinas>
3. <sessões ativas e os seus nomes>

## Fios em aberto (por ordem)
| # | Fio | Próximo passo | Onde |
|---|---|---|---|

## Regras de trabalho que não mudam
- <as regras invioláveis do projeto>
```

## Modelo de ficheiro de estado
```markdown
---
name: <tema>
description: <uma linha para decidir se é relevante>
metadata:
  type: project
---

**Estado a <data hora>.** Reescrito por inteiro.

- <facto> · <onde> · <pendente> · <decisão que aguarda o utilizador>

Ver [[retomar]].
```

## Índice (`MEMORY.md`)
```markdown
- [RETOMAR · comece aqui](retomar.md) — onde ficou o trabalho e o que verificar
- [<Tema>](<tema>.md) — <gancho de uma linha>

Ficheiros de estado (…): são REESCRITOS por inteiro no fecho de cada bloco. Os restantes são decisões estáveis.
```
