---
layout: post
title: Diário GameDev - AirGear Dia 51~53

---

Nos 3 últimos dias, conseguimos implementar o básico do nosso sistema de partidas usando um server dedicado. Envolveu todo um fluxo complicado, porque nós tivemos que fazer:

- Monitorar como os servers seriam abertos (lembrando que será 1 processo do UE4 por partida jogada)
- Permitir que os usuários criassem salas, monitorando se o mesmo já não estava ingressado em uma sala
- Permitir que os outros usuários listassem as salas já abertas, fizemos isso guardando uma lista de salas, atreladas ao process ID e a porta que a mesma usa
- Permitir que outros usuários pudessem ingressas na sala
- Achar uma forma de quem criou a sala ter uma autoridade maior que os outros usuários, como por exemplo decidir quando iniciar a partida
- Permitir o ingresso somente de usuários logados

Estamos entrando em um patamar difícil, porém bastante divertido. Estou tendo a oportunidade de aprender e testar teorias que sempre tive em mente, mas nunca implementei.

Como disse no post anterior, fizemos um diagrama de como será nosso modelo de conexão, [que pode ser encontrado aqui](https://www.facebook.com/photo.php?fbid=1106885549453514&set=a.138416599633752.31585.100003962385728&type=3)

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="1663" height="683" src="https://www.youtube.com/embed/iOtN3Bah5nw" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>