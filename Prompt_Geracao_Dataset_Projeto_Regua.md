Gere um dataset sintético e 100% fictício em formato CSV para o Projeto Régua, um projeto de Machine Learning voltado ao enriquecimento e à aferição de uma base de ocorrências policiais.



Contexto: o Projeto Régua busca utilizar características relacionadas às circunstâncias de uma ocorrência — como local, horário, duração, características da vítima e do suspeito e condições externas — para prever sua classificação legal. O dataset sintético será utilizado exclusivamente para testes e exercícios de MLOps, sem utilização de dados pessoais ou ocorrências reais.



Gere exatamente 40 registros, com as seguintes colunas:



1\. id — tipo inteiro — identificador sequencial único do registro.

2\. borough — tipo categórico — região fictícia da ocorrência, utilizando as categorias Manhattan, Brooklyn, Queens, Bronx e Staten Island apenas como categorias geográficas de teste.

3\. periodo\_dia — tipo categórico — período em que ocorreu o fato: Madrugada, Manhã, Tarde ou Noite.

4\. dia\_semana — tipo categórico — dia da semana em que ocorreu o fato.

5\. fim\_de\_semana — tipo booleano — indica se a ocorrência aconteceu em sábado ou domingo.

6\. idade\_vitima — tipo inteiro — idade fictícia da vítima em anos.

7\. idade\_suspeito — tipo inteiro — idade fictícia do suspeito em anos.

8\. duracao\_minutos — tipo inteiro — duração estimada e fictícia da ocorrência em minutos.

9\. ambiente — tipo categórico — ambiente predominante da ocorrência: Residencial, Comercial, Via Pública, Transporte ou Outro.

10\. temp\_media\_c — tipo decimal — temperatura média fictícia, em graus Celsius, associada ao período da ocorrência.

11\. precipitacao\_mm — tipo decimal — precipitação fictícia, em milímetros, associada ao período da ocorrência.

12\. feriado — tipo booleano — indica se a data fictícia da ocorrência corresponde a um feriado.

13\. taxa\_desemprego — tipo decimal — indicador socioeconômico fictício associado à região da ocorrência.

14\. renda\_mediana\_domiciliar — tipo decimal — renda mediana domiciliar fictícia associada à região.

15\. LAW\_CAT\_CD — tipo categórico — classificação legal da ocorrência e coluna-alvo do modelo, utilizando as categorias FELONY, MISDEMEANOR e VIOLATION.



Coluna-alvo (target): LAW\_CAT\_CD, com as categorias FELONY, MISDEMEANOR e VIOLATION.



Regras importantes:



* &#x20;Todos os registros devem ser integralmente fictícios e utilizados exclusivamente para fins acadêmicos.
* Não utilizar nomes de pessoas, números de ocorrências ou descrições de casos reais.
* Distribuir os registros de forma aproximadamente equilibrada entre as três categorias da coluna LAW\_CAT\_CD.
* Manter relações plausíveis entre as variáveis, sem afirmar relações causais entre condições ambientais, socioeconômicas e criminalidade.
* Incluir propositalmente 4 valores faltantes na coluna idade\_vitima, para permitir testes de tratamento de dados ausentes.
* Incluir propositalmente 2 outliers na coluna duracao\_minutos, com valores significativamente superiores ao padrão dos demais registros.
* Incluir propositalmente 2 outliers na coluna precipitacao\_mm.
* Utilizar ponto como separador decimal.
* Retornar apenas o conteúdo CSV, com o cabeçalho na primeira linha e os campos separados por vírgulas, sem explicações, comentários ou blocos Markdown.



