---
layout: post
title: Diário GameDev - AirGear Dia 47~50

---

Depois de 3 dias de árduo trabalho, conseguimos elaborar e começar a implementar a solução do nosso server dedicado. Agora, em vez de 1 jogador ser o host e outros ingressarem no servidor que ele abrir, iremos usar um serviço centralizado, criado por nós mesmos. Conseguimos elaborar o sistema de login e senha utilizando NodeJS (com diversos modules), MongoDB (Banco de dados) e o UE4 como cliente frontend. Usamos tecnologias padrões web RESTful para fazer a autenticação/cadastro, isso foge um pouco do desenvolvimento do jogo em si, logo não vejo muito porque abordar isso aqui. O formulário ainda está mockado, não planejamos um design ainda, então por favor "não reparem na casa bagunçada".

Fizemos um diagrama de como será nosso modelo de conexão, [que pode ser encontrado aqui](https://www.facebook.com/photo.php?fbid=1106885549453514&set=a.138416599633752.31585.100003962385728&type=3)

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/6-89sTPb6S0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>