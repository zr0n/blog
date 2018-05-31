---
layout: post
title: Diário GameDev - AirGear Dia 38

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Hoje demos continuidade nas alterações da HUD. Tínhamos que criar um chat e não fazíamos ideia de como fazê-lo. Uma dificuldade era fazer um chat sem poluir a tela, e fazer também que o jogador pudesse navegar pelo chat com o scroll do mouse. A solução que achamos para isso foi, uma vez que o scroll do mouse não tinha importância no jogo, redirecionar toda entrada do scroll do mouse na widget. Ou seja, criei um evento de scroll próprio que funciona até quando a widget não está em destaque. Ao apertar enter, damos foco na widget e impedimos que o jogador use qualquer tecla de comando na nave, para não interferir na digitação da mensagem.

Implementamos mensagens globais e em time, onde a grande diferença é que, na primeira todos vêem a mensagem, independente do time, enquanto a segundo só é visível para jogadores que possuírem o mesmo time de quem enviou a mensagem. Para enviar mensagem global, escolhemos a combinação de teclas ctrl + enter, caso o ctrl não seja apertado, será enviada uma mensagem visível apenas para o time.

A parte mais divertida foi implementar a ideia do Wesley, de fazer uma engrenagem rodando por um trilho, dando uma ideia bem steam punk, além de, a engrenagem ser um dos principais símbolos da identidade do jogo (Gear significa engrenagem). Fizemos uma animação da engrenagem rodando para um lado quando a tela de chat expande e para o outro quando a janela se retrai. Mudamos também a opacidade do fundo da janela, para não atrapalhar a visão do jogador enquanto ele não estiver com foco no chat, ao focar no chat (apertar enter) a opacidade aumenta, deixando o fundo da janela menos transparente e as mensagens mais legíveis.  

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1653" height="665" src="https://www.youtube.com/embed/hvb85jU8q-s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>