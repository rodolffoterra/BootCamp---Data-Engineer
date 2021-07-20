# Digital Innovation One

Código criado para utilização junto a plataforma da Digital Innovation One

<p align="center"><img src="./DIO.png" width="500"></p>

## Desafio GCP Dataproc

O desafio faz parte do curso na plataforma da Digital Innovation One:

__*Criando um ecossitema Hadoop totalmente gerenciado com Google Cloud Platform*__

O desafio consiste em efetuar um processamento de dados utilizando o produto Dataproc do GCP. Esse processamento irá efetuar a contahem das palavras de um livro e informar quantas vezes cada palavra aparece no mesmo.

---

### Etapas do Desafio

1. Criar um bucket no Cloud Storage
    1. Criação de um orçamento de Alerta
    1.  Análise de faturamento
    1. Habilitação do API: DataProc e Computer Engine
    1. Criar um cloud Stoprage
    1. Criar o clusters
1. Atualizar o arquivo ```contador.py``` com o nome do Bucket criado nas linhas que contém ```{SEU_BUCKET}```.
1. Fazer o upload dos arquivos ```contador.py``` e ```livro.txt``` para o bucket criado (instruções abaixo)
    - https://cloud.google.com/storage/docs/uploading-objects
1. Utilizar o código em um cluster Dataproc, executando um Job do tipo PySpark chamando ```gs://{SEU_BUCKET}/contador.py```
1. O Job irá gerar uma pasta no bucket chamada ```resultado```. Dentro dessa pasta o arquivo ```part-00000``` irá conter a lista de palavras e quantas vezes ela é repetida em todo o livro.

### Entrega do Resultado

1. Criar um repositório no GitHub.
2. Criar um arquivo chamado ```resultado.txt```. Dentro desse arquivo, colocar as 10 palavras que mais são usadas no livro, de acordo com o resultado do Job.
3. Inserir os arquivo ```resultado.txt``` e ```part-00000``` no repositório e informar na plataforma da Digital Innovation One.

----

## Alguns comandas na VM

rodolffoterra@cloudshell:~ (desafiodiodataproc)$ **gcloud compute instances list**
NAME             ZONE           MACHINE_TYPE   PREEMPTIBLE  INTERNAL_IP  EXTERNAL_IP     STATUS
instance-hadoop  us-central1-a  e2-standard-4               10.128.0.2   34.133.251.234  RUNNING

---

### Realizando o desafio

* Abrir o cloud shell

* cloune do repositório: https://github.com/marcelomarques05/dio-desafio-dataproc.git

  ​	$ git clone https://github.com/marcelomarques05/dio-desafio-dataproc.git

  ​	$ cd dio-desafio-dataproc/

  ​	$ ls - la

  ​	$ gsutil ls

  ​	$ gsutil cp contador.py livro.txt gs://desafio-dataproc-rodolfo/

