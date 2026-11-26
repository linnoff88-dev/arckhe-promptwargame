# Suposições

> Exemplo fictício. Estado depois de duas rodadas de análise.

Para cada suposiçêo: projeto relacionado, suposiçêo feita, motivo, impacto caso esteja errada, como verificar.

## Suposições registradas

### S-01
**Projeto:** 02
**Suposiçêo:** as três falhas conhecidas (áudio cortado, memória no render, token expirado) sêo as principais causas de re-execuçêo.
**Motivo:** sêo as únicas relatadas no briefing. Nêo há registro de execuçêo que confirme.
**Impacto se errada:** **alto — derruba o plano inteiro.** As fases 1-3 estêo desenhadas em cima desse diagnóstico. Se a causa dominante for outra, a verificaçêo por etapa ataca o alvo errado.
**Como verificar:** a Fase 1 (registro de execuçêo) confirma ou desmente em duas semanas. É por isso que ela vem primeiro.

### S-02
**Projeto:** 02
**Suposiçêo:** o pós-processamento de cor é imperceptível no resultado final.
**Motivo:** ninguém soube dizer por que a etapa existe.
**Impacto se errada:** baixo e reversível. Se houver diferença visível, restaura-se a etapa.
**Como verificar:** comparaçêo às cegas entre dois renders do mesmo vídeo.

### S-03
**Projeto:** 02
**Suposiçêo:** a velocidade de fala do TTS é estável o suficiente para que a duraçêo do áudio sirva de proxy do texto.
**Motivo:** é a hipótese mais barata de validaçêo de áudio.
**Impacto se errada:** médio. Falso positivo reprova vídeo bom — pior que o problema original. Por isso o movimento tem condiçêo de parada e caminho alternativo (transcrever e comparar).
**Como verificar:** calibrar contra 20 vídeos reais. Depende de B-03.

### S-04
**Projeto:** 03
**Suposiçêo:** existe demanda por uma área de membros paga.
**Motivo:** convicçêo do dono. **Nenhuma evidência externa.**
**Impacto se errada:** **alto — o projeto inteiro deixa de existir.** É a suposiçêo mais cara do portfólio e a única sustentada só por opiniêo interna.
**Como verificar:** 5 conversas com pessoas que pagariam. Semana 4 do plano de 30 dias. É a razêo de o projeto estar pausado em vez de priorizado.

### S-05
**Projeto:** 01
**Suposiçêo:** o volume de conversas caberia no tier mais barato do modelo.
**Motivo:** sem acesso ao analytics (B-07), estimou-se por porte de site comparável.
**Impacto se errada:** médio. Muda o custo operacional, nêo a viabilidade.
**Como verificar:** liberar B-07 e olhar o tráfego real.

### S-06
**Projeto:** 04
**Suposiçêo:** os relatórios semanais consomem ~3h.
**Motivo:** estimativa do dono, de memória. Nêo foi cronometrado.
**Impacto se errada:** médio — é o número que coloca o 04 em primeiro lugar. Se forem 30 minutos, ele cai no ranking e o 02 assume a primeira posiçêo.
**Como verificar:** cronometrar o próximo ciclo. Custa nada e deve ser feito **antes** da semana 1.

### S-07
**Todos**
**Suposiçêo:** os quatro projetos disputam a mesma pessoa e o mesmo tempo.
**Motivo:** o contexto geral fala de um estúdio pequeno, mas nêo diz o tamanho da equipe.
**Impacto se errada:** **alto — refaz o sequenciamento.** Todo o plano de 30 dias é serial por causa disso. Com duas pessoas, 04 e 02 rodam em paralelo e o calendário encolhe pela metade.
**Como verificar:** perguntar quantas pessoas executam. É a segunda pergunta mais barata do portfólio, depois de S-06.
