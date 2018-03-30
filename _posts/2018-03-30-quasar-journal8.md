---
layout: post
title: Diário GameDev - Quasar dia 8
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Hoje tive somente 2 horas para programar, porque tive que resolver problemas com meu pc, configurar meu ssd novo e instalar tudo de novo. Resolvi focar no que conseguiria fazer a ponto de conseguir gerar algum conteúdo em vídeo para o diário já que ontem não fiz nada. 

Resolvi dar início ao sistema de aliados. Pelo projeto estar bem componentizado, eu consegui usar a mesma lógica tanto para inimigo quanto para aliados, as únicas variáveis que mudam são: uma indicando se aquele personagem é inimigo ou não; e outra indicando a cor que eu usei para diferenciar inimigos de aliados. Lembrando que todos os modelos são placeholders, e serão substituídos no futuro.

Para fazer essa lógica compartilhável, precisei substituir a inteligência artifical antiga, que só focava o player principal, para focar no alvo mais próximo, e atualizar esse alvo periodicamente. Para isso, usei a função de ordenar arrays, do framework do Unreal Engine e [que se encontra nesse link](http://api.unrealengine.com/INT/API/Runtime/Core/Containers/TArray/Sort/1/index.html). Primeiramente busquei todos os personagens que fossem do time oposto, no caso se a nave fosse do time inimigo, buscava todos os aliados, e se fosse do time aliado, buscava todos os inimigos. E então ordenei esse resultado por distância da nave em questão, em ordem crescente. Fazendo isso, bastou pegar o primeiro elemento, que logicamente seria o mais próximo. 

Sabendo como pegar o inimigo mais próximo, e colocando ele como alvo no meu sistema de AI, todo o resto já estava pronto. Esse é um exemplo que vale para ressaltar a importância de sempre fazer código incrementável e reutilizável. Vejam abaixo como ficou na prática. 

Vídeo do sétimo dia:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/hkbszY0Xhyg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<p class= "message"> - Luiz Fernando </p>

