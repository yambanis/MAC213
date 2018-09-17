# Introdução ao Excel

Tópicos a serem cobertos

* O que é uma planilha?
    Morfologia básica
    
* Importando conjunto de dados

## O que é uma planilha? 

A planilha ou inglês spreadsheet e uma aplicação de software que tem como finalidade salvar e organizar dados em linhas e colunas.

Usaremos a versão 2016 do Excel neste tutorial mas tudo deve ser equivalente para outras versões.

![Tela inicial do Excel 2016](tela_inicial.PNG)

Alguns dos elementos presentes na tela inicial do Excel são:

1. Células
2. Linhas - indicadas por números
3. Colunas - indicadas por letras
4. Barra de fórmulas
5. Faixa de opções 
6. Nome da planilha atual

## Importando conjuntos de dados

### Baixando os dados
Vamos começar importando um conjunto de dados para nosso trabalho.

Primeiramente, acesse [a pagina de dados abertos da prefeitura](http://dados.prefeitura.sp.gov.br/organization/educacao1). Nela existem diversos bancos de dados abertos. 

Para o nosso tutorial iremos usar o conjunto de dados [Perfil dos educandos ](http://dados.prefeitura.sp.gov.br/dataset/perfil-dos-educandos-cor-raca-idade-sexo-necessidades-educacionais-especiais)

Nesta página encontramos três arquivos: Dicionário, que consta uma explicação das siglas, e dois arquivos .csv - um extraído em 2017 e um 2016.


![Baixando arquivo .csv](download.png)

Clique em explorar e selecione a opção Baixar

Você pode reparar que existem dois tipos de arquivo, o de extensão .CSV e o .XLSX
![extensoes](extensao.png)

Os arquivos .CSV são arquivos de "valores separados por vírgulas". São dados em tabelas que foram salvos como arquivos de texto.

Já os arquivos .XLSX ou .XLS são arquivos nativos do Excel.

Não vamos entrar em mais detalhes por enquanto, o importante é que conseguimos editar ambos os tipos de arquivo com o Excel.

## Abrindo o arquivo

### Opção 1 - abrir em um novo arquivo

Se você ainda não tem um arquivo de excel em que está trabalhando, pode ser mais prático apenas abrir o arquivo e deixar que o excel faça a importação automaticamente.

Simplesmente abra a pasta onde você fez o download do arquivo e dê um click duplo sobre ele.

Se você já tiver o excel instalado em seu computador, ele irá avaliar automaticamente o arquivo .csv como uma planilha e fará todo o processo automaticamente.

No final, você terá uma tela parecida com esta:

![importado](importado.png)



### Opção 2 - importar

Se você já tem uma planilha em que está trabalhando e deseja importar esse novo conjunto de dados

* Clique na aba "Dados"
* selecione a opção "Obter dados externos"
* escolha " de texto"

![Importando CSV](importar.png)

Escolha o arquivo que deseja importar, no nosso caso, idadeserieneeracadez17.csv, que fizemos o download na sessão anterior

Apareceram 3 telas do assistente de importação

1. Selecione "delimitado" e "Meus dados possuem cabeçalhos". Clique "Avançar >"


![Assistente 1](assist1.png)

2. Selecione "Ponto e vírgula". Clique "Avançar >"


![Assistente 2](assist2.png)

3. Finalmente, apenas clique "Concluir"
![Assistente 3](assit3.png)

4. Na tela "Importar dados" você pode selecionar coletar os dados na planilha existente ou em uma nova planilha. Neste momento, vamos selecionar a planilha existente.


![Assistente 4](assist4.png)

Depois de finalizado este processo, sua planilha deve parecer com algo similar a isto:

![importado](importado.png)


