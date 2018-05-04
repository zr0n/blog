---
layout: post
title: Diário GameDev - AirGear Dia 20

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Continuando a trabalhar nas skills da dupla Jessy and Joel, resolvi o barrel roll que estava meio bugado no fim do dia de ontem. Foi desenvolvida também a primeira skill do drone assistente. Aqui tivemos um problema de implementação de gameplay, porque o tiro deveria partir do drone, mas quem controla a mira é o jogador. Como o drone se movimenta livremente, apesar de acompanhar o jogador, enfrentamos o problema de ter que implementar um projétil o qual o player guiasse a direção e o tiro fosse disparado a partir do drone, que poderia estar em qualquer lugar e em qualquer rotação da tela. 

Para resolver isso, rebusquei lá no fundo da memória, nos primórdios da minha era gamer "online", o jogo chamado gunbound. Nesse jogo tinha um veículo chamado A. Sate, onde você atirava com o jogador/veículo, fazendo um movimento parabólico, e era marcada a posição onde esse projétil acertava. Em uma fração de segundo depois, era lançado um tiro em linha reta na direção em que o projétil marcou. Caso não conheça, busque por Gunbound A. Sate no youtube.

Isso era justamente o que precisávamos, apresentei a ideia para o resto da confraria e me deram o aval para implementar. Fiz uma lógica então com 2 projéteis, sendo o primeiro destes, um marcador. Depois de acertar algo, o drone vira e lança um tiro naquela direção. Enfrentamos um problema extra, que é o fato de até o drone se virar e atirar, o alvo poderia já ter se movido. Resolvi então salvar uma referência do objeto que foi atingido pelo marcador, assim o drone sempre teria um ponto em tempo real de onde mirar, logo pode se virar suavemente e atirar de qualquer lugar que esteja. Ao drone acertar o tiro, o alvo recebe diminuição na velocidade de movimento em 25% por 3 segundos. 


Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="685" src="https://www.youtube.com/embed/XoA_iREkZqM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>