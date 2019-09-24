#FCA2 FC Auto Analyser v0.4 beta (set/19)

FCA2 é um algoritmo em Python criado para análise exploratória básica de dados, que visa
trazer produtividade para analistas. Desenvolvido por Fabiano Castello, é disponibilizado
sob licença GPU GNL 3.0 para toda a comunidade.

O código está construído com a estrutura de códigos estruturados dos anos 80.
FCA2 é disponibilizado em beta. Use por seu próprio risco.

Contato com o desenvolvedor original em fabianocastello.com
Código mais atualizado disponível em github.com/fabianocastello

#PARÂMETROS
Parâmetros podem ser alterados no início do código. São auto-explicativos:

datain  = ".\data.in"    #coloque aqui seus arquivos xls ou csv
dataout = ".\data.out"   #onde analisador vai gravar os resultados
datalog = ".\data.log"   #onde o analisador vai gravar os logs do processamento 
datatmp = ".\data.tmp"   #arquivos temporários. Será limpo após o processamento

max_freq = 10            #numeros de categorias máximas nos campos texto 

#COMO USAR

Basta colocar seus arquivos formato xls, xlsx ou csv no diretório de entrada.
A leitura é automática.

#NOTAS IMPORTANTES

> várias pastas em arquivos xls ou xlsx: o FCA2 pegará a primeira delas para analisar.
> Vírgula "," ou ponto e vírgula ";" em arquivos CSV: o FCA2 conta o número de ocorrências 
de cada tipo na primeira linha do arquivo, e considera como separador o maior número de ocorrências
