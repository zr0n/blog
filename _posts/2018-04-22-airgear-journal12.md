---
layout: post
title: Diário GameDev - AirGear Dia 12
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Estou feliz com as novidades. Hoje consegui implementar algo que vinha tirando meu sono há algum tempo, que era a remover a vantagem que o jogador host tem sobre os clientes. Consegui fazer isso passando a autoridade sobre o movimento da nave para os clientes, sendo assim a mesma forma que o cliente vê o server se mover é a forma como o server vê o cliente se mover, sempre dependendo da conexão dos 2, e não somente do cliente como estava antes. 

Isso é um problema muito grave, porque tive que deixar a autoridade no cliente, porém repliquei as regras de movimentação do servidor para o cliente, sendo assim, mesmo o cliente sendo responsável por mover a própria nave, sempre terá que obedecer um conjunto de regras como velocidade máxima, aceleração máxima entre outras.

Mudamos também a forma como a câmera e a nave se movimentam. Agora a câmera nunca fica de cabeça para baixo, melhoramos bastante a mira também. Além disso implementamos 2 partículas diferentes, a de velocidade do turbo e uma de explosão quando o jogador morre. No vídeo a explosão tá gigante, porque esqueci de regurar a escala, mas tá valendo.

Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/A5DmowBQXR4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>