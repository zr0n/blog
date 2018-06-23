---
layout: post
title: Diário GameDev - AirGear Dia 47

---

Hoje fizemos um dome sci fi, que detecta a presença do jogador, e quando o mesmo se aproxima, é criada uma rede que o prende dentro da área jogável. Corrigimos alguns bugs, como por exemplo o de colisão com objetos estáticos no client. Ao client colidir em algo estático, tinha um leve bug causado por discrepância entre o cliente e o servidor, isso é algo já conhecido no sistema de réplica da engine, o node ADD IMPULSE funciona baseado no framerate, logo, mesmo se você usar add impulse no server e no client, vai gerar posições finais diferentes, porque raramente o framerate do cliente será como o do servidor, tirando o lag de envio de pacotes. Achamos uma solução para isso, e modificamos a velocidade e controle das aeronaves.

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="732" src="https://www.youtube.com/embed/eKG46baaLMQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>