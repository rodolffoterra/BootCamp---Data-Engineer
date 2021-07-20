## HDFS



## 1.0 O que é HDFS



#### Copiar arquivo HDFS para local

$ hdfs dfs -get /tmp/file_tste.txt



#### Ingestão manual

$ hdfs dfs -put file_teste.txt / user/**nameuser**-bigdata/ 



****



## 2.0 Principais comandos 

$  sudo -u hdfs hdfs -chmod -R 777 /tmp

$ hdfs dfs -ls -h/

$ hdfs dfs -cat /tmp/file_teste.txt |head -10

$ hdfs dfs -rm /tmp/file_teste.txt

$ hdfs dfs -mkdir /tmp/delete

$ hdfs dfs -cp /tmp/file_teste.txt /tmp/delete/

$ hdfs dfs -touchz /tmp/delete/empty_file

$ hdfs dfs -rm -R /tmp/delete

$ hdfs fsck /temp/ -files - blocks 



****

