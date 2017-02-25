---
title: Javascript Hoisting
date: 2016-12-23 14:01:43 Z
categories:
- front-end
tags:
- sample post
layout: post
excerpt: Javascript e suas variáveis.
comments: true
---

Antes algumas informações
=========================

Parece ser uma informação básica porem podemos nos surpreender com a quantidade de desenvolvedores javascript que podem se perder nesse conceito, por pensar que por javascript ser parecido com java (alias ela herda algumas coisas realmente), é a mesma linguagem porem não é e possui sua particularidades, com alguns exemplos de código poderemos entender.

dito isso vamos lá então...
===========================

Temos o seguinte código que é uma declaração normal e vai funcionar perfeitamente, perceba que estou declarando e inicializando a variável `nome` para so depois chamar a mesma.

{% highlight javascript %}
	var nome = "Valter";
	console.log(nome);
{% endhighlight %}

Mas e se quisermos fazer isso... Não vai funcionar horas como eu quero chamar uma variável que inda não existe?

{% highlight javascript %}
	var nome = meuNome;
	console.log(nome);
	// ReferenceError: meunome is not defined
{% endhighlight %}

Mas e agora dessa forma... Não recebemos mais um erro agora nosso valor é **undefined**, entenda que a variável já existe mesmo antes de ela ter sido declarada no código isso acontece pois o javascript sobe as declarações (sem a inicialização) para o topo do código e o mesmo acontece com funções por definição.

{% highlight javascript %}
	var nome = meuNome;
	console.log(nome);
	var meuNome;
	//undefined
{% endhighlight %}

Isso acontece pelo mesmo motivo anterior a declaração foi arrancada para o topo porem sem a inicialização por isso temos o erro.

{% highlight javascript %}
	console.log( multiplicaNumero(10,20) );
	var multiplicaNumero = function(n1,n2){
    return n1 * n2
	};

	//TypeError: undefined is not a function
{% endhighlight %}

Dessa forma vai funcionar normalmente pois toda declaração de função não anônima é elevada para o topo do escopo.

{% highlight javascript %}
	console.log(multiplicaNumero(10,10));
	function multiplicaNumero (a,b) {
	  return a*b;
	}
	// 100
{% endhighlight %}

Por isso é uma boa prática declarar ou iniciar variáveis no inicio do escopo.

That's it.
