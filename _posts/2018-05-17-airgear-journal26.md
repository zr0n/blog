---
layout: post
title: Diário GameDev - AirGear Dia 26

---

Olá amigos, como estão? Como vocês sabem, todo dia eu to postando como foi o dia de desenvolvimento do jogo AirGear e falando um pouco sobre o que eu fiz.

Hoje resolvemos fazer a ultimate da dupla Vall’hart e Natasha. Que é:

R – Vortex: Vall’hart utiliza seu dispositivo de absorção de massa para criar um vortex que irá atrair todos os aviões inimigos dentro do alcance para o seu centro por 6 segundos, simultaneamente, ele ganha um escudo de 400 de hp durante todo o período da skill, enquanto ela estiver conjurada, ele nega danos de impacto e causa 250 de dano ao colidir com os inimigos. Cooldown 50 segundos.

Foi bem divertido desenvolver isso. Criei um sistema para gerar uma órbita no centro do Vortex, atraindo os aviões para o centro. Um dos desafios de fazer isso foi o fato de não simular física da engine nos aviões. Mas usando as opções de força do CharacterMovement foi bem fácil obter esse resultado no final. O vortex é regulável, como ainda estamos testando valor, não dá pra definir um comportamento adequado para ele a priori. No vídeo eu tentei explorar bastante, comecei com um vortex com bastante força, depois coloquei um bem fraco, onde o personagem inclusive conseguia sair da órbita dele e por último uma força moderada, onde o personagem não era atraído para o centro se estivesse fazendo força contra, mas também não conseguia sair da órbita.

Enfim, segue o vídeo de como ficou:

<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/Kc03olfPbjA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<p class= "message"> - Luiz Fernando </p>