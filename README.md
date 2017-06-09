# Word Count on Tweets using MapReduce

**Files:**
1. /input/football.txt : Tweets on the topic Soccer
2. /output1/part-r-00000 : Output of MapReduce
3. /Tweets.ipynb : R code to obtain the tweets
4. /WordCloud.ipynb : R code to obtain the wordcloud
5. /WordCloudPhoto.png : Wordcloud
6. /WordCount.java : MapReduce program to obtain the wordcount
7. /WordCountTweet.jar : Jar corresponding to WordCount.java

**How to Run:**
1. Put the 'input' folder from folder in hdfs using the command : hdfs dfs –put ~/input/ ~/
2. Run the jar 'WordCOuntTweets.jar' using the command: hadoop jar WordCountTweets.jar WordCount ~/input ~/output1
3. The output will be stored in ~/output1 in hdfs.
4. To get the output1 folder into local current directory : hdfs dfs –get ~/output1
5. To view the output on terminal : hdfs dfs -cat ~/output1/part-r-00000

**Run the WordCloud visualization code:**
1. Open jupyter and access the 'WordCloud.ipynb' present in /Ancillary/Part1/
2. Check if the input file 'MR_Output.csv' is present in the same folder as 'WordCloud.ipynb'
3. Run the notebook cell by cell to view the input.