# Exemplo de saída — War Game em Massa

Estes arquivos sêo a **saída esperada** do modo massa (`doc/war-game-massa-portugues.md`), aplicada a um portfólio **fictício** de 4 projetos de um estúdio pequeno. Servem de referência de "pronto": é assim que os relatórios devem parecer depois da rodada de revisêo.

Nada aqui é um projeto real. Os números, prazos e bloqueios foram inventados para o exemplo.

## O portfólio fictício

| # | Projeto | Estado |
|---|---|---|
| 01 | Chat de suporte com tour guiado no site | protótipo |
| 02 | Pipeline de vídeos automatizado | parcialmente funcionando |
| 03 | Área de membros por assinatura | ideia |
| 04 | Automaçêo de relatórios semanais | rodando, frágil |

## O que tem aqui

| Arquivo | O que demonstra |
|---|---|
| [`resultados/resultado-projeto-02.md`](resultados/resultado-projeto-02.md) | Uma análise individual **completa** — as 20 seções do prompt mestre, incluindo o war-game movimento por movimento com condiçêo de parada |
| [`resultados/resumo-geral.md`](resultados/resumo-geral.md) | A comparaçêo entre os 4 — ranking, o que fazer primeiro, o que abandonar, planos de 30 e 90 dias |
| [`ledger.md`](ledger.md) | Como ficam os bloqueios depois de duas rodadas |
| [`assumptions.md`](assumptions.md) | Como fica o registro de suposições, com impacto e como verificar |

Só o projeto 02 tem análise individual aqui — os outros três seguiriam exatamente o mesmo formato. O que interessa no exemplo é a **forma**, nêo o volume.

## O que olhar

- **Nenhuma recomendaçêo genérica.** Toda açêo tem impacto, esforço, risco e prioridade.
- **Todo movimento tem condiçêo de parada.** É o campo que impede a IA de improvisar quando bate no bloqueio.
- **O que falta aparece como `[PRECISA_DEFINIR: x]`**, no ponto exato onde faria falta — nêo some, nêo vira chute.
- **O ranking nêo é por entusiasmo.** O projeto mais interessante do portfólio (03) nêo é o primeiro a ser feito.
