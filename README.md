# Shapelet-Cluster
Unsupervised Learning clustering technique is implemented in order to label a given unlabeled dataset.
Output of the implementation will provide a classify each time instance of a multivariate time series dataset. 
采用无监督学习聚类技术对给定的未标记数据集进行标记。
实现的输出将为多元时间序列数据集的每个时间实例提供分类。

# How to run
## EuclideanV1.1.py script
Function named cluster_algo(r,c,eps,min_pts,dataset_name) has to be called passing the necessary parameters.
  r - Number of rows of the total dataset
  c - Expected number of events/clusters the multivariate time series is expected to be clustered to
  eps - maximum radius to be considered with respect to a given data point in defining cluster boundary
  min_pts - minimum number of points within a cluster
  dataset_name - provide the obtained dataset file name
  函数cluster_algo(r,c,eps,min_pts,dataset_name)必须通过调用必要的参数。
  r -总额的数据集的行数
  c -预期的事件数量/集群多元时间序列将集群
  eps -最大半径被认为是对一个给定的数据点在定义集群边界
  min_pts -最小数量的点在一个集群
  dataset_name提供获得数据集文件的名字
  
## cluster_accuracy.py script
Function named cluster_accuracy(input_file_with_clusters,output_file_with_stats) has to be called passing the necessary parameters.
必须调用名为cluster_accuracy的函数(input_file_with_clusters,output_file_with_stats)并传递必要的参数。  

# Important
The technique only facilitates numeric datasets
The accuracy of the clustering technique will be varied upon the values passed for eps, min_pts
该技术只方便数值数据集
根据eps、min_pts传递的值，聚类技术的准确性会有所不同

# Testing
In order to test the approach we have used following labeled datasets and prepared the dataset file without the annotated column
and compared the results obtained from our implementation against the actual annotation.
  Occupancy Detection Dataset - https://archive.ics.uci.edu/ml/datasets/Occupancy+Detection+
  EEG-Eye State Dataset - https://archive.ics.uci.edu/ml/datasets/EEG+Eye+State
为了测试这种方法，我们使用了以下标记的数据集，并准备了不带注释列的数据集文件
并将我们实现的结果与实际注释进行了比较。
