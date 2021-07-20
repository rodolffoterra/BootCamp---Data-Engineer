## YARN 



### 1.0. Introdução a Yarn e primeiros comandos



$  sudo service  **haddop-hdfs-namenode** start

$  sudo service  **haddop-hdfs-secondarymenode** start

$  sudo service  **haddop-hdfs-datanode** start

$  sudo service  **haddop-mapreduce-historyserver** start

$  sudo service  **haddop-yarn-resourcemanager** start

$  sudo service  **haddop-yarn-nodemaneger** start

****



### 2.0 Comandos com YARN - Parte 2

$ sudo sed -i 's|hdfs://hdfs://bigdata-srv:8020/|g'/etc/hadoop/conf/yarn-site.xml



$ ssh **ip.de.vcs** -l **nameuser**



$ dudo -u hdfs yarn jar /usr/lib/hadoop-mapreduce/hadoop-mapreduce-exemples.jar wordcount /tmp/file_teste.txt /tmp/wc_output

****

#### Para ler o arquivo

$ hdfs dfs -cat /tmp/file_teste.txt | head(10)

$ hdfs dfs -ls /tmp/wc_output

$ hdfs dfs -cat /temp/wc_output/part-r-00000

****



### 3.0 Comandos com YARN - Parte 3



$ sudo -u hdfs yarn lods -applicationId **application_1611089476809_0001** | more



resoltado em texto puro

$ sudo -u hdfs yarn logs -applicationId a**pplication_1611089476809_0001** > wordcount.log



$ sudo -u hdfs yarn lods -applicationId **application_1611089476809_0001** | tail -f

<--Acompanhar em tempo de execução -->













