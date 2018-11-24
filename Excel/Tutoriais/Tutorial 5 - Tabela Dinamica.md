# Tabela Dinamica

Vamos importar a base de dados [sobre Rendimento e movimento escolar](http://dados.prefeitura.sp.gov.br/dataset/rendimento-e-movimento-escolar-ensino-fundamental).

Comecamos abrindo um novo arquivo, selecionando _Arquivo -> Importar_.

Selecionamos Upload e realizamos a transferencia do arquivo "censoevolutivomovimentorendimento.csv".

No campo "Tipo de Separador", escolher Personalizado e digitar o simbolo de ponto e virgula.

![A.gif](../Gifs/Dinamica/A.gif)

Agora, em uma nova planilha, selecionamos _DADOS -> Tabela Dinamica_

No campo "Quais dados?" selecionamos a planilha "censoevolutivorendimento" em sua totalidade, selecionando o quadrado cinza no canto superior esquerdo das celulas.

![B.gif](../Gifs/Dinamica/B.gif)

Vamos agora fazer uma analise da evolucao das taxas de reprovacao e evasao das unidades, ao longo dos anos.

Para isso, vamos criar uma tabela dinamica com 3 colunas: Ano, numero de abandonados, aprovados e reprovados.

Para isso, vamos primeiro selecionar _ANO_ no campo Linhas.

Em seguida, no campo valores, vamos clicar 3 vezes em adicionar e selecionar _TOTALEF_ABAND_, TOTALEF_REPROV e _TOTALEF_APROV_.

![C.gif](../Gifs/Dinamica/C.gif)

Vamos agora criar uma nova coluna, para guarda o valor do total de alunos do ensino fundamental e uma outra para guardar o total de não aprovados(reprovados + abandonos)

![D.gif](../Gifs/Dinamica/D.gif)

Vamos copiar os valores relativos aos aprovados e reprovados em 2015 e criar um grafico de pizza para representar esses dados.

![E.gif](../Gifs/Dinamica/E.gif)

Vamos criar um grafico de areas empilhadas, selecionando os dados relativos ao numero de abandonos e reprovacoes de todos os anos que temos acesso. Vamos excluir o ano de 2014, pois parece haver um erro neste ano, ja que todos os valores sao zero.

Assim, sera possivel obter uma visualização do numero de não-aprovados(reprovados e abandonados) e a evolução com os anos.

![F.gif](../Gifs/Dinamica/F.gif)
