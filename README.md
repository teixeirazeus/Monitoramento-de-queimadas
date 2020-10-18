# Monitoramento-de-queimadas
Projeto para monitorar e identificar queimadas na região de Pocone - Mato Grosso, através de drones utilizando inteligência artificial.

## O problema das queimadas no Brasil
No ano de 2020 as queimadas ganharam foco nos assuntos mais importantes do ano perante o público e a mídia, o que é de se esperar, só em 2020 os pesquisadores estimam que uma área de 23 mil km² foi perdida para as queimadas. Para o tamanho do Brasil, o número não é muito expressivo, porém essa área corresponde a ¼ de Portugal, ou para melhor senso de comparação, quase 10 vezes o tamanho de Luxemburgo.

Outros países como os Estados Unidos e a Austrália também sofreram sérios danos durante o ano de 2020 referentes às queimadas, sendo que na Austrália, estima-se que as queimadas mataram ou removeram de seu habitat natural cerca de 3 bilhões de animais,sendo considerado a maior catástrofe da fauna da história moderna.

De acordo nossos estudos usando um [bando de dados](http://dados.gov.br/dataset/sistema-nacional-de-informacoes-florestais-snif) do governo brasileiro sobre queimadas, é notavel o aumento do numero de queimadas no Brasil, considerando o tempo de 1998 até 2017, como demonstra a figura 1.
<br>
<img src="./graficos/aumento_queimadas.png" width="600">
<br>
Somando todos as ocorrências de queimadas neste período e classificando por estados, conforme a Figura 2, o Mato Grosso se destaca, sendo o estado com maior ocorrência de queimadas.
<br>
<img src="./graficos/estadosx.png" width="600">
<br>
A cidade escolhida para a implementação do projeto foi Poconé no sul do Mato Grosso, a cidade com um dos maiores números de incidentes com queimadas, concentrando 16% das queimadas no Mato Grosso, sengundo nossas analise do [bando de dados](http://queimadas.dgi.inpe.br/queimadas/portal) de queimada do Instituto Nacional de Pesquisas Espaciais (INPE), no período de 2019-2020.
<br>
<img src="./graficos/pocone.png" width="600">
<br>
Poconé é o segundo municipio com mais ocorrências de queimadas no Brasil, com 210.805 ocorrências, perdendo somente para Corumba Mato Grosso do Sul com 229.153 ocorrências. Foi escolhido um municipio do Mato Grosso, pois além de ser o estado com maior concentração de queimadas, dos Top 10 municipio com queimadas do Brasil, 3 são de Mato Grosso.
<br>
<img src="./graficos/Municipios.png" width="600">
<br>


## O projeto
No Brasil, as áreas de queimada exigem grande esforço para serem identificadas, ou por se localizarem em mata fechada, ou por estarem em ambiente acidentado. A utilização de drones começou a ser implementada para resolver esse problema, permitindo que bombeiros e voluntários soubessem exatamente onde a queimada se localiza antes de se locomover, porém, essa opção depende de um diagnóstico humano e toda a operação depende de um piloto para o drone, além de depender de alguma denúncia ou resquício que há fogo no lugar.

Nossa solução consiste em um drone de patrulha equipado com uma câmera térmica, instalada para identificar temperaturas elevadas juntamente com um algoritmo de classificação, responsável por dar autonomia ao equipamento e retirando a necessidade de um operador durante a patrulha. O drone conta com uma inteligência artificial desenvolvida pela equipe para identificar imagens que contém fogo ou fumaça, permitindo uma análise automática, sem necessidade de um operador/piloto.
