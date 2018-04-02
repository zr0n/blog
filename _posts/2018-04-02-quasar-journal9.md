---
layout: post
title: Diário GameDev - Quasar dia 9
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Hoje trabalhei um pouco melhorando o sistema de inteligência artificial para inimigos e aliados. Ainda não está perfeito devido a um pequeno bug com os inimigos e os aliados estão se sobrepondo, porém ambos problemas são fáceis de solucionar. Fiz um sistema de interface, para que os atores que vão aparecer no minimap pudessem ter o tamanho de seu ícone definido de forma dinâmica. Hoje foquei na movimentação da nave principal, que fica no centro da tela. Fiz um componente vetor, que aponta na direção em que ela deve estar, e ela sempre se moverá na direção desse vetor. Uma vez que a nave estiver totalmente fora da tela, o jogador irá perder o jogo, consegui implementar isso de forma bem básica hoje também. Consegui resolver um bug visual, que eram as naves entrando dentro da nave principal, agora elas passam por cima. 
PS: As naves aliadas são imortais por motivos de teste, por isso se sobressaem bem melhor que os inimigos.

Foi um dia relativamente bem produtivo, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/9Bof0MRzuws" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<p class= "message"> - Luiz Fernando </p>