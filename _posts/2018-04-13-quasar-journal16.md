---
layout: post
title: Diário GameDev - Quasar dia 16
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Hoje resolvi uns bugs de jogabilidade, relacionados a nave principal. Mudei a forma que a torreta lança o laser, em vez de o dano ser em linha reta agora será em um alvo fixo, decidimos que seria assim por motivos estéticos. MAS O MAIS IMPORTANTE foi fazer o sistema mostrando dano quando acerta algum personagem "danificável" no mapa do jogo.

Extraímos essa ideia de uma rapida sharingada no ragnarok. A razão de isso estar presente, é para deixar o jogo mais transparente, e os projéteis serão reimplementados, dessa vez vão trespassar o jogador caso o dano do projétil seja maior que a vida do jogador. Exemplificando: Se um projétil possui o valor de dano de 300 e atinge um jogador com 200 de vida, irá matar esse doido e mudará seu valor de dano para 100, podendo acertar ainda mais algum danificável e descontar esse valor restante. 


Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1653" height="709" src="https://www.youtube.com/embed/f-KHXGrFBck" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>
