---
title: HackerRank - Melhorando como Programador
date: 2017-02-11 15:29:00 Z
categories:
- dicas
tags:
- sample post
excerpt: Uma dica legal.
comments: true
layout: post
---

**Introdução**
===========

E ae galera, mais um post estou tendo uma dificuldade enorme em escrever esses posts aqui, falta de motivação e outras coisinhas a mais, por isso eu só vou escrever quando realmente o assunto for muito do meu interesse e o assunto de hoje é o **hackerrank**, quero passar um overview da plataforma e algumas dicas, acredito que alguns já conheçam até porque é bem conhecida e vamos lá então, lembre no final de deixar um comentário. Thank's

**Singup na plataforma super simplificado**
====================================

Como podemos ver é bastante fácil ter uma conta no hackerrank, você pode conectar 498498498 de contas, facebook, google, likedin, github. E se essas opções não forem suficiente você pode escolher o seu melhor e-mail e se cadastrar. Sem desculpas façam seus cadastros.

![](https://camo.githubusercontent.com/10adb88b5de116cdf7ff1b21cdcf630bacef2fad/68747470733a2f2f7777772e657665726e6f74652e636f6d2f73686172642f733434332f73682f34363032653332352d383463332d343131392d396533642d3139333566333864616466322f38666232353966373130396661646165383932393864383665303439303638652f7265732f61626438636230632d623135652d343835662d396161642d3462323637386466613063312f53656d2532307425433325414474756c6f2e706e673f726573697a65536d616c6c2677696474683d383332)

**Exercícios de todos os tipos e linguagens**
====================================

Isso mesmo aqui você vai encontrar exercícios divididos por linguagens como ruby, phyton, java, c++ e também por skills especializados como inteligência artificial, sql, databases, etc. Tem desafios para todos os gostos aqui. o/

![](https://camo.githubusercontent.com/3fcc451ee872867768171be512456fe940051ea7/68747470733a2f2f7777772e657665726e6f74652e636f6d2f73686172642f733434332f73682f34363032653332352d383463332d343131392d396533642d3139333566333864616466322f38666232353966373130396661646165383932393864383665303439303638652f7265732f61306233356332662d353063372d343535362d613566662d3762376532373637393764302f53656d2532307425433325414474756c6f2e706e673f726573697a65536d616c6c2677696474683d383332)

Os mesmos são divididos em subcategorias como introdução(alias é bom prestar atenção nessa parte pois é bem importante vou falar mais adiante), strings, entre outros vários.

E dentro dos exercícios você vai ter as abas problem, submissions, leaderboard e discussions.

- Problem como o próprio nome já diz é onde o problema sera descrito.
- Submissions são os códigos que você submeteu para resolver o problema.
- Leaderboard é um rank com alguns monstros das soluções que vão das mais eficientes até as menos
- Discussions essa é uma parte muito interessante onde os usuários podem postar suas dúvidas em relação ao problema aconselho você a explorar bastante essa aba.

**Algumas dicas**
==============

Considero essas dicas que vou passar muito importantes pois estou na plataforma a alguns meses e algumas delas eu so percebi a pouco tempo(ontem), perdi bastante tempo por não as conhecer mas vamos lá, sempre tem algo novo a aprender isso é ótimo.

**#1**

Aba leaderboard - caso você esteja em um problema a muito(muito muito) tempo, e já fez de tudo utilizou o discussions e procurou no google. Tem uma coisa legal que você pode fazer na aba leaderboard que é ver o código de outros participantes isso mesmo haha, ver o código dos asiáticos e afins, o único onus disso é que suas submissões nessa questão não vão mais valer pontos ;/, as vezes é bom você vai aprender com as soluções.

Clica na area verde:
![](https://camo.githubusercontent.com/39028b2830c37e00107d0e882c9c8388968f1733/68747470733a2f2f7777772e657665726e6f74652e636f6d2f73686172642f733434332f73682f34363032653332352d383463332d343131392d396533642d3139333566333864616466322f38666232353966373130396661646165383932393864383665303439303638652f7265732f31333061373130652d323662662d343866622d383136642d3337633966386165333966642f53656d2532307425433325414474756c6f2e706e673f726573697a65536d616c6c2677696474683d383332)

Depois clica na area verde de novo e você será capaz de ver o código:
![](https://camo.githubusercontent.com/496960811aaa8bfc89d86276b7e0031240e8f03e/68747470733a2f2f7777772e657665726e6f74652e636f6d2f73686172642f733434332f73682f34363032653332352d383463332d343131392d396533642d3139333566333864616466322f38666232353966373130396661646165383932393864383665303439303638652f7265732f34343739363666652d646263312d346338662d393333342d3031666665613162393162632f53656d2532307425433325414474756c6f2e706e673f726573697a65536d616c6c2677696474683d383332)

**Extra:**

As vezes o código vai abrir no [codepair](https://codepair.hackerrank.com/paper/AuoTik5I?b=eyJyb2xlIjoiY2FuZGlkYXRlIiwibmFtZSI6IlZhbHRlckJhcnJvcyIsImVtYWlsIjoidmFsdGVyaW5zaWRlQGdtYWlsLmNvbSJ9) que é um editor online do hackerrank um projeto a parte(vale a pena pesquisar sobre depois) se o código for muito grande vai abrir em uma pagina em branco.

**#2**

O próprio **hackerrank** vai te prover os inputs - essa aqui eu sofri bastante para descobrir, no exemplo podemos ver que através do objeto `scanner` os inputs serão recebidos, agora você tem a oportunidade de chegar na plataforma em certa vantagem com essa dica.

{% highlight java %}
     import java.util.*;

     public class Solution {

          public static void main(String[] args) {
          Scanner scan = new Scanner(System.in);
          int a = scan.nextInt(); //
          // Complete this line
         // Complete this line

        System.out.println(a);
        // Complete this line
       // Complete this line
  }
}
{% endhighlight %}

**Conclusão**
===========

Nós programadores trabalhamos resolvendo problemas todos os dias, e quanto mais prática tivermos melhor, a prática leva a perfeição se você se dedicar, as questões vão ficando mais fáceis pois você vai ter como uma biblioteca de soluções em seu cérebro, ao mesmo tempo que o seu trabalho de programador também vai, com soluções mais rápidas para diversos problemas.

Se uma questão parece complicada tente por um tempo depois vá para outra, e é isso espero que tenha gostado até a próxima.

That's it
