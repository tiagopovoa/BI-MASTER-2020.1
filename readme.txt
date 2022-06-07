# ALOCAÇÃO DE INVESTIMENTOS EM FIIs (FUNDO DE INVESTIMENTO IMOBILIARIO) #

Aluno: TIAGO RAMOS POVOA (https://gist.github.com/tiagopovoa) E FREDERICO MARANH O CUNHA (https://gist.github.com/fremcunha)
Orientador: [Felipe Borges](https://github.com/FelipeBorgesC) 


Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pre-requisito para conclusao de curso e obtenc o o de cr dito na disciplina "Projetos de Sistemas Inteligentes de Apoio   Decis o".


## RESUMO

Fundos de Investimento Imobiliario (FIIs) foram criados pela Lei n  8668/93, sendo definido pela  comunh o de recursos, captados  por meio de sistema de distribuição  de valores mobiliários, destinados e  aplicação em Empreendimentos
imobiliários 

E dezembro/20 existiam mais de 300 FIIs listados na B3, com o Patrimonio de R$ 122 Bilh es. 

Qual investir? Vamos entender a nossa modelagem que bateu o IFX entre 2015-2021.


## 1. INTRODUÇÃO

Com inúmeras quantidade de FIIs, queriamos investir R$ 1 MM em FIIs de modo a reduzir a volatilidade e maximizar o retorno da carteira.


## 2. MODELAGEM

Primeiramente, rodamos um modelo que comparava o Resultado da Carteira escolhida com o IFX, de forma segmentada, entre abril-set/21.

Rodamos o modelo de Otimiza  o com a ferramenta Solver LP Simplex, com as restri  es para a nossa carteira:  

Segmentos de FII:
- CRI (Certificado de Cr dito Imobili rio)  - 24%
- Logistica                                 - 16%  	 
- Renda Urbana                              - 14%  	 
- FOF (Fundo de Fundo )                     - 10% 
- Agencias                                  -  8% 
- Laje Corporativa                          -  7%  	 
- Malls                                     -  10%  	 
- Demais                                    -  11% 

Restrições:
1: carteira totalmente alocada = 100% 
2: volatilidade m xima = 12,0%
3: alocação nos setores =< 20% acima) 
4: alocação máximo por papel = 2,5%

No segundo momento, fizemos o Re-teste entre o per odo de 01 a 15 dias de out/21.

Finalmente, comparamos o resultado financeiro da carteira entre jan/15 a dez/21 com o IFX. Tamb m analisamos as correlações do IFX x Indicadores de Mercado ( % Selic, NTN-B e Efeito Eleições).


## 3. RESULTADOS

[No 1o] IFX x Carteira - abril/21 a set/21.
       
        > Nossa carteira: - rentabilidade de 0,2% c/ vol 12,00%
        > IFX             - rentabilidade de -4,8% c/ vol 13,79%4,
        Destaques    - Em nossa carteira  possui 41 FIIs;
                     - A volatilidade (vol) da nossa carteira atingiu 12% e a rentabilidade bem superior (+0,2%) comparado ao Indice IFX (-4,78%) e vol superior (13,79%)
                     - Segmentos em destaque:  CRI, Malls, Renda Urbana; 
			   - Sem Aloca  o em Fundo de Agencias.
 
[No 2o]  Re-teste entre o per odo de 01 a 15 dias de out/21
       
        > Nossa carteira: - 0,63% c/ vol 8,81%
        > IFX             - 1,08% c/ vol 10,34%

        Destaques    - Apresentando uma vol menor que o IFX porém com um rentabilidade menor.
                     - Segmentos em destaque:  CRI, FOF, Malls, Logistica 
			   - Sem Alocação em Fundo de Agencias.

[No 3o] Por fim, fizemos uma análise no  periodo de 6 anos (2015 a 2021), a nossa carteira valorizou 110% enquanto o IFIX atingiu 99%.
        Fizemos também uma análise entre o IFX e indicadores de mercado ( Selic, NTN-B) e também a períodos de Eleições Presidenciais.
      
	Destaques    - Nao encontramos correlação entre IFX x Selix ou IFX x NTN-B.
                   - Identificamos uma correlaão entre Juros Pré em anos de Eleicoes Presidencias 
                    

## 4. CONCLUSÃO

O Modelo de Otimizacao com a ferramenta Solver LP Simplex se mostrou bem eficiente para alocacaoo de recursos em FII sem demostrando uma melhor rentabilidae que o IFX ao longos dos ultimos 6 anos (2014-21).




Matricula Tiago Ramos P voa: 2011 90 203
Matricula Frederico Cunha:   201.190.258


Pontificia Universidade Cat lica do Rio de Janeiro
Curso de Pós Graduação Business Intelligence Master
