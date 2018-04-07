---
layout: post
title: Diário GameDev - AirGear - 3 dias 
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.


Então, resolvi antes de mais nada implementar o sistema de multiplayer no AirGear. Levei 3 longos dias até deixar o sistema de chat, matchmaking, lan, steam, lobby e a fase estáveis. Tive alguns problemas, dentre eles, um dos que me deu mais dor de cabeça, foi replicar o momvimento das naves. Depois de algum tempo tentando fazer meu próprio sistema de réplica de movimento, descobri que ia perder performance ou tempo demais até fazer algo eficaz. Percebi que a melhor alternativa seria usar o CharacterMovement do UE4, tive que reescrever toda a movimentação da nave, 2 vezes inclusive, porque antes do character movement, tentei usar flying pawn movement (o qual não tem o movimento replicável). Nem gravei o código nesse vídeo, porque ficou bem bagunçado, tenho que arrumar a zona que ficou lá ainda xD

Segue um vídeo abaixo de como ficou: 

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/EQ6dNE2QSUQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>  


<p class= "message"> - Luiz Fernando </p>