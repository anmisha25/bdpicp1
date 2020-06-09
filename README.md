# bdpicp1

Create the new directory in HDFS:

hdfs dfs -mkdir user/hadoop

Copy files from Local to HDFS:

hdfs dfs -copyFromLocal Desktop/BDP/shakespeare.txt /user/hadoop/.

hdfs dfs -copyFromLocal Desktop/BDP/word_list.txt /user/hadoop/.

Append the file:

hdfs dfs -appendToFile Desktop/BDP/word_list.txt /user/hadoop/shakespeare.txt

now we Get first and last 5 lines of file:

hdfs dfs -cat /user/hadoop/shakespeare.txt | head -5

hdfs dfs -cat /user/hadoop/shakespeare.txt | tail -5
