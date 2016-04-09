
### SparkContext

In order to use Spark and its API we will need to use a SparkContext. When running Spark, you start a new Spark application by creating a SparkContext. When the SparkContext is created, it asks the master for some cores to use to do work. The master sets these cores aside just for you; they won't be used for other applications. When using Databricks Cloud or the virtual machine provisioned for this class, the SparkContext is created for you automatically as sc.

sc = spark context

### Parallelize data using 8 partitions
### This operation is a transformation of data into an RDD
### Spark uses lazy evaluation, so no Spark jobs are run at this point
xrangeRDD = sc.parallelize(data, 8)

### Let's view the lineage (the set of transformations) of the RDD using toDebugString()
print xrangeRDD.toDebugString()
