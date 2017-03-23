---
title: Galeria de imagens com Display:flex
date: 2016-12-23 14:01:43 Z
categories:
- front-end
tags:
- sample post
layout: post
excerpt: Uma dica legal.
comments: true
---

Introdução
===========================
O valor **flex** para a propriedade **display** é algo bastante útil no front-end, para saber quais navegadores e versões são compatíveis você pode checar no [caniuse](http://caniuse.com/#search=flex), assim que conheci já comecei a user em meus projetos ele consegue
tornar o posicionamento de conteúdos na página bem mais simples, atividade essa temida por alguns devs haha (eu),
isso quando temos que utilizar position, float ou até mesmo frameworks como bootstrap. Conheci a propriedade em um curso do [codecademy](https://www.codecademy.com)
e me aprofundei no site [css-tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

Explicando o básico sobre a propriedade display:flex
====================================================

`display:flex` Além de várias outras coisas ele serve para alinhar os filhos de um elemento horizontalmente.

![display flex exemplo image](/assets/img/display-flex.png)

Para que esses elementos não fiquem na mesma linha que no caso é o comportamento padrão deles você deve usar `flex-wrap:wrap`.

![flex-wrap exemplo image](/assets/img/flex-wrap.png)

Já no caso de você querer centralizar o conteúdo após utilizar as propriedades acima você precisa usar `justify-content:center`

![flex-wrap exemplo image](/assets/img/justify-content.png)

Práticando com display:flex
=============================

Primeiro criamos uma **.galeria** vamos alinhar os **.galeria-item** por ele.

{% highlight html %}
  <div class="galeria">
    <figure class="galeria-item">
      <img src="http://cdn2.knowyourmobile.com/sites/knowyourmobilecom/files/2016/10/the-last-of-us1.jpg">
    </figure>
      
    <figure class="galeria-item">
      <img src="https://images5.alphacoders.com/338/338417.jpg">
    </figure>

    <figure class="galeria-item">
      <img src="http://media.gamerevolution.com/images/galleries/1337/the-last-of-us-1.jpg">
    </figure>

    <figure class="galeria-item">
      <img src="https://jovemnerd.com.br/wp-content/uploads/The-Last-of-Us-2-concept-art.jpg">
    </figure>
  </div>  
{% endhighlight %}

E aqui está a mágica que vai alinhar, centralizar e garantir que tudo não fique em apenas uma linha.

{% highlight css%}
  .galeria{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
{% endhighlight %}

Agora nossos elementos já devem estar alinhados com seu respectivo pai, como eu peguei imagens da internet vou precisar definir tamanhos fixos e utilizar a propriedade `object-fit:cover` para que as imagens não percam seu aspecto.

{% highlight css %}
  .galeria img{
    width:  500px;
    height: 500px;
    object-fit: cover;
  }
{% endhighlight %}

Podemos definir uma margem entre as imagens...

{% highlight css %}
  .galeria-item{
    margin: 20px;
  }
{% endhighlight %}

Resultado final:
===========================
![thelastofus]({%site.url%}/assets/img/galery-tlou.png)

Então, meu primeiro post aqui no blog, estou adorando o **jekyll** que é a plataforma que estou utilizando, bastante simples e funcional. Espero poder ajudar outros devs compartilhando conhecimento por aqui e dessa forma também aprender, se chegou até aqui obrigado ;D.

![Por hoje é só. Até a próxima pessoal!](/assets/img/he-man-frase.jpg)
