# Alternativas ao Excel

## Google Sheets

O Google Sheets e uma ferramente muito poderosa e, o melhor de tudo, gratis!

Ela pode ser acessada pelo navegador, editada por multiplos usuarios e os seus arquivos ficam salvos na nuvem e podem ser acessados por qualquer computador, atraves da sua conta do google.

### Acessando o Google Sheets

* Acesse [o site do google sheets](https://www.google.com/sheets/about/), logue com sua conta do google.

* Crie uma nova planilha em branco

### Importando nosso .csv

* Faca o download do arquivo ["Instituições Credenciadas - Abr/2018"](http://dados.prefeitura.sp.gov.br/dataset/organizacoes-credenciadas-para-atendimento-da-educacao-infantil)

* Clique em Arquivo > Importar > Upload 

* Arraste o arquivo osccredenciamentoabr18.csv da pasta de downloads para a janela do Google sheets

* Aguarda a realizacao do upload

* Selecione **Inserir novas paginas**

* Selecione **Personalizado** e insira um ponto e virgula ; na caixa

* Clique em **Importar dados**

* Aguarde a finalizacao da importacao e clique em **"Abrir agora"**, caso sua planilha nao apareca automaticamente.

### Usando funcoes no Google Sheets

Agora que temos nossos dados importados no Google Sheets, podemos comecar a operar sobre eles.

Vamos analisar quais sao os bairros com organizacoes credenciadas e quantas elas sao.

#### Criando uma tabela dinamica no Google Sheets

* Na aba superior, clique em Dados > Tabela Dinamica

* No Menu da direita, na secao "Linhas", clique em ADICIONAR e no menu, escolha Bairro

* Em Ordem, selecione Decrescente

* Em classica por, selecione COUNTA de Bairro

* Na secao "Valores", clique em ADICIONAR e selecione Bairro

* Na secao "FILTROS", clique em ADICIONAR, selecione "Status Credenciamento"

* Clique em "Mostrando todos os itens" e descelecione "DESCREDENCIADA" e clique em OK

* Feche o menu da direita, clicando no "X"

O que obtivemos e uma nova tabela, em que os bairros aparecem em ordem alfabetica e, ao lado, temos quantas organizacoes credenciadas estao presentes em cada um deles.

### Criando um grafico a partir dos dados

Vamos criar um grafico, mostrando quais bairros tem, pelo menos, 10 organizacoes ou mais cadastradas.

* Clique sobre a celula 1A e, sem soltar o clique, arraste ate a celula B11, contendo o 10 referente a ITAQUERA

* Clique em Inserir > Grafico

* Em "Tipo de grafico", selecione Grafico de colunas

* Clique na caixa "Alternar linhas/colunas"

* Assim, obtivemos um grafico com os bairros que tem mais de 10 organizacoes cadastradas e os suas quantidaes correspondentes



