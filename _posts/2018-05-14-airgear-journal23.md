---
layout: post
title: Diário GameDev - AirGear Dia 23

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Hoje o dia foi bem tranquilo. Ainda to me recuperando do desgaste da última dupla que fizemos, então resolvi puxar umas tarefas simples de desenvolver, porém fundamentais para o jogo. A tarefa de hoje foi fazer o indicador de dano, que mostra a direção a qual o dano veio. A lógica foi tão simples e compacta, que inclusive resolvi mostrar o código no vídeo. 

Usei as funções geométricas básicas da engine para conseguir achar a direção tridimensional de onde o dano vem, usando o node Find Look at Rotation. Então, fiz um delta entre a rotação atual do jogador e a direção de onde o tiro vem. O delta basicamente é a diferença entre 2 Vetores de Euler, também conhecidos como Rotators. Tendo o rotator dessa diferença, pude eliminar os 2 ângulos que não me interessavam (Pitch e Roll) e usei o Yaw, que é a rotação em torno do eixo Y, com isso consegui o ângulo entre o jogador e o causador do dano, sendo visto de cima. 

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="734" src="https://www.youtube.com/embed/eTnFG013t34" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>