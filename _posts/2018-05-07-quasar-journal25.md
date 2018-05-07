---
layout: post
title: Diário GameDev - Quasar Dia 25
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Cara, hoje tive um pouco de trabalho, mas sem sombra de dúvida foi um dia compensador. Reescrevi a forma como todas as naves se movimentam, em vez de fazer usando o movimento de vôo tridimensional, resolvi aplicar um plano invisível com movimento em 2 direções. É como se as naves fossem personagens andando no chão, só que o chão é invisível. Essa decisão foi tomada por inúmeros benefícios, mas o que se destaca dentre eles, é o uso do famoso nav mesh. 

Se por algum motivos precisarmos de pathfinding no futuro (Pathfinding é um algoritmo que calcula caminhos, o GPS do google maps é um exemplo de path finding), perderíamos muito tempo e sanidade tendo que implementar um pathfinding próprio. Assim podemos aproveitar o já bem testado e aprimorado algoritmo pronto da engine, que até onde vai meu conhecimento, só funciona para personagens que caminhem em um plano. 

Aproveitei que reescrevi o componente de movimento, para aprimorar a AI. Com 2 linhas de código em C++ (que achei pronto xD) consegui implementar as AI's de uma forma que a velocidade delas não seja totalmente desacelerada ao encontrar o ponto no mapa que elas buscam, que resumidamente foi "fazer as naves deslizarem", e não pararem imediatamente, dando uma sensação robótica como antigamente. Aproveitei para ativar uma opção chamada RVO Avoidance, RVO significa Reciprocal Velocity Obstacle. Reciprocal vem de recíproco, e Velocity Obstacle pode ser encontrado nesse [link aqui](https://en.wikipedia.org/wiki/Velocity_obstacle)

Resumidamente o que o RVO faz, é evitar que a AI colida com outros AI's. Então ela traça um caminho tendo em vista o caminho que as outras AI's vão traçar e evita colisão. Isso é muito maneiro, porque parece que as AI's são pro players. 

Consertei diversos bugs também, a mecânica principal já está ficando com cara de pronta. 

Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="734" src="https://www.youtube.com/embed/as-vq989tj8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>