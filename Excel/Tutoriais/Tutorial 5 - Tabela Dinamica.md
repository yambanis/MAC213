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
