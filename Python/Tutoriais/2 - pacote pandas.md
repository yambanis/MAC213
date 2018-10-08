# Bibliotecas

Bibliotecas(ou _libraries_) são conjuntos de rotinas que poderemos utilizar em nosso programa. O python já vem com algumas por padrão, por exemplo o print que utilizamos no exemplo anterior, mas podemos ainda importar outras bibliotecas diferentes.

## Pacote Pandas

O pandas ou [Python Data Analysis Library](https://pandas.pydata.org/) e uma biblioteca muito util, que irá nos fornecer diversas ferramentas para análise de dados.

Para utiliza-la, escrevemos no início do nosso código no Google Colab:

	import pandas as pd

Clicamos em _play_ para realizar a importação da biblioteca.

O comando import realiza a importação enquanto o _as_ da um "apelido" para a nossa biblioteca, para que não tenhamos que escrever seu nome inteiro no nosso código.

Nesse caso, importamos a biblioteca pandas e iremos nos referenciar a ela com _pd_ em nosso código.

## Lendo CSV com pandas

Primeiramente vamos baixar um arquivo csv para utilizarmos.
Entre na [pagina de dados abertos prefeitura](http://dados.prefeitura.sp.gov.br/pt_PT/dataset/rendimento-e-movimento-escolar-ensino-fundamental) e faca o download do arquivo _Rendimento e Movimento Escolar - 2000 a 2015_ clicando em Explorar->Transferir.

Agora precisamos realizar o upload do arquivo para o ambiente do Colab.
Para isso, vamos utilizar o seguinte comando:

	from google.colab import files
	uploaded = files.upload()

Apos clicar no _play_, clique em _Choose Files_, selecione o arquivo censoevolutivomovimentorendimento.csv e espere o termino do upload.

Agora, vamos realizar a leitura desse arquivo CSV com o comando pd.read_csv

Para tal, vamos criar uma variavel csv e salvar a leitura nela:

	csv = pd.read_csv(uploaded("censoevolutivomovimentorendimento.csv"), index_col=0, parse_dates=True)