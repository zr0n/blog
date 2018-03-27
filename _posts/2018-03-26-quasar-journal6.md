---
layout: post
title: Diário GameDev - Quasar dia 6
---

Olá amigos, como estão? Hoje foi o sexto dia do desenvolvimento do Quasar. Desenvolvi o sistema de limite de campo, e toda vez que o jogador alcançar alguma das 4 paredes limite, é teleportado em direção oposta. Para fazer isso trabalhei com sistema de line trace que o Unreal Engine fornece (também conhecido como Raycast), basicamente precisei verificar quando o jogador se choca contra a parede, calcular o inverso normalizado do vetor da velocidade  (basicamente pegar a direção oposta em que o jogador está se movendo, só quis falar bonito xD), e então traçar uma linha nessa direção, ver onde a linha bate e então mover o jogador para lá. Isso deixou o mapa "infinifo". Implementei os novos meshs, que ainda estão sem material, apliquei um material metálico para os inimigos apenas. Coloquei um lagg na câmera, para ajudar a dar sensação de movimento/velocidade na nave, sensação a qual vai ser melhor experimentada ainda, quando tivermos nosso sistema de parallax pronto. Segue o vídeo mostrando como ficou:

Vídeo do sexto dia:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/KGlsOQx_HTg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<p class= "message"> - Luiz Fernando </p>

