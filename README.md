# Spark-program-to-find-in-degree-distribution
The in-degree of a node (or vertex), is the number of incoming links to that node. We are interested to find the in-degree distribution of the twitter graph. The in-degree probability distribution p(k) of a network is the fraction of nodes in the network with degree k. That is 𝑝(𝑘)=𝑛k/𝑛  where 𝑛𝑘 is the number of vertices with in-degree k and n is the total number of nodes in the graph .

This spark program produces a pair RDD of the form (k,p(k)) where k is an indegree and p(k) is the indegree probability for k in the twitter graph as explained above. For example an rdd element (1, 0.01) means that 1% of the nodes in the twitter graph have indegree 1

The input dataset can be downloaded from here: https://snap.stanford.edu/data/higgssocial_network.edgelist.gz and is in the following form:  
             <userid1> <userid2> 
  Where userid1 follows userid2.  
 
