#Differnt print statements to help with troubleshooting











## Spark
**Printing RDDs**

```
rdd.foreach(print)
```
While this will work as expected on a single machine, it could lead to some unexpected results when you are working in a cluster. Since the output to stdout is being called by the executors, they are writing to the executor's stdout and they do not appear on the driver node's stdout. You should use collect() to bring the entire RDD to the master node for printing.

 If you were to call collect() on RDDs of that size, you will most likely cause the driver node to run out of memory because the collective memory of the cluster is greater than the memory of the individual master where data is collected to.

 **Print subset of RDD (to not overload memory)**
```
print(rdd.take(100))