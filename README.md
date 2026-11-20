# War Game Prompt

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Prompt reutilizÃ¡vel que transforma o planejamento de qualquer build de IA num **war game**: em vez de assumir o caminho feliz de A a B, forÃ§a a IA a quebrar o projeto em fases, cada uma com objetivo, suposiÃ§Ã£o otimista, suposiÃ§Ã£o pessimista, modos de falha provÃ¡veis com correÃ§Ã£o, critÃ©rios de saÃ­da verificÃ¡veis, caminho alternativo, condiÃ§Ã£o de parada e orÃ§amento de tentativa â€” alÃ©m de uma tabela mestre de riscos (infra, API do modelo, frontend, qualidade de conversa, seguranÃ§a, loop de aprendizado) e um loop semanal de autoavaliaÃ§Ã£o.

ðŸ“– **Guia completo (landing + passo a passo):** https://inematds.github.io/promptwargame/guia/

## Dois modos

| | **War Game** | **War Game em Massa** |
|---|---|---|
| Para | Um projeto, a fundo | VÃ¡rios projetos, comparados |
| Responde | Como construir isso sem levar porrada no caminho? | Tenho N projetos parados â€” qual faÃ§o primeiro, qual simplifico, qual abandono? |
| Entrega | Plano em fases + tabela de falhas + dossiÃª HTML | Uma anÃ¡lise por projeto + ranking + plano de 30/90 dias |

Os dois usam a mesma lÃ³gica â€” **aÃ§Ã£o â†’ reaÃ§Ã£o â†’ contra-aÃ§Ã£o** â€” e a mesma regra: prever a barreira antes de escrever a primeira linha de cÃ³digo.

## ConteÃºdo

| Arquivo | O que Ã© |
|---|---|
| [`doc/war-game-prompt.md`](doc/war-game-prompt.md) | O prompt de um projeto, em **inglÃªs** |
| [`doc/prompt-war-game-portugues.md`](doc/prompt-war-game-portugues.md) | O prompt de um projeto, em **portuguÃªs** |
| [`doc/mass-war-game.md`](doc/mass-war-game.md) | O modo massa, em **inglÃªs** |
| [`doc/war-game-massa-portugues.md`](doc/war-game-massa-portugues.md) | O modo massa, em **portuguÃªs** |
| [`doc/war-game.html`](doc/war-game.html) | DossiÃª de exemplo (EN) gerado a partir do prompt para o caso PA-CHAT-V0 |
| [`doc/war-game-portugues.html`](doc/war-game-portugues.html) | DossiÃª de exemplo (PT-BR) do mesmo caso |
| [`doc/exemplo-massa/`](doc/exemplo-massa/) | SaÃ­da de exemplo do modo massa: anÃ¡lise individual completa, resumo geral, ledger e suposiÃ§Ãµes |

## Como usar â€” um projeto

1. Abra `doc/prompt-war-game-portugues.md` (ou a versÃ£o EN) e copie o conteÃºdo inteiro.
2. Preencha os campos entre colchetes (`[PROJETO]`, `[Claude Haiku]`, `[Supabase Edge Functions]`, `[workshops/serviÃ§os]` etc.) com os detalhes reais do seu projeto.
3. Cole como a **primeira mensagem** de uma conversa nova com sua IA de planejamento â€” sem contexto prÃ©vio, o prompt jÃ¡ foi desenhado para um cold-start agent.
4. PeÃ§a os dois entregÃ¡veis: o plano em Markdown e a versÃ£o visual em HTML com diagramas.
5. Execute fase por fase, conferindo os critÃ©rios de saÃ­da antes de avanÃ§ar.

Veja o passo a passo detalhado, com exemplos, no [guia publicado](https://inematds.github.io/promptwargame/guia/).

## Como usar â€” vÃ¡rios projetos

1. Abra `doc/war-game-massa-portugues.md` (ou a versÃ£o EN) e monte a estrutura de pastas que ele descreve.
2. Escreva **um arquivo por projeto** â€” nunca todos num sÃ³. Comece pelo briefing mÃ­nimo (5 perguntas); o que vocÃª nÃ£o souber, deixe em branco.
3. Preencha `contexto-geral.md` e `criterios.md`. SÃ£o eles que tornam os projetos comparÃ¡veis.
4. Rode o **prompt mestre** com o modelo mais capaz. Ele gera uma primeira versÃ£o de todos, sem polir nenhum.
5. Rode o **prompt de revisÃ£o** por cima â€” Ã© essa segunda rodada que tira o genÃ©rico.
6. Leia o `resumo-geral.md`, escolha **um** projeto e entregue o war-game dele ao modelo barato com o prompt de execuÃ§Ã£o.

O modelo caro pensa e antecipa. O barato executa o plano jÃ¡ mastigado.

Para saber onde vocÃª quer chegar, veja a saÃ­da de exemplo em [`doc/exemplo-massa/`](doc/exemplo-massa/) â€” um portfÃ³lio fictÃ­cio de 4 projetos, com uma anÃ¡lise individual completa, o resumo geral com ranking e planos de 30/90 dias, e os dois arquivos vivos (ledger e suposiÃ§Ãµes).

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>