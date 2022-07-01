# MapReduce-WordCount-CSV-
Creation d'un répertoire InputMapReduceHadoop.

hdfs dfs -mkdir /inputMapReduceHadoop

Copie du fichier CSV pour le mettre dans HDFS. 


hdfs dfs -put /home/cloudera/Bakery.csv /inputMapReduceHadoop

Dans eclipse exporté le projet au format Jar
![image](https://user-images.githubusercontent.com/57175461/176192697-7a006cf7-86d8-4670-8da5-b6a6b9b8e061.png)



Lancement du MapReduce


hadoop jar /home/cloudera/Bakery.jar Bakery.BakeryDriver /inputMapReduceHadoop/Bakery.csv /outputMapReduceHadoop

![image](https://user-images.githubusercontent.com/57175461/176192621-d408edc8-f490-4578-b4c2-e3e69b101672.png)

Resultat :
![image](https://user-images.githubusercontent.com/57175461/176962523-a2af112d-a014-4024-a317-093d4f397532.png)
