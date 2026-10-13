# Testes de campo · <projeto> · <data>

## 1. Montagem (verificar ANTES de começar)
| O quê | Valor | Verificado? |
|---|---|---|
| Máquinas e dispositivos (modelo, SO, versão da aplicação) | | |
| Como se arranca cada peça (**a partir de um terminal limpo**, não a partir de outra sessão ou processo que herde variáveis) | | |
| Modo de permissões / configuração de cada sessão (p. ex. sem modo automático se estiverem a ser testadas aprovações) | | |
| Configurações que o teste precisa de ter ligadas (p. ex. notificações push, Remote Control, depuração USB) | | |
| Dados de teste (reais ou de semente; nunca dados pessoais em capturas de ecrã que fiquem guardadas) | | |
| Quem executa e quem observa (utilizador / sessão / outra máquina) | | |
| Como se observa (capturas de ecrã, ADB, registos, `dumpsys`, consola) | | |
| **Porta «compila»:** verificação de tipos e build de produção a verde sobre o commit que se testa (o servidor de desenvolvimento não o garante) | | |

## 2. Testes
| # | Teste | O que confirma | Passos | Resultado esperado | Prioridade |
|---|---|---|---|---|---|
| P1 | | | | | Alta |

## 3. Resultados
| # | Resultado (✅ / ❌ / ⚠ não válido) | Hora | Evidência (captura, saída) | Detalhe |
|---|---|---|---|---|
| P1 | | | | |

«⚠ não válido» = a montagem não cumpriu a tabela 1; repete-se e não conta como falha do produto.

**Um teste que falha não se salta:** repete-se (p. ex. 3 vezes) para saber se é instável ou real, vê-se a captura e apura-se se falha o teste ou a aplicação. Se no fim se salta, consta como «saltado» e com o motivo.

## 4. Conclusões e alterações
| Conclusão | Afeta (regra / documento / código) | Alteração feita ao mesmo tempo |
|---|---|---|
| | | |

## 5. Pendente de repetir
-
