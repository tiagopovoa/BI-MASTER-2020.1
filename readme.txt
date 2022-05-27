# ALOCA��O DE INVESTIMENTOS EM FIIs (FUNDO DE INVESTIMENTO IMOBILIARIO) #

Aluno: TIAGO RAMOS POVOA (https://gist.github.com/tiagopovoa) E FREDERICO MARANH�O CUNHA 
Orientador: [Felipe Borges](https://github.com/FelipeBorgesC) 


Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pre-requisito para conclusao de curso e obtenc�o o de cr�dito na disciplina "Projetos de Sistemas Inteligentes de Apoio � Decis�o".


## Resumo

Fundos de Investimento Imobili�rio (FIIs) foram criados pela Lei n� 8668/93, sendo definido pela  comunh�o de recursos, captados  por meio de sistema de distribui��o  de valores mobili�rios, destinados �  aplica��o em �empreendimentos
imobili�rios�..... e em dezembro/20 existiam mais de 300 FIIs listados na B3, com o Patrimonio de R$ 122 Bilh�es.


## 1. Introdu��o

Com in�meras quantidade de FIIs, queriamos investir R$ 1 MM em FIIs de modo a reduzir a volatilidade e maximizar o retorno da carteira.


## 2. Modelagem
Primeiramente, rodamos um modelo que comparava o Resultado da Carteira escolhida com o IFX, de forma segmentada, entre abril-set/21 
Rodamos o modelo de Otimiza��o com a ferramenta Solver LP Simplex, com as restri��es para a nossa carteira:  carteira totalmente alocada = 100% 2: volatilidade m�xima = 12,0%
3: aloca��o nos setores =< 20% acima) 4: aloca��o m�ximo por papel = 2,5%
No segundo momento, fizemos o Re-teste entre o per�odo de 01 a 15 dias de out/21.
Finalmente, comparamos o resultado financeiro da carteira entre jan/15 a dez/21 com o IFX.

## 3. Resultados

[No 1o] > Nossa carteira: - 0,2% c/ vol 12,00%
        > IFX             - 4,8% c/ vol 13,79%

[No 2o] > Nossa carteira: - 0,63% c/ vol 8,81%
        > IFX             - 1,08% c/ vol 10,34%

[No 3o] No per�odo de 6 anos (2015 a 2021), a Nossa Carteira valorizou 110% enquanto o IFIX atingiu 99%.

## 4. Conclus�o

O Modelo de Otimiza��o com a ferramenta Solver LP Simplex se mostrou bem eficiente para aloca��o de recursos em FIIs.



Matricula Tiago Ramos P�voa: 2011 90 203

Matricula Frederico Cunha:  201.190.258


Pontif�cia Universidade Cat�lica do Rio de Janeiro
Curso de P�s Gradua��o Business Intelligence Master
