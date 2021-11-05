# AWS-Big-Data-Desafio
 Criando seu Ecossistema de Big Data na Nuvem

## Desafio
Com base no repositório disponibilizado pelo expert,
te desafiamos a replicar e, porque não, 
melhorar o algoritmo de extração/contabilização de palavras. 
Para isso, você pode ordenar as palavras por ocorrência
e não por ordem alfabética (apresentando as mais citadas no
texto com prioridade), por exemplo. 
Sinta-se à vontade para evoluir o algoritmo de outras formas ;)

### Criando ambiente virtual em Python

virtualenv --python=python3.6 venv_diolive_edu


### Instalando apps e bibliotecas úteis

VSCode: code . \n
Boto3: pip install boto3
MrJob: pip install mrjob


### Startando o ambiente virtual

source venv_diolive_edu_prod/bin/activate


### Startando o algoritmo

python3 wordcount.py -r emr s3://dio-live-datalake-prod/data/sherlock_holmes.txt --cloud-tmp-dir=s3://dio-live-datalake-prod/temp
