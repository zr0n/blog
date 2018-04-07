---
layout: post
title: Diário GameDev - Quasar dia 12
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Resolvemos cancelar o espelhamento das paredes, aquele esquema de teleportar o player na direção oposta quando ele passasse do limite do mapa. Agora vamos usar a área do mapa como uma área segura, e sempre que o jogador sair dessa área, receberá uma estática, como se estivesse perdendo o sinal. Ele também levará dano por segundo, enquanto estiver fora da área segura. Para fazer isso utilizei uma widget simples, com apenas um texto e uma animação feita no próprio UE4. Usei também um post process com um material cheio de panners, para fazer aquela linha de estática subindo, como em TV's antigas.


Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/7vISP3poro4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>
