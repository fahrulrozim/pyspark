# pyspark and Data Visualization with Google Data Studio

This is a repository for `Session 5 - Data Engineer Fellowship Program By IYKRA`. The topic in this session is `Data Visualization and Introduction to Batch Processing`.

In data visualization, we used Google Data Studio as a way to create dashboard for our data visualization. The project that I'm doing is using `Green Taxi Trip Data` from this [link](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page). For the sake of simplicity, I'm just taking the data from `green taxi in August 2021`. If you want to access the dashboard that I created, you can move to link below.

Link to Google Data Studio for `Green Taxi Trip Data` : [Google Data Studio](https://datastudio.google.com/reporting/ea4344dc-6fd1-44b4-b7b5-fb1bdcf9f1b6).

Tutorial to install pyspark:
In this step, we will discover how to install pyspark and print it's version in our jupyter notebook later. Since I'm using windows version, I'll just describe how to install it from windows version. I'll update for Linux and Mac when I have the time later.

Requirements:
1. Java 8 or later
2. Python 3.7 or later
3. Jupyter notebook

## Install Java 8 or later
Before we begin with pyspark, we have to install Java 8 or later in your computer. You can download the Java version from [Oracle](https://www.oracle.com/java/technologies/downloads/#java8) and install it to your system. If you already have java installed and don't know what version it is, simply check it with command `java -version` or `javac -version` in your terminal.
If it's your first time in installing java, then you have to set up `environment path` first.

Set your Java path with this:
`JAVA_HOME = C:\Program Files\Java\jdk1.8.0_201`

`PATH = %PATH%;C:\Program Files\Java\jdk1.8.0_201\bin`

## Install Pyspark
First, you have to install python. I recommend to download `Anaconda Navigator` or `Anaconda Prompt` since it comes with a set of `python` and `jupyter notebook`. The link to get Anaconda can be clicked [here](https://www.anaconda.com/products/distribution). After installation, don't forget to set up your `environment path` or at least confirm if it's already set. To do that, you can check by typing `python` in command prompt terminal and you should be able to see your python version and start to code python. In case it didn't work, you can see this [tutorial](https://initialcommit.com/blog/python-is-not-recognized-as-an-internal-or-external-command) to solve the problem.

Next, download pyspark by getting `.tgz` file from [spark download](https://spark.apache.org/downloads.html) page. You can unzip it with 7-zip or any other extractor file. After that, copy the extracted folder to `c:\apps` and set environment variables with:

`SPARK_HOME  = C:\apps\spark-3.0.0-bin-hadoop2.7`

`HADOOP_HOME = C:\apps\spark-3.0.0-bin-hadoop2.7`

`PATH=%PATH%;C:\apps\spark-3.0.0-bin-hadoop2.7\bin`

Remember to change the path based on your spark version and after successfully setting up environment variables, install `winutils.exe` on your windows system. You can get that [here](https://github.com/steveloughran/winutils/blob/master/hadoop-2.7.1/bin/winutils.exe) and copy it to `%SPARK_HOME%\bin` folder. Note that winutils is different for each Hadoop version and you can download the right version from this [link](https://github.com/steveloughran/winutils).

Now you can open pyspark by typing `pyspark` on your `command prompt` or `anaconda prompt`. To access web UI, it will be set as default `https://localhost:4040`, note that if you close your command prompt you can't open the web UI.

## Pyspark with jupyter notebook
Now after pyspark running successfully, you can open jupyter notebook and start working on it. Running pyspark commands will still throw an error (as it does not know which cluster to use) and in that case you have to use python library called `findspark` and use the following commands on your jupyter notebook:

`import findspark`

`findspark.init()`

If you want to check how to use pyspark, you can find it in my version check ipynb to check version and I'll add some links in case you have trouble installing it.
1. [Setup pyspark datamics](https://blog.datamics.com/how-to-install-pyspark-on-windows-faf7ac293ecf).
2. [Setup pyspark sparkbyexamples](https://sparkbyexamples.com/pyspark/how-to-install-and-run-pyspark-on-windows/).
