---
layout: post
title: Diário GameDev - AirGear Dia 17

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Implementado sistema de skills e cooldowns. Nos inspiramos bastante em MOBAS, até mesmo porque teremos uma modalidade MOBA dentro do jogo, além dessa deathmatch padrão. Conseguimos implementar os 4 skills da dupla de pilotos Vallete e Danma. Criamos também um sistema de estados cumulativos, estados como: invisibilidade, aumento de força, defesa e etc. Exibimos esses estados no target, e também na HUD. Por enquanto estamos usando imagens placeholder, não só nisso como em toda a HUD.
Skills do Vallete e Danma:

Vallete e Danma (Ás e Atiradora):

Q – Rush: Danma força o motor, permitindo que ele, dentro de 3 segundos, utilize o turbo sem haver gastos. Durante o período, o avião recebe 30% de chance de bloquear qualquer fonte de dano. Cooldown 20 segundos.
W – Pump up: Vallete toma animo pela batalha, durante 5 segundos todas as fontes de dano tem sua força aumentada em 40%, no entando, Vallete e Danma recebem 20% de dano a mais, durante o mesmo período. Cooldown 10 segundos.
E – Shazam!: Danma ativa um dispositivo de camuflagem que deixa o avião invisível por 7 segundos e cancela qualquer tipo de efeito debilitativo. Alvos invisíveis não deixam de ser perseguido por armas teleguiadas desde que estas tenham marcado o alvo antes dele ficar invisível. Cooldown 20 segundos.
R – Royal Flush: Danma e Vallete se tornam temporariamente (6 segundos) imbatíveis, mitigando 80% do dano recebido, além ter o efeito positivo de “Pump up” ativo, mesmo que em cooldown. Kills causados durante o Royal Flush, diminuem o tempo de recarga dessa skill em 10 segundos, e recarregam o efeito de “Shazam” imediatamente. Ativar “Shazam!” anula o efeito de Royal Flush. Cooldown 80 segundos.


Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/9I8fB3R3GbU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>