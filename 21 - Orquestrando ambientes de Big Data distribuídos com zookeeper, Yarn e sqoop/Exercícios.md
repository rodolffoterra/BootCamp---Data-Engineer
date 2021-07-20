## Exercíciuos

**Import subset com Sqoop seguindo as seguintes premissas:**

​	**1) Todos os Pokémons lendários**

$ sudo -u hdfs sqoop import \

​	--connect jbdc:mysql://localhost/trainning \ 

​    --username root --password "Everis@2021" \

​	--direct \

​	--table pokemon \ 

​	--target-dir /user/everis-bigdata/pokemon/i \

​	--where "Legendary=1"

****



​	**2) Todos os Pokémons de apenas um tipo**



****



​	**3) Os top 10 Pokémons mais rápidos**



****

​	**4) Os top 50 Pokémons com menor HP**



****

​	**5) Os top 100 Pokémons com maiores atributos**



​	 	