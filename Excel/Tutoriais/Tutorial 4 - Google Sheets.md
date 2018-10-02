# Alternativas ao Excel

Tópicos a serem abordados

* Google Sheets

* Importando .csv

* Usando funções no Google Sheets

* Criando uma tabela dinâmica no Google Sheets

* Criando um gráfico a partir dos dados

* Função FREQUÊNCIA

## Google Sheets

O Google Sheets é uma ferramenta muito poderosa e, o melhor de tudo, grátis!

Ela pode ser acessada pelo navegador, editada por múltiplos usuários e os seus arquivos ficam salvos na nuvem, podendo ser acessados por qualquer computador, através da sua conta do Google.

### Acessando o Google Sheets

* Acesse [o site do Google Sheets](https://www.google.com/sheets/about/), logue com sua conta do Google.

* Crie uma nova planilha em branco

### Importando .csv

* Faça o download do arquivo ["Instituições Credenciadas - Abr/2018"](http://dados.prefeitura.sp.gov.br/dataset/organizacoes-credenciadas-para-atendimento-da-educacao-infantil)

* Clique em Arquivo > Importar > Upload 

* Arraste o arquivo osccredenciamentoabr18.csv da pasta de downloads para a janela do Google Sheets

* Aguarda a realização do upload

* Selecione **Inserir novas páginas**

* Selecione **Personalizado** e insira um ponto e vírgula na caixa

* Clique em **Importar dados**

* Aguarde a finalização da importação e clique em **"Abrir agora"**, caso sua planilha não apareça automaticamente.

![importando](../Gifs/GSheets/importa.gif)

### Usando funções no Google Sheets

Agora que temos nossos dados importados no Google Sheets, começaremos a operar sobre eles.

Vamos analisar quais são os bairros com organizações credenciadas e quantas são essas organizações.

#### Criando uma tabela dinâmica no Google Sheets

* Na aba superior, clique em Dados > Tabela Dinâmica

* No Menu da direita, na seção "Linhas", clique em ADICIONAR e, no menu, escolha Bairro

* Na seção "Valores", clique em ADICIONAR e selecione Bairro

* Na seção "FILTROS", clique em ADICIONAR, selecione "Status Credenciamento"

* Clique em "Mostrando todos os itens", desselecione "DESCREDENCIADA" e clique OK

![PivotTables](../Gifs/GSheets/Ptable.gif)

* De volta à seção "Linhas", em Ordem, selecione Decrescente

* Em classificar por, selecione COUNTA de Bairro

* Feche o menu da direita, clicando no "X"

![ordena](../Gifs/GSheets/ordena.gif)

O que obtivemos é uma nova tabela, em que os bairros aparecem em ordem alfabética e, ao lado, quantas organizações credenciadas estão presentes em cada um deles.

### Criando um gráfico a partir dos dados

Criaremos um gráfico, mostrando quais bairros têm, pelo menos, 10 organizações cadastradas ou mais .

* Clique sobre a célula A1 e, sem soltar o clique, arraste até a célula B11.

* Clique em Inserir > Gráfico

* Em "Tipo de gráfico", selecione Gráfico de colunas

* Clique na caixa "Alternar linhas/colunas"

* Assim, obteremos um gráfico com os bairros que têm mais de 10 organizações cadastradas e suas quantidades correspondentes

![tenPlus](../Gifs/GSheets/Graph.gif)


### Verificando distribuição de organizações por bairros

E se quiséssemos saber quantos bairros têm uma instituição cadastrada, quantos têm duas e assim por diante?

Primeiro, calcularemos as frequências:

* Crie uma coluna "Quantidade de organizações"

* Preencha suas linhas com valores de 1 até 6

* Na linha de número 8 escreva 7 ou mais

![ranges](../Gifs/GSheets/Range.gif)

Repare que o texto "7 ou mais" ficou alinhado à esquerda, vamos arrumar isso:

* Clique sobre a célula **C8**

* Clique na opção Formatar > Alinhar > Direita

Pronto, agora todos os valores estão alinhados!

![alinhar](../Gifs/GSheets/alinhar.gif)

Agora, criaremos a coluna "Quantidade de bairros", na coluna D. Nessa coluna, colocaremos quantos bairros têm exatamente a quantidade de organizações listadas à esquerda. Para isso, usaremos a função **FREQUÊNCIA**.

#### FREQUÊNCIA

A função frequência recebe dois argumentos, um vetor com dados e os intervalos com os quais iremos separar esses dados.


	=FREQÜÊNCIA(matriz_dados; matriz_bin)
	=FREQÜÊNCIA(dados; intervalos)

Nós já temos esses dois argumentos! A matriz_dados é nossa coluna B, e os intervalos são nossa coluna C, que criamos anteriormente!

* Clique sobre a célula D2, digite =Frequency e selecione a função frequency

* Selecione a coluna B em sua totalidade, clicando sobre o B. Esse é nosso vetor de dados

* Digite ponto e vírgula, indicando o fim do primeiro argumento

* Selecione agora os números de 1 a 6 na Coluna C. Esses são os nossos intervalos.

* Não selecionamos 7 ou mais. Automaticamente, a função frequência vai colocar os valores acima do nosso intervalo na célula seguinte.

![frequencia](../Gifs/GSheets/frequencia.gif)

### Plotando um novo gráfico

Vamos agora criar um novo gráfico, a partir das novas informações coletadas.

* Selecione as células de D2 a D8

* Clique em Inserir > Gráfico

* Selecione "Gráfico de "

* Clique em marcador e escolha as células de C2 a C8 

Pronto! Agora, temos um gráfico que mostra a distribuição do número de organizações cadastradas por bairro: quantos bairros têm uma organização cadastrada, quantos têm dois e assim por diante.

![pieC](../Gifs/GSheets/pieC.gif)
