# local-spark-cluster

### Requirements

* docker
* docker-compose

### Usage

```
$ git clone https://github.com/rodolfoap/local-spark-cluster.git

$ cd local-spark-cluster

$ docker-compose up -d

$ docker exec -it spark-master bash

$ I have no name!@0ebee434f2d7:/opt/bitnami/spark$ spark-shell

Setting default log level to "WARN".
To adjust logging level use sc.setLogLevel(newLevel). For SparkR, use setLogLevel(newLevel).
24/11/14 14:35:23 WARN NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable
Spark context Web UI available at http://0ebee434f2d7:4040
Spark context available as 'sc' (master = local[*], app id = local-1731594923602).
Spark session available as 'spark'.
Welcome to
      ____              __
     / __/__  ___ _____/ /__
    _\ \/ _ \/ _ `/ __/  '_/
   /___/ .__/\_,_/_/ /_/\_\   version 3.5.3
      /_/

Using Scala version 2.12.18 (OpenJDK 64-Bit Server VM, Java 17.0.13)
Type in expressions to have them evaluated.
Type :help for more information.

scala> val mydata= List(("pierre", "T"), ("jeanne", "E"))
mydata: List[(String, String)] = List((pierre,T), (jeanne,E))

scala> ...
```
