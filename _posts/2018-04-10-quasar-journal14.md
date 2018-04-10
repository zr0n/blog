---
layout: post
title: Diário GameDev - Quasar dia 14
---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo Quasar e falando um pouco sobre o que eu fiz.

Na lógica do jogo Quasar, as naves principais são abastecidas por unidades de energia central, as quais chamamos de Cores. Para dar essa ideia de "Energia", resolvemos usar um cristal rodando em cima de uma base, sugerindo que seja um gerador que utiliza uma fonte de energia desconhecida em nosso mundo real. Como não usamos barra de energia, percebi que seria um problema para o jogador ter uma noção de quanto dano faltava para o core ser destruído. Isso se agravaria mais ainda pelo fato de o core ser algo um pouco mais durável do que as outras estruturas que temos no jogo, foi quando dei a ideia de usarmos um material que muda de cor de acordo com a quantidade de vida do inimigo.

A implementação em si foi bem simples, porque criei uma classe que herda da BaseEnemy, que é a nossa classe com toda a configuração do inimigo que pode ser atingido pelo jogador. Logo, bastou alterar os valores de vida, criar a função para mudar a cor do material e uma função para rodar o cristal. 

Ainda não está completo, quando todos os cores da nave principal são destruídos, a nave principal é destruída também. Mas isso vai ficar para uma implementação futura. 

Corrigi mais alguns problemas na AI, como elas deslizavam passando pelo alvo, precisei criar mais um node, para deixar que elas sempre fiquem "olhando" para o alvo em que estão perseguindo, em vez de ficarem mirando no vácuo. 


Segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/Q1FtHoHSViM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>
