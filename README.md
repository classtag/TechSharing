# TechSharing
## Unlock Spark from A to Z
“Big data" analysis is a hot and highly valuable skill – and this series will discuss with you the hottest technology in big data: Apache Spark. More and more teams are using Spark to quickly extract meaning from massive data sets across a fault-tolerant Hadoop cluster.

What Shall We Discuss together?

- Frame big data analysis problems as Apache Spark scripts
- Develop distributed code using the Scala programming language 
- Optimize Spark jobs through partitioning, caching, and other techniques
- Build, deploy, and run Spark scripts on EMR clusters
- Process continual streams of data with Spark Streaming
- Transform structured data using SparkSQL and DataFrames
- It maybe the first time to know these topics, but you really don't need to prepare too much, it's easier than you might think.

Learn and master the art of framing data analysis problems as Spark problems through over 20 hands-on examples, and then scale them up to run on cloud computing services in this course.

- Learn the concepts of Spark's Resilient Distributed Datastores
- Get a crash course in the Scala programming language
- Develop and run Spark jobs quickly using Scala
- Translate complex analysis problems into iterative or multi-stage Spark scripts
- Scale up to larger data sets using Amazon's Elastic MapReduce service
- Understand how Hadoop YARN distributes Spark across computing clusters
- Practice using other Spark technologies, like Spark SQL, DataFrames, DataSets, Spark Streaming
- By the end of this series, we'll be running code that analyzes gigabytes worth of information – in the cloud – in a matter of minutes. 

We'll have some fun along the way. You'll get warmed up with some simple examples of using Spark to analyze movie ratings data and text in a book. Once you've got the basics under your belt, we'll move to some more complex and interesting tasks. We'll use a million movie ratings to find movies that are similar to each other, and you might even discover some new movies you might like in the process!

This series is very hands-on; you'll spend most of your time following along with the instructor as we write, analyze, and run real code together – both on your own system, and in the cloud using Amazon's Elastic MapReduce service. With over 20 real examples of increasing complexity you can build, run and study yourself. Move through them at your own pace, on your own schedule. The series wraps up with an overview of other Spark-based technologies, including Spark SQL, Spark Streaming, and MLLib.

Enjoy it!

You need to know

Some prior programming or scripting experience is required.
A crash course in Scala is included, but you need to know the fundamentals of programming in order to pick it up.

### Sessions
![image](https://raw.githubusercontent.com/classtag/TechSharing/master/spark-overview.png)

#### Getting Started
![image](https://raw.githubusercontent.com/classtag/TechSharing/master/getting-started.png)

- **Introduction, and Getting Set Up**
A brief introduction to the course, and then we'll get your development environment for Spark and Scala all set up on your desktop. A quick test application will confirm Spark is working on your system! Remember - be sure to install Spark 2.0.0 or newer.

- **Create a Histogram of Real Movie Ratings with Spark!**
Let's dive right in! We'll download a data set of 100,000 real movie ratings from real people, and run a Spark script that generates histogram data of the distribution of movie ratings. Some final setup of your Scala development environment and downloading the course materials is also part of this lecture, so be sure not to skip this one.

#### Scala Scratch
Spark works best when using the Scala programming language, and this series includes a crash-course in Scala to get you up to speed quickly.
![image](https://raw.githubusercontent.com/classtag/TechSharing/master/scala-scratch.png)
- **Scala Basics**

We'll go over the basic syntax and structure of Scala code with lots of examples. It's backwards from most other languages, but you quickly get used to it

- **Flow Control in Scala**

You'll see how flow control works in Scala (if/then statements, loops, etc.), and practice what you've learned at the end.

- **Functions in Scala**

Scala is a functional programming language, and so functions are central to the language. We'll go over the many ways functions can be declared and used in Scala, and practice what you've learned.

- **Data Structures in Scala**
We'll cover the common data structures in Scala such as Map and List, and put them into practice.

#### Spark Basics and Simple Examples
![image](https://raw.githubusercontent.com/classtag/TechSharing/master/spark-basics.png)
- **Introduction to Spark**

What is Apache Spark anyhow? What does it do, and what is it used for?

- **The Resilient Distributed Dataset**

The core object of Spark programming is the Resilient Distributed Dataset, or RDD. Once you know how to use RDD's, you know how to use Spark. We'll go over what they are, and what you can do with them.

- **Ratings Histogram Walkthrough**

Now that we understand Scala and have the theory of Spark behind us, we can revisit the rating counter code from lecture 2 and better understand what's actually going on within it.

- **Spark Internals**

How does Spark convert your script into a Directed Acyclic Graph and figure out how to distribute it on a cluster? Understanding how this process works under the hood can be important in writing optimal Spark driver scripts.

- **Key / Value RDD's, and the Average Friends by Age example**

RDD's that contain a tuple of two values are key/value RDD's, and you can use them much like you might use a NoSQL data store. We'll use key/value RDD's to figure out the average number of friends by age in some fake social network data.

- **Running the Average Friends by Age Example**

We'll run the average friends by age example on your desktop, and give you some ideas for further extending this script on your own.

- **Filtering RDD's, and the Minimum Temperature by Location Example**

We'll cover how to filter data out of an RDD efficiently, and illustrate this with a new example that finds the minimum temperature by location using real weather data.

- **Running the Minimum Temperature Example, and Modifying it for Maximum**

We'll run our minimum temperature by location example, and modify it to find maximum temperatures as well. Plus, some ideas for extending this script on your own.

- **Counting Word Occurrences using Flatmap()**

flatmap() on an RDD can return variable amounts of new entries into the resulting RDD. We'll use this as part of a hands-on example that finds how often each word is used inside a real book's text.

- **Improving the Word Count Script with Regular Expressions**

We extend the previous lecture's example by using regular expressions to better extract words from our book.

- **Sorting the Word Count Results**

Finally, we sort the final results to see what the most common words in this book really are! And some ideas to extend this script on your own.

- **Find the Total Amount Spent by Customer**

Your assignment: write a script that finds the total amount spent per customer using some fabricated e-commerce data, using what you've learned so far.

- **Check your Results, and Sort Them by Total Amount Spent**

We'll review my solution to the previous lecture's assignment, and challenge you further to sort your results to find the biggest spenders.

- **Check Your Results and Implementation Against Mine**

Check your results for finding the biggest spenders in our e-commerce data against my own solution.

#### Advanced Examples of Spark Programs
![image](https://raw.githubusercontent.com/classtag/TechSharing/master/advanced-spark.png)
- **Find the Most Popular Movie**
We'll revisit our movie ratings data set, and start off with a simple example to find the most-rated movie.

- **Use Broadcast Variables to Display Movie Names**
Broadcast variables can be used to share small amounts of data to all of the machines on your cluster. We'll use them to share a lookup table of movie ID's to movie names, and use that to get movie names in our final results.

- **Item-Based Collaborative Filtering in Spark, cache(), and persist()**
Back to our movie ratings data - we'll discover movies that are similar to each other just based on user ratings. We'll cover the algorithm, and how to implement it as a Spark script.

- **Running the Similar Movies Script using Spark's Cluster Manager**
We'll run our movie similarties script and see the results. In doing so, we'll introduce the process of exporting your Spark script as a JAR file that can be run from the command line using the spark-submit script (instead of running from within the Scala IDE.)

- **Improve the Quality of Similar Movies**
Your challenge: make the movie similarity results even better! Here are some ideas for you to try out.


## Mastering Concurrency Programming with Java 8
  
Mastering the principles and techniques of multithreaded programming with the Java 8 Concurrency API.

it will cover below topics:

- Concurrency Design Principles
- Managing Lots of Threads – Executors
- Getting the Maximum from Executors
- Getting Data from the Tasks – The Callable and Future Interfaces
- Running Tasks Divided into Phases – The Phaser class
- Optimizing Divide and Conquer Solutions – The Fork/Join Framework
- Processing Massive Datasets with Parallel Streams – The Map and Reduce Model
- Processing Massive Datasets with Parallel Streams – The Map and Collect
- Diving into Concurrent Data Structures and Synchronization Utilities
- Testing and Monitoring Concurrent Applications
- I split above topics into 4 parts:


### Sessions
- Part 1: Concurrency Design Principles and Executors
- Part 2: Tasks and Fork/Join
- Part 3: Parallel Streams
- Part 4: Concurrent Data Structures, Synchronization Utilities, and Testing
- Part 5: Advantage concurrent framework: Disruptor and Akka
