---
layout: post
title: Diário GameDev - AirGear Dia 37

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Hoje implementamos algumas coisas na HUD. Primeiramente implementamos aquela "bússola linear", que pra ser sincero eu não sei se o nome é esse. Mas é aquela bússola que parece uma régua, que fica no topo da tela, muito presente em jogos Battle Royale/Battlegrounds, como em Fortnite. Implementamos as barras de shield, turbo e vida de forma circular também. Implementamos um velocímetro para ficar mais transparente para o jogador os dados do mundo simulado.

De tudo que fizemos hoje, o mais interessante foi desenvolver a bússola linear, porque precisamos criar uma "imagem infinita", ou pelo menos algo que desse efeito. Devem ter diversas formas de fazer isso, mas a que encontramos foi a de fazer uma imagem com a bússola que vai de 0 a 360 graus. Colocamos essa imagem 3 vezes maior, extendendo ela para esquerda e para direita, além da área visível, e então fazemos um cálculo para não deixar nunca a imagem sair da tela. Como fazemos isso? É bem simples, pare para pensar em os ângulos de uma circunferência. Em 360°, você dá uma volta em uma circunferência, você volta ao ponto 0, sendo assim, 540° apontarão para o mesmo ponto que 180° aponta, exceto que 360° tem uma volta a mais. O que fazemos então é normalizar a posição da imagem. Imagine se quando está em 260° a imagem esteja na posição de 600px. Caso o jogador comece a rotacionar o plano, uma hora ele vai chegar no mesmo ponto, como no caso de 580°, então nós podemos em vez de exibir a posição de 580º, voltamos ela para a posição 600px (260º), dando a noção de que estamos rolando uma imagem infinita.

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="685" src="https://www.youtube.com/embed/XIar6k-xx7I" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>