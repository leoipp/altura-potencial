# Altura Máxima Potencial de Vegetação Nativa do Estado de Minas Gerais

A altura do dossel florestal tem importante significado para a ecologia e para o manejo florestal. Uma alternativa para medição da altura de florestas é a utilização de sistemas lidar orbitais, como o Global Ecosystem Dynamics Investigation (GEDI), que podem fornecer medidas exatas e precisas da elevação. 
Para grandes extensões de terra, como o estado de Minas Gerais, a utilização de modelos de máquina de aprendizagem para predição de altura pode ser necessária. Nestes modelos, o algoritmo realiza a correlação de diferentes variáveis que podem exercer influência sobre a altura do dossel como solo, clima e topografia. 

## Objetivo do Script

Estimar a altura máxima potencial de vegetação nativa para o estado de Minas Gerais por meio de interpolação de dados do GEDI nível 3 e variáveis ambientais. Apenas os dados
lidar GEDI nível 3 correspondentes às classes de uso e ocupação do solo obtidas pelo MapBiomas relacionadas às formações florestais, savânicas e campestres foram selecionados.
O filtro de máximos locais foi aplicado sobre as variáveis ambientais de precipitação e temperatura média anual, modelo digital de elevação, declividade, número de dias sem nuvens
e número de meses com precipitação inferior a 100 mm para obtenção das observações correspondentes à fronteira de eficiência. Aqueles que apresentaram correlação com os dados de altura relativa do GEDI nível 3, foram escolhidos para treinamento do modelo random forest. 

## O Modelo

O modelo ajustado estimou as alturas máximas potenciais de vegetação nativa para o estado de Minas Gerais de acordo com as variáveis ambientais selecionadas. A variabilidade do estado, em função de sua extensão e diferenças geográficas, se caracterizou pelas diferentes alturas máximas potenciais de vegetação nativa estimadas.
