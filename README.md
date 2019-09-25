# FCA2 FC Auto Analyser v0.6 beta (set/19)

(English version on the way - please be pacient)

FCA2 é um algoritmo em Python criado para análise exploratória básica de dados, que visa trazer produtividade para analistas. De forma automática, o algoritmo captura arquivos em formato csv, xls e xlsx e realiza diversas análises:

__ identificação de campos texto, campos numéricos inteiros e números decimais

__ campos texto: quantidade de registros, duplicações e de categorias, top "n" categorias (baseada em max_freq)

__ campos numéricos: quantidade de registros, registros zerados, soma total, média, desvio, máximos e mínimos, amplitude, quatis. Mesmas descrições para a base descontando os registros zerados

Desenvolvido por Fabiano Castello, é disponibilizado sob licença GNL3.0 para toda a comunidade. O código está construído com a estrutura de códigos estruturados dos anos 80. FCA2 é disponibilizado em beta. Use por seu próprio risco.

Contato com o desenvolvedor original em fabianocastello.com 
Código mais atualizado disponível em github.com/fabianocastello/fca2
Código original registrado no DOI abaixo:
https://doi.org/10.6084/m9.figshare.9902417

## DEPENDÊNCIAS
FCA2 utiliza os seguintes pacotes:
os, sys, numpy, requests, pandas, datetime, time, socket, locale, seaborn, mathplot

## PARÂMETROS
Parâmetros podem ser alterados no início do código. São auto-explicativos:

datain  = ".\data.in"    #coloque aqui seus arquivos xls ou csv
dataout = ".\data.out"   #onde analisador vai gravar os resultados
datalog = ".\data.log"   #onde o analisador vai gravar os logs do processamento 
datatmp = ".\data.tmp"   #arquivos temporários. Será limpo após o processamento

max_freq = 10            #numeros de categorias máximas nos campos texto 

## COMO USAR

FCA2 rodar, atualmente, a partir de cadernos do Jupyter Notebook, com Kernel Python 3. Recomendo fortemente instalação do Anaconda (www.anaconda.com).

Para rodar o analizadort basta colocar seus arquivos formato xls, xlsx ou csv no diretório de entrada. A leitura é automática e a análise de cada arquivo é disponibilizada no diretório de saída, com o mesmo nome do arquivo.

## NOTAS IMPORTANTES

__ várias pastas em arquivos xls ou xlsx: o FCA2 pegará a primeira delas para analisar.

__ vírgula "," ou ponto e vírgula ";" em arquivos CSV: o FCA2 conta o número de ocorrências de cada tipo na primeira linha do arquivo, e considera como separador o maior número de ocorrências


## NO FUTURO

__ colocar todas as informações juntas em um PDF.

__ inserir data labes nos histogramas.

__ montar correlação entre variáveis numéricas.

__ criar uma versão compilada para ampliar o uso por pessoas que não usam python



