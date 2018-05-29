---
layout: post
title: Diário GameDev - AirGear Dia 36

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Além de corrigir alguns dos inúmeros bugs, implementamos um radar. Esse radar atualiza todas as posições a cada 0,5 segundos. Poderíamos ter colocado as posições em tempo real, como é em um minimap, mas quisemos preservar essa ideia de radar. O posicionamento do radar ocorre por grupos de distância.
Até 30m o inimigo fica bem próximo do centro.
De 30 à 60 ele continua na menor circunferencia porém um pouco mais próximo da borda.
De 60 à 80 ele fica na segunda circunferência do radar.
de 80 à 100 ele fica na última circunferência.
Acima de 100m de distância o radar não detecta. 


Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="734" src="https://www.youtube.com/embed/-9OAA4ICoyY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>