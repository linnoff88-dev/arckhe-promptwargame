ï»¿# War Game Prompt

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Prompt reutilizêÂ¡vel que transforma o planejamento de qualquer build de IA num **war game**: em vez de assumir o caminho feliz de A a B, forêÂ§a a IA a quebrar o projeto em fases, cada uma com objetivo, suposiêÂ§êÂ£o otimista, suposiêÂ§êÂ£o pessimista, modos de falha provêÂ¡veis com correêÂ§êÂ£o, critêÂ©rios de saêÂ­da verificêÂ¡veis, caminho alternativo, condiêÂ§êÂ£o de parada e orêÂ§amento de tentativa ê¢â¬â alêÂ©m de uma tabela mestre de riscos (infra, API do modelo, frontend, qualidade de conversa, seguranêÂ§a, loop de aprendizado) e um loop semanal de autoavaliaêÂ§êÂ£o.

ê°Å¸ââ **Guia completo (landing + passo a passo):** https://linnoff88-dev.github.io/arckhe-/guia/

## Dois modos

| | **War Game** | **War Game em Massa** |
|---|---|---|
| Para | Um projeto, a fundo | VêÂ¡rios projetos, comparados |
| Responde | Como construir isso sem levar porrada no caminho? | Tenho N projetos parados ê¢â¬â qual faêÂ§o primeiro, qual simplifico, qual abandono? |
| Entrega | Plano em fases + tabela de falhas + dossiêÂª HTML | Uma anêÂ¡lise por projeto + ranking + plano de 30/90 dias |

Os dois usam a mesma lêÂ³gica ê¢â¬â **aêÂ§êÂ£o ê¢â â reaêÂ§êÂ£o ê¢â â contra-aêÂ§êÂ£o** ê¢â¬â e a mesma regra: prever a barreira antes de escrever a primeira linha de cêÂ³digo.

## ConteêÂºdo

| Arquivo | O que êÂ© |
|---|---|
| [`doc/war-game-prompt.md`](doc/war-game-prompt.md) | O prompt de um projeto, em **inglêÂªs** |
| [`doc/prompt-war-game-portugues.md`](doc/prompt-war-game-portugues.md) | O prompt de um projeto, em **portuguêÂªs** |
| [`doc/mass-war-game.md`](doc/mass-war-game.md) | O modo massa, em **inglêÂªs** |
| [`doc/war-game-massa-portugues.md`](doc/war-game-massa-portugues.md) | O modo massa, em **portuguêÂªs** |
| [`doc/war-game.html`](doc/war-game.html) | DossiêÂª de exemplo (EN) gerado a partir do prompt para o caso PA-CHAT-V0 |
| [`doc/war-game-portugues.html`](doc/war-game-portugues.html) | DossiêÂª de exemplo (PT-BR) do mesmo caso |
| [`doc/exemplo-massa/`](doc/exemplo-massa/) | SaêÂ­da de exemplo do modo massa: anêÂ¡lise individual completa, resumo geral, ledger e suposiêÂ§êÂµes |

## Como usar ê¢â¬â um projeto

1. Abra `doc/prompt-war-game-portugues.md` (ou a versêÂ£o EN) e copie o conteêÂºdo inteiro.
2. Preencha os campos entre colchetes (`[PROJETO]`, `[Claude Haiku]`, `[Supabase Edge Functions]`, `[workshops/serviêÂ§os]` etc.) com os detalhes reais do seu projeto.
3. Cole como a **primeira mensagem** de uma conversa nova com sua IA de planejamento ê¢â¬â sem contexto prêÂ©vio, o prompt jêÂ¡ foi desenhado para um cold-start agent.
4. PeêÂ§a os dois entregêÂ¡veis: o plano em Markdown e a versêÂ£o visual em HTML com diagramas.
5. Execute fase por fase, conferindo os critêÂ©rios de saêÂ­da antes de avanêÂ§ar.

Veja o passo a passo detalhado, com exemplos, no [guia publicado](https://linnoff88-dev.github.io/arckhe-/guia/).

## Como usar ê¢â¬â vêÂ¡rios projetos

1. Abra `doc/war-game-massa-portugues.md` (ou a versêÂ£o EN) e monte a estrutura de pastas que ele descreve.
2. Escreva **um arquivo por projeto** ê¢â¬â nunca todos num sêÂ³. Comece pelo briefing mêÂ­nimo (5 perguntas); o que vocêÂª nêÂ£o souber, deixe em branco.
3. Preencha `contexto-geral.md` e `criterios.md`. SêÂ£o eles que tornam os projetos comparêÂ¡veis.
4. Rode o **prompt mestre** com o modelo mais capaz. Ele gera uma primeira versêÂ£o de todos, sem polir nenhum.
5. Rode o **prompt de revisêÂ£o** por cima ê¢â¬â êÂ© essa segunda rodada que tira o genêÂ©rico.
6. Leia o `resumo-geral.md`, escolha **um** projeto e entregue o war-game dele ao modelo barato com o prompt de execuêÂ§êÂ£o.

O modelo caro pensa e antecipa. O barato executa o plano jêÂ¡ mastigado.

Para saber onde vocêÂª quer chegar, veja a saêÂ­da de exemplo em [`doc/exemplo-massa/`](doc/exemplo-massa/) ê¢â¬â um portfêÂ³lio fictêÂ­cio de 4 projetos, com uma anêÂ¡lise individual completa, o resumo geral com ranking e planos de 30/90 dias, e os dois arquivos vivos (ledger e suposiêÂ§êÂµes).

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>