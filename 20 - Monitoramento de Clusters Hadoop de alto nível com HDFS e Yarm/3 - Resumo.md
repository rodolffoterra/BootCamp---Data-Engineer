## Resumo



**HDFS** é a camada de armazenamento do Hadoop;

- Divide os dados em blocos e os distribui pelo clustes;
- -Os workers rodam o daemon DataNode e o master o daemon NameNode;



**MapReduce** foi o primeiro framework de computação distribuída utilizado com o HDFS;

- Levou o processamento aos servidores onde o dado está armazenado.



**YARN** gerencia os recursos no cluster

- Trabalha com o HDFS para executar as tarefas quando o dado é armazenado;
- Os workers rodam o daemon "NodeManager" e o master o daemon "ResourceMaganger";
- É possível monitorar os jobs atrav´[es da porta 8088.



Aplication:

![image-20210708124144082](C:\Users\USER\AppData\Roaming\Typora\typora-user-images\image-20210708124144082.png)

