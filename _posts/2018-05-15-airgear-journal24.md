---
layout: post
title: Diário GameDev - AirGear Dia 24

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Hoje fiz uma fórmula para calcular o dano exercido sobre o personagem quando ele colide com algum objeto do mundo. Essa formula se baseia em o quão rápido o avião está, quanto de armadura o avião tem e o quanto a nave está rotacionada na direção do ponto de impacto. Obter esse último valor, foi o grande desafio do dia. Explicando melhor, esse valor serve para causar mais dano caso o avião bata de frente, causar menos dano caso pegue de raspão. No vídeo eu mostro a fórmula, que é essa: 

(1 - Armadura) * FatorDeColisãoPorImpacto * [360 - Magnitude(Normal([(RotaçãoDoPersonagem) - (Rotação do ponto de impacto)])) * [(Velocidade) / (VelocidadeMáxima)]]

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="685" src="https://www.youtube.com/embed/wc2pB0dIeOo" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>