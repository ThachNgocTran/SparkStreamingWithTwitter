# Spark Streaming With Twitter
In Spark Summit 2014 [2], there was a hand-on exercise on Streaming with Twitter. I am reproducing this exercise using the latest versions at present (May-2016).

This is the (almost) complete source code (I finished the missing part "Your code goes here" in the exercise). All one needs to do now is to fill in Twitter's credentials [6]. The library dependencies (Twitter4J, spark-streaming-twitter) are also included here for convenience.

There are two ways to reproduce:

* By Intellij: Open the project (*.iml), reference to "spark-assembly-1.6.1-hadoop2.6.0.jar", 3rd party libraries (spark-streaming-twitter_2.10-1.6.1.jar, twitter4j-async-4.0.4.jar, twitter4j-core-4.0.4.jar, twitter4j-examples-4.0.4.jar, twitter4j-media-support-4.0.4.jar, twitter4j-stream-4.0.4.jar). Then Run.

* By Command Line: Build the artifact (SparkStreamingWithTwitter.jar), then use the command: spark-submit.cmd --class "Tutorial" --jars "spark-streaming-twitter_2.10-1.6.1.jar,twitter4j-async-4.0.4.jar,twitter4j-core-4.0.4.jar,twitter4j-examples-4.0.4.jar,twitter4j-media-support-4.0.4.jar,twitter4j-stream-4.0.4.jar" "SparkStreamingWithTwitter.jar".

Note: In case those additional jars cannot be found, use absolute paths!

## Software Environment:

* Apache Spark v1.6.1

* IntelliJ IDEA Community Edition 2016.1.2 (with Scala plugin)

* Scala v2.10.5

* Java SDK v1.8.0_92 64-bit

* spark-streaming-twitter_2.10-1.6.1.jar [5]

* Twitter4J v4.0.4 [4]

* Windows 8.1 64-bit

## References:

1. [Spark Streaming Programming Guide v1.6.1](http://spark.apache.org/docs/1.6.1/streaming-programming-guide.html)

2. [Spark Summit 2014 Training Archive](https://spark-summit.org/2014/training)

3. [Hands-on Exercises](https://databricks-training.s3.amazonaws.com/index.html)

4. [Twitter4J](http://twitter4j.org/en/index.html)

5. [spark-streaming-twitter_2.10-1.6.1](http://search.maven.org/#search%7Cga%7C1%7Ca%3A%22spark-streaming-twitter_2.10%22)

6. [Twitter Apps](https://dev.twitter.com/apps)
