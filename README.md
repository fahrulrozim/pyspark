# pyspark

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
`JAVA_HOME = C:\Program Files\Java\jdk1.8.0_201
PATH = %PATH%;C:\Program Files\Java\jdk1.8.0_201\bin`

## Install Pyspark
First, you have to install python. I recommend to download `Anaconda Navigator` or `Anaconda Prompt` since it comes with a set of `python` and `jupyter notebook`. The link to get Anaconda can be clicked [here](https://www.anaconda.com/products/distribution). After installation, don't forget to set up your `environment path` or at least confirm if it's already set. To do that, you can check by typing `python` in command prompt terminal and you should be able to see your python version and start to code python. In case it didn't work, you can see this [tutorial](https://initialcommit.com/blog/python-is-not-recognized-as-an-internal-or-external-command) to solve the problem.

