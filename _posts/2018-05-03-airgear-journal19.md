---
layout: post
title: Diário GameDev - AirGear Dia 19

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Materiais do Skyhawk foi melhorado um pouco. Demos início as skills da segunda dupla de piloto/atirador, que no caso são Joel e Jessy. Uma grande dificuldade dessa dupla é que eles vão possuir um droid que vai ficar seguindo a aeronave, eu não queria deixar parecendo algo preso a nave, busquei de todas as formas fazer parecer como uma nave acompanhante e não um simples componente. Perdi algumas horas nisso, a melhor solução que encontrei foi escrever na mão o movimento do componente, fazer a velocidade diretamente proporcional a distância que o droid está da nave a qual acompanha. Dessa forma como o usuário usar o turbo, vai ter a impressão de que o droid usou o turbo também, pouco tempo depois, para alcançar o usuário. 

O barrel roll não tá ideal, a nave tá tremendo quando usa, mas estava funcionando antes xD. Fiquei tão focado no droid, que devo ter alterado alguma coisa que prejudicou o funcionamento desse barrel roll, mas como estou esgotado vou deixar para resolver isso da próxima vez que for corrigir bugs. Quando isso acontece, geralmente é porque o servidor, que é autoritativo está alterando a posição de um actor enquanto o cliente, que tem uma versão replicável desse ator, também tenta alterar essa posição.


Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/o2qlwiE18YA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>