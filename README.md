PROJETO RÉGUA



Projeto desenvolvido pelo Grupo 8 na disciplina MLOps \& CI/CD do MBA em BI \& Data Science.



OBJETIVO



O Projeto Régua tem como objetivo enriquecer e aferir uma base de ocorrências policiais, construindo um pipeline reproduzível e auditável para preparação dos dados e modelagem.



A partir das circunstâncias da ocorrência, como local, horário, duração, características da vítima e do suspeito e condições externas, o projeto busca prever a classificação legal da ocorrência.



A variável-alvo do modelo é LAW\_CAT\_CD, composta pelas categorias FELONY, MISDEMEANOR e VIOLATION.



O projeto também busca estabelecer um critério objetivo de seleção de variáveis, denominado régua de ruído, para avaliar quais atributos apresentam sinal preditivo superior ao acaso.



DADOS



O projeto utiliza como base o NYPD Complaint Data Historic e prevê o enriquecimento dos dados com atributos derivados e fontes públicas externas.



Para os exercícios acadêmicos de MLOps desta disciplina, a pasta data contém dois arquivos:



\- NYPD\_Enriquecido\_amostra.csv: amostra da base enriquecida utilizada no desenvolvimento do Projeto Régua.



\- regua\_sintetico.csv: pequeno dataset sintético e fictício criado a partir de prompt de IA para testes reproduzíveis e realização dos exercícios da disciplina, sem utilização de ocorrências ou dados pessoais reais.



ESTRUTURA DO PROJETO



data/ - arquivos de dados

terraform/ - infraestrutura como código com Terraform

pulumi/ - infraestrutura como código com Pulumi

airflow/dags/ - orquestração de pipelines

kubeflow/ - recursos relacionados ao Kubeflow

app/ - aplicação

k8s/ - recursos Kubernetes

github/workflows/ - workflows de CI/CD



OBSERVAÇÃO



As associações analisadas pelo Projeto Régua são preditivas. O projeto não realiza inferência causal e não se destina à tomada automatizada de decisão sobre casos individuais.

