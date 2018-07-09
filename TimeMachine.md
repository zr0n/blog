---
layout: page
title: Nando's Time Machine
---

<p class="message">
[07-09-2018]
  Máquina do tempo - UE4 [TUTORIAL]
</p>

Olá, como estão? Fiz um tutorial em 2 vídeos, um com 1h30' e outro com 2 minutos, explicando uma forma de montar um sistema de máquina do tempo. 
Esse sistema requer algumas técnicas delicadas, porque se você quiser usar muitos objetos dentro dele, não poderá consumir muita memória ram, que é onde as variáveis ficam guardadas. Essa é a parte interessante do desafio, porque nós precisávamos de arrays que memorizassem a trajetória, rotação e escala dos atores, e também precisávamos que esses arrays não fossem muito grandes. A forma como eu solucionei, foi não usar o tick, que é executado em todo frame, para memorizar, e sim criar um intervalo padronizado de tempo (0,2 segundos) para guardar esses valores. Considerando que o tick em 60 fps executa uma vez a cada 0,016 segundos, essa técnica permitiu salvar mais de 90% da memória ram que seria utilizada. Para permanecer com transições suaves, usei a famosa técnica de interpolação linear (lerp), para transitar de um estado ao outro.

Outro grande desafio, é fazer isso com inteligência artifical. Precisaríamos garantir que um personagem que se movimenta aleatoriamente pelo ambiente, que ao voltar no tempo, e então voltar a velocidade normal, fizesse o mesmo trajeto que tinha feito antes, para criar aquele efeito que a Ubisoft fez em Prince of Persia - The Sands of time. Para isso, toda as vezes que o personagem regredia, eu salvei uma array separada, memorizando por onde ele voltou, para quando retornasse a velocidade normal pudesse seguir exatamente a mesma trajetória, e só quando não tivesse mais trajetória para seguir sorteasse um novo caminho para percorrer.
Usei técnicas de play rate para ajustar as animações.

Para permitir escolher qual personagem não seria afetado pela manipulação do tempo, tivemos que usar uma dose de bruxaria também. Como estava usando dilatação do tempo, precisamos fazer um cálculo para normalizar a velocidade de movimento e das animações. Como a animation blueprint é afetada pela dilatação do tempo, tivemos que que recalcular o input do blend space, para a animação do personagem que se move em paralelo ao tempo pudesse funcionar corretamente 

Tem muito mais coisa no vídeo, acho que vale a pena conferir. Sintam-se livres para adaptarem como convir a sua necessidade.
<div class="videoWrapper">
  <iframe width="1663" height="732" src="https://www.youtube.com/embed/MeOh9XI5s-k" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="videoWrapper">
  <iframe width="1663" height="732" src="https://www.youtube.com/embed/iTIAQbGm2E4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>