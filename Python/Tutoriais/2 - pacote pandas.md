# Bibliotecas

Bibliotecas(ou _libraries_) são conjuntos de rotinas que poderemos utilizar em nosso programa. O python já vem com algumas por padrão, por exemplo o print que utilizamos no exemplo anterior, mas podemos ainda importar outras bibliotecas diferentes.

## Pacote Pandas

O pandas ou [Python Data Analysis Library](https://pandas.pydata.org/) e uma biblioteca muito util, que irá nos fornecer diversas ferramentas para análise de dados.

Para utiliza-la, escrevemos no início do nosso código no notebook:

	import pandas as pd

Clicamos em _play_ para realizar a importação da biblioteca.

O comando import realiza a importação enquanto o _as_ da um "apelido" para a nossa biblioteca, para que não tenhamos que escrever seu nome inteiro no nosso código.

Nesse caso, importamos a biblioteca pandas e iremos nos referenciar a ela com _pd_ em nosso código.

## Lendo CSV com pandas

Primeiramente vamos baixar um arquivo csv para utilizarmos.
Entre na [pagina de dados abertos prefeitura](http://dados.prefeitura.sp.gov.br/pt_PT/dataset/rendimento-e-movimento-escolar-ensino-fundamental) e faca o download do arquivo _Rendimento e Movimento Escolar - 2000 a 2015_ clicando em Explorar->Transferir.


Agora, vamos realizar a leitura desse arquivo CSV com o comando pd.read_csv.

Coloque o arquivo na mesma pasta do seu notebook.

Para tal, vamos criar uma variavel df e salvar a leitura nela:

	df = pd.read_csv('idadeserieneeracadez17.csv' , 
		   sep = ";", encoding = 'latin-1', header = 0)

Atraves desse comando, a nossa variavel df ira ler e armazenar o arquivo csv. O argumento sep indica que o ponto e virgula e o elemento de separacao do nosso csv, em enconding utilizamos latin-1 para indicar a codificacao de simbolos utilizados no portuges, como cedilha e indicamos o header igual a zero, mostrando que a informacao do header de cada coluna esta na linha 0.

Se digitarmos:

	type(df)

sera possivel constatar que df e uma variavel do tipo pandas.core.frame.DataFrame.

O [DataFrame](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html) e uma estrutura tabular do Pandas, que possui diversas funcoes ja implementadas. Nossa tabela(ou csv) esta guardada dentro dela e iremos manipula-la para extair as informacoes que desejamos.

## Analise de dados utilizando DataFrame


