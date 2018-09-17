# Fórmulas

Agora que já temos nossos dados importados, vamos começar a extrair informações deles.

Lembre-se que na [pagina](http://dados.prefeitura.sp.gov.br/dataset/perfil-dos-educandos-cor-raca-idade-sexo-necessidades-educacionais-especiais) que fizemos o download do CSV, temos o arquivo "Dicionario" que sera importante para "traduzirmos" as siglas presentes no nosso CSV.

Tópicos a serem abordados:

* Introdução a funções

* Função SOMA

* Funcao CONT.SE

* Função SE

* Função SOMASE

## Introdução a funções

As funções no excel são uma das maneiras mais simples de automatizar os processos, o que e muito útil, desde quando estamos tratando pequenos conjuntos de valores até tabelas bastante grandes.

## Introduzindo valores
Para introduzir um valor no excel, basta clicar na célula em questão e digitar o valor que quisermos. Aqui, usamos o termo valor de forma genérica: Pode ser uma quantia em dinheiro, uma data, um nome. O excel é capaz de tratar todos estes tipos de dados. Vamos ver como informar o que está na célula do excel mais a frente.

![Valores](../Gifs/Funcoes/Valores.gif)


## Introduzindo funções
Para introduzir funções, fazemos de maneira similar aos valores: clicamos na célula que queremos alterar e digitamos o que desejamos inserir. Entretanto, para avaliarmos ao excel que queremos que aquilo seja avaliado como uma função ao invés de um valor, basta colocarmos um símbolo de **=** no começo do que estamos digitando.

Uma vantagem de escrever assim, o excel imediatamente reconhece que estamos escrevendo uma fórmula e mostra uma série de opções assim que começamos a escrever o nome da função.

![Funcao](../Gifs/Funcoes/Funcao.gif)

## Barra de Fórmulas

Além de escrever diretamente nas células, umas ferramenta muito prática e a barra de fórmulas. Nela, podemos escrever ou editar o conteúdo das células.

Para isso, basta selecionar a célula que queremos editar, clicando sobre ela e, então, digitar os valores ou fórmulas que desejamos inserir diretamente na barra de fórmulas.

Escrever sobre a célula ou na barra de fórmula são equivalentes, tudo depende da ação que estamos realizando.

![formulaBar](../Gifs/Funcoes/formulaBar.gif)

## Fórmulas básicas

Podemos fazer operações básicas no excel usando os operadores conhecidos da matemática: +, -, * e /.
No excel nos referenciamos a células pela letra de sua coluna seguida pelo número de sua linha.
Assim, podemos selecionar uma célula para guardar o resultado da operação entre outras células.

1. Para somar, escolha uma célula para guardar o resultado e digite, =C1+C2, por exemplo, e pressione ENTER
2. Para subtrair, escolha uma célula para guardar o resultado e digite, =C1-C2, por exemplo, e pressione ENTER
3. Para multiplicar, escolha uma célula para guardar o resultado e digite, =C1*C2, por exemplo, e pressione ENTER
4. Para dividir, escolha uma célula para guardar o resultado e digite, =C1/C2, por exemplo, e pressione ENTER

![formulaBasicas](../Gifs/Funcoes/formulasbsc.gif)

## Algumas funções úteis

### Função SOMA
Esta é uma das funções mais básicas e úteis do excel.

Vamos supor que queremos calcular o total de vendas de uma empresa. Para calcular o total de produtos vendidos,
vamos usar a função soma.

* Vamos clicar na célula que queremos guardar o valor da soma.
* Vamos digitar =SOMA e clicar sobre a opção SOMA.
* Vamos então clicar sobre a célula contendo o primeiro item a ser somado e, sem soltar, arrastar até o último item da lista a ser somado.
* Finalmente vamos clicar ENTER e visualizar o valor total da soma

![soma](../Gifs/Funcoes/soma.gif)

### Combinando funções
Vamos supor agora que nossos produtos têm valores distintos, vamos ver a renda total das vendas.
Primeiramente, precisamos multiplicar a coluna com os preços unitários pelas quantidades

* Selecionamos a célula B2 e multiplicamos pela célula C2

![mult](../Gifs/Funcoes/mult.gif)

Precisamos fazer os mesmo para as células de baixo, mas não precisamos reescrever a fórmula!
Basta clicar no canto inferior da célula com a fórmula que desejamos copiar e arrastar para as células de destino. Dessa forma, o excel aplica a mesma fórmula de maneira automática.

Podemos fazer o mesmo para copiar as fórmulas de soma que escrevemos anteriormente

![copiaFunc](../Gifs/Funcoes/copiaFunc.gif)


### Funcao CONT.SE
Vamos agora começar algumas análises simples dos dados que importamos, utilizando algumas funções do excel

A funcao CONT.SE e bastante útil e pode nos informar o número de células que atendem a algum critério. Vamos supor como exemplo que desejamos contar quantos alunos são do sexo masculino e quantos são do sexo feminino. Temos um numero enorme de dados, mas essa analise fica muito simples com a funcao CONT.SE

Primeiramente, vamos criar uma nova planilha, para organizarmos nossas análises. Vamos clicar no botão +, localizado na parte inferior da nossa tela.

Uma nova aba vai se abrir. Podemos clicar duas vezes sobre ela para renomeá-la. Vamos chamá-la de análises.

![NewSheet](../Gifs/Funcoes/NewSheet.gif)

Agora nessa nova planilha, vamos usar a funcao CONT.SE para verificar a distribuicao de alunos do sexo masculino e feminino.

* Selecionamos uma célula e digitar o símbolo de =
* Digitamos CONT.SE. Perceba que o excel começa a mostrar opções conforme você digita, não sendo necessário digitar o comando inteiro.
* Clique duas vezes sobre o nome CONT.SE para inserir a formula na celula.

![InsertForm](../Gifs/Funcoes/insertForm.gif)

Conforme aparece na tela, o comando CONT.SE leva dois argumentos:

	=CONT.SE(intervalo; critérios)
	=CONT.SE(Onde você quer procurar?; O que você quer procurar?)
 
Queremos procurar quantos alunos do sexo feminino estão presentes na coluna P da planilha "idadeserieneeracadez17". Então vamos entrar esses dois argumentos na nossa fórmula.

Depois de inserir a CONT.SE na celula, vamos agora selecionar os argumentos.

Primeiro vamos selecionar as células que nos interessam. Neste caso, as informações sobre o sexo dos estudantes estão na coluna P. Queremos selecionar a coluna P em sua totalidade. 

* Vamos clicar na planilha "idadeserieneeracadez17" e clicar sobre o "P" que marca o nome da coluna.

Automaticamente, a fórmula que estamos criando, que está escrita na barra de fórmula já foi preenchida com o argumento "idadeserieneeracadez17!P:P" que indica que vamos analisar a coluna P da planilha "idadeserieneeracadez17" em sua totalidade.

Agora precisamos preencher o segundo argumento da função, que nesse caso é o que queremos contar. 

* Clicamos na barra de fórmulas e adicionamos um ponto e vírgula - ;

O ; indica que vamos agora inserir o próximo argumento. Neste caso, queremos contar o número de meninas.

* Inserimos "F", a letra F entre aspas, assim o excel irá contar todas as ocorrências da letra F na coluna P.

* Colocamos então um fecha parênteses - ) - no fim da fórmula e damos enter.


![ArgsContSe](../Gifs/Funcoes/argsContse.gif)

Agora, na nossa planilha "Análises", temos na célula escolhida um valor, 175986, que representa o número de entradas F na coluna P.

Assim, conseguimos obter esse valor de forma muito prática, mesmo o conjunto de dados contendo mais de 300 mil entradas.

Para obter o número de alunos do sexo masculino, a operação é muito similar, basta trocarmos o segundo argumento da CONT.SE de "F" para "M":

![masculinos](../Gifs/Funcoes/masc.gif)

Agora temos o total de meninas e meninos. Para obter o total de estudante, basta somarmos, escrevendo em uma nova célula =A1+A2

![total](../Gifs/Funcoes/tot.gif)

Agora sabemos que o total de estudantes e 346861, sendo 175986 meninas e 170875 meninos. 

Podemos utilizar o CONT.SE para extrair muitas outras informações, como total de alunos por período, ocorrência de raça

### FUNÇÃO SE

A função SE permite que criemos uma condição para que alguma tarefa seja realizada.

Com o COUNT.SE fomos capazes de contar quantas vezes ocorreu um certo valor nos nossos dados, mas e se quisermos, além de ver a ocorrência de grupos femininos e masculinos, saber a quantidade total de alunos de cada sexo, multiplicando pela coluna QTD?

Vamos usar a função **SE**

* Escolha uma célula de destino e digite =SE e clique sobre a função duas vezes

A função SE recebe três argumentos:

	=SE(Teste lógico, valor verdadeiro, valor falso)	
	=SE(Algo for Verdadeiro, faça tal coisa, caso contrário, faça outra coisa)

Entao podemos escrever a funcao como:

	=SE(CELULASEXO = "F", QTD, 0)

Dessa forma, se a célula em questão for igual a F, recuperamos o valor QTD associado a. Se nao, nao contamos ela.

![if](../Gifs/Funcoes/IF.gif)

### FUNÇÃO SOMASE

Mas a função SE ainda não é suficiente para descobrirmos o valor total de alunos de cada sexo. Utilizando a função SOMASE, finalmente conseguimos este resultado.

A função SOMASE recebe três argumentos:

	=SOMASE(intervalo, critérios, intervalo_soma)

O argumento intervalo e o intervalo a ser avaliado, segundo o critério no segundo argumento.
O argumento intervalo_soma é opcional: Se o próprio intervalo a ser somado e o mesmo sendo avaliado, deixamos esse argumento em branco. Se não, colocamos o intervalo correspondente a ser somado.

* Escolha uma célula e entre a função =SOMASE clicando duas vezes sobre seu nome

* Escolha a coluna P em sua totalidade. Este é nosso intervalo a ser avaliado.

* Na barra de fórmulas, entre '; "F"', este é o nosso critério de soma

* finalmente, adicione mais um ; e selecione a coluna T, para selecionar as quantidades. Esse é nosso intervalo de soma.

* Adicione um fecha parentes ) e clique enter para visualizar o valor encontrado

* Faremos o mesmo para obter o número de meninos, apenas trocando o "F" por "M"

![SomaSe](../Gifs/Funcoes/somase.gif)





