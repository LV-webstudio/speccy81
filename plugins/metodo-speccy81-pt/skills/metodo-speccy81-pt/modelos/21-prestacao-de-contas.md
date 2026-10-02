# Prestação de contas (regra 2)

Fecha **cada** encargo, mesmo que seja curto. Vai ao utilizador ou ao coordenador (e, com o Wassup, ao direto e à
caixa de correio). Se faltar algum ponto, o encargo fica «sem prestar contas».

## Formato
```markdown
## Prestação de contas · <encargo> · <data e hora>
Ordem (literal): «<texto exato da ordem, com quem a deu e em que janela>»
Feito:
- <o que se fez, uma linha por coisa>
Prova: <commit, impressão digital SHA-256, caminho, linha de registo ou saída de um comando>
Prova: <uma por cada coisa feita; vale com marcador: «- Prova: …»>
Não feito: <o que não se fez> — <porquê (bloqueio de permissões, falta um dado, fora do âmbito)>
Por verificar: <o que se afirma sem o ter verificado> | nada
```

## Regras
- A linha começa por `Prova:` (ou `- Prova:`). Etiqueta por idioma: es Prueba · en Proof · ca, pt e it Prova ·
  fr Preuve (com espaço antes de «:») · de Nachweis · nl Bewijs · pl Dowód.
- As palavras **feito, verificado, carregado, implantado, apagado, instalado, publicado e aplicado** sem uma
  `Prova:` no mesmo ponto são um aviso.
- Uma prova é algo que outro pode voltar a ver: «vi-o» não é prova; «guardou-o a app» também não, se não
  se releu no destino.
- O que não se pôde provar diz-se em «Por verificar», com quem o deve fazer (p. ex. «iPhone real: pendente de
  dispositivo»).
- Se depois aparecer um erro em algo prestado, **errata** com o mesmo cabeçalho e «Corrige a: <data>».

## Exemplo
```markdown
## Prestação de contas · índice do guia · 01-03-2026 10:40
Ordem (literal): «Corrige as ligações quebradas do índice» (utilizador, na janela de construção)
Feito:
- 3 ligações corrigidas em GUIA.md
Prova: commit 4f2a9c1
Prova: `validar-conhecimento.sh` → «0 ligações quebradas»
Não feito: o índice do README inglês — não é desta sessão (dono: revisão)
Por verificar: nada
```
