---
layout: post
title: Diário GameDev - Quasar Dia 26
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Voltando ao desenvolvimento do quasar. Hoje fizemos mais umas alterações nas naves bots, limitamos os spawn points para sempre verificar a quantidade de inimigos antes de spawnar. Exemplificando: Se o máximo de inimigos no spawn points for 2, ele só vai spawnar o próximo quando tiverem 2 ou menos inimigos no level.

Uma das principais mudanças que implementamos também foi a parallax, para dar ideia de movimento. O efeito parallax se trata de dividir um elemento visual em camadas, e mover essas camadas em diferentes velocidades. Isso deveria ser automático, mas pela skybox ser um elemento muito grande e estar muito afastada da tela, o deslocamento normal da câmera quase não surte efeito. Então criei uma função para calcular o deslocamento do jogador, inverter esse valor, multiplicar pela velocidade que eu queria que a skybox se movesse, e então aplicar esse deslocamento na skybox

Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="734" src="https://www.youtube.com/embed/FD0Ju1NIP7s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>