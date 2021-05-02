# Processo-Quaest

### Objetivo: 
Este repositório tem por objetivo a realização da avaliação técnica proposto pela Quaest em seu processo seletivo para estagiário em Ciência de Dados. A avaliação é composta por três questões a respeito de uma base de dados composta por respostas de survay de eleitores.

<br>
Todas as explicações e códigos detalhados estarão dentro do notebook ''. É só abrir e conferir
Abaixo terá um resumo das respostas das questões, apenas no formato de texto/gráficos.
 
<br>
<br>
Intenção de Votos Válidos: Voto em algum dos candidatos
OBS: para todo o trabalho, foi considerado apenas as intenções válidas e brancos/nulos na formação do total, visto que brancos/nulos + intenções válidas precisa dar 100%.
Os que não responderam não foi levado em consideração, ou seja, temos apenas 860 registros válidos.

### Questão 1 - Qual o % de intenção de voto para cada candidato?
### Resposta: <br>
Utilizando o data['voto1'].value_counts() é possível ver os valores únicos que este atributo pode assumir e suas respectivas quantidades. É possível ver a existência de 14 candidatos e também os que votam branco/nulo. <br>
OBS: Não será considerado como intenção de voto os que não sabem/ não responderam. Por isso, a quantidade total de registros será 860 e não 1000, pois temos 140 respostas nessa classificação <br> <br>
Candidato 1 = 42/ 860 = 0,04883% = 4.883% <br>
Candidato 2 = 523/ 860 = 0,6081% = 60.81% -- Maior Porcentagem<br>
Candidato 3 = 16/ 860 = 0,01860% = 1.86% <br>
Candidato 4 = 12/ 860 = 0,01395% = 1.395% <br>
Candidato 5 = 25/ 860 = 0,02906% = 2.906% <br>
Candidato 6 = 10/ 860 = 0,01163% = 1.163% <br>
Candidato 7 = 7/ 860 = 0,00814 = 0.814% <br>
Candidato 8 = 26/ 860 = 0,03023 = 3.023% <br>
Candidato 9 = 19/ 860 = 0,0221% = 2.21% <br>
Candidato 10 = 20/ 860 = 0,02325% = 2.325% <br>
Candidato 11 = 3/ 860 = 0,0035% = 0.35% <br>
Candidato 12 = 6/ 860 = 0,0070% = 0.7% <br>
Candidato 13 = 3/ 860 = 0,0035% = 0.35% <br>
Candidato 14 = 6/ 860 = 0,0070% = 0.7% <br>

<p align="center"> 
<img src="./prints/question1.png" >
</p>

### Questão 2 - Qual o candidato com maior % de intenção de voto entre as MULHERES?
### Resposta: <br>

O Candidato 2 possui a maior porcentagem de intenção de votos entre as MULHERES, o que corresponde a mais de 63% da intenção dos votos delas. Foi excluído todos os registros (linhas) que possuíam o atributo 'sexo' classificado como 'masculino' para que se fosse trabalhado apenas com as mulheres e também as que não responderam o Survey, criando uma nova base de dados filtrada. Após isso, apenas foi checado o atributo de intenção de votos e feito o cálculo da porcentagem. <br> <br>
OBS: As que não responderam não entraram no cálculo


### Questão 3 - O candidato que lidera as intenções de voto é o candidato de situação ou oposição ao governo ?
### Resposta: <br>
Considerando apenas as 523 pessoas que tem intenção de voto no Candidato 2 (é ele quem lidera), é perceptível que a avaliação que elas fizeram ao governo é extremamente positiva, visto que mais de 86% deles disseram que é "boa/ótima" e se incluir "regular positiva" somatiza quase toda a totalidade. Dessa forma, se eles avaliaram bem o governo e a intenção deles é realizar o voto no Candidato 2, então é muito provável que o mesmo seja o candidato de situação. <br><br>

<p align="center"> 
<img src="./prints/question3.png" >
</p>
