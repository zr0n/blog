---
layout: post
title: Diário GameDev - AirGear Dia 46

---

Tá ficaodo um pouco difícil gravar vídeos periódicos do air gear, porque estamos em uma fase muito instável de experimentações. Nos últimos dias refizemos a HUD. Testamos um framework da nvidia e acabamos optando por não implementar. Colocamos um indicador para quando o jogador estiver com pouca vida (borda vermelha na tela piscando). Fizemos um indicador de quando os status do jogador mudam, para deixar o jogo mais transparente. Exemplo: "Invincible", "Speed +10", "Attack -30" e etc.

E acho que a modificação mais visível: Implementamos um toon shader, que é a mistura do famoso cel shading com um outliner. Caiu muito bem, mudamos quase radicalmente a nossa identidade visual. Daqui para frente vamos desenvolver já para se encaixar nesse ambiente gráfico.

Também corrigimos diversos bugs, e no mais foi isso.

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="683" src="https://www.youtube.com/embed/eQXHFcl8DZw" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>