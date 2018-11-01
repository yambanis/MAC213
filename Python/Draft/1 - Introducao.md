# Introdução ao Python para análise de dados

Neste tutorial, iremos cobrir conceitos básicos de python e alguns de seus pacotes úteis para análise de dados.

## O que é Python?

[Python](https://www.python.org/) e uma das linguagens de programacao mais utilizadas atualmente. Ele e conhecida por ser de fácil legibilidade.

Este tutorial não tem por objetivo ser um curso completo de Python. Iremos utilizá-la apenas como uma ferramenta para analisarmos dados e vamos cobrir apenas aspectos que forem se mostrando necessários.

Existem muitos [materiais](https://www.python.org/about/gettingstarted/) [excelentes](https://www.codecademy.com/learn/learn-python) [na internet](https://www.tutorialspoint.com/python/) e, se voce se interessar mais por Python, recomendamos que consulte algum deles. 

## Ambiente de programação

Existem várias formas de programar em Python. Voce pode [baixa-lo](https://www.python.org/downloads/) em seu computador e, usando seu editor de textos favoritos ou diretamente no terminal, roda-lo de forma local.

Existe tambem a ferramenta online [notebook](https://colab.research.google.com/), que permite que criemos um ambiente virtual, onde iremos rodar o Python nas máquinas do Google.

Além disso, o colab permite controle de versões e que seja mais fácil compartilhar nosso código entre computadores.

## Anaconda

Uma maneira pratica e poderosa de programar em Python e utilizado o pacote Anaconda. Voce pode [baixa-lo aqui](https://www.anaconda.com/download/)

Siga as intrucoes de instalacao. Iremos utilizar o modulo Jupyter Notebook. Ele e automaticante instalado junto com o Anaconda.

Voce pode tambem acessar um versao online do jupyter notebbok [neste link](https://mybinder.org/v2/gh/yambanis/MAC213/master)

## Variáveis

Programar em Python pode ser bastante simples.

Vamos começar declarando uma variável.

[Variaveis](https://pt.wikipedia.org/wiki/Vari%C3%A1vel_(programa%C3%A7%C3%A3o)) e um nome que, em computacao, se refere a um local onde iremos guardar informações.

Usando algumas informacoes que coletamos [neste tutorial](https://github.com/yambanis/MAC213/blob/master/Excel/Tutoriais/Tutorial%202%20-%20Funcoes.md), vamos criar uma variavel para guardar o numero de matriculados no distrito de AGUA RASA.

Escreva o seguinte no notebook:

	aguaRasa

Pronto! Sua variável já está criada! Simples não?

Mas nossa variável aguaRasa ainda não possui nenhuma informação dentro dela. Para isso guardar o dado em uma variável, usamos o comando de [atribuicao](https://pt.wikipedia.org/wiki/Atribui%C3%A7%C3%A3o_(computa%C3%A7%C3%A3o)), usando o símbolo de igual.

	aguaRasa = 5578

Dessa forma, nossa variável aguaRasa agora guarda dentro de si o valor 5578.

## Funções

Utilizando [funções](https://www.cs.utah.edu/~germain/PPS/Topics/functions.html) somos capazes de realizar tarefas que alguém já programou previamente, sem saber como elas funcionam!

Vamos agora imprimir(mostrar na tela) o valor que guardamos na nossa variável aguaRasa. Muitas coisas estão envolvidas neste processo, como acesso à memória, controle de entrada e saída, mas utilizando a função **print()** não é necessário que saibamos fazer nenhuma dessas coisas. Basta escrever:

	print(aguaRasa)

Clique no _play_ do notebook e o valor da variável aguaRasa irá aparecer na tela.

Geralmente as funções tem um nome e argumentos que elas recebem. Neste caso, o nome da nossa função é _print_ e o argumento, ou o que ela recebe dentro dos seus parênteses, e o que desejamos imprimir, nesse caso a variável aguaRasa.

Se quisermos imprimir a palavra Agua Rasa ao invés da variável, basta escrevermos o que desejamos imprimir entre parênteses:

	print("Numero de matriculados no distrito de Agua rasa:")

Dessa forma, será impresso exatamente aquilo que escrevemos entre parênteses.

## Operações simples 

Para realizarmos operações simples em Python, basta escrevê-las de forma bastante intuitiva.

Vamos Realizar a soma dos valores dos distritos de AGUA RASA, ALTO DE PINHEIROS E ANHANGUERA.

Vamos, primeiro armazenar esses dados em 3 variáveis:

	aRasa = 5578
	aPinheiros = 434
	anhanguera = 8813

Agora vamos criar uma variável total que será a soma das três. Basta escrever:

	total = aRasa + aPinheiros + anhanguera

Finalmente, vamos imprimir esse valor na tela:

	print(total)

Aperte o _play_ da célula do notebook para visualizar o resultado.

Para realizar outras operações matemáticas elementares, como subtracao, multiplicacao e divisao, basta escrever de modo natural, assim como fizemos para a soma.
