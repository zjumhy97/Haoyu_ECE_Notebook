# Mixture Models and EM

Date: 2019/12/18\
Source: Reference 1 Page 440

## Logic
1. A joint distribution $P(x,y)$ over **observed and latent variables**\
   $P(x) = \sum_{y}P(x|y)P(y)$\
   $x$ - observed\
   $y$ - latent (continuous, discrete)
2. Gaussian Mixture can be interpreted in terms of **discrete** latent variables.
3. Mixture Models
   - more complex probability distributios
   - cluster data
4. Cluster also could be used in data compression


---
### What is K-means?
$J = \sum_{n=1}^N\sum_{k=1}^Kr_{nk}\|\mathbf{x}_n-\mathbf{\mu}_k\|^2$\
two-stage optimization
#### steps  two-stage optimization
1. optimize $r_{n,k}$
2. optimize $\mathbf{\mu}_k$\
   set $\mathbf{\mu}_k$ equal to the mean of all of the data points $\mathbf{x}_n$ assigned to cluster $k$.
#### properties
1. converge to a local rather than global minimum

#### Limitation
1. based on the use of squared Euclidean distance\
   case: some or all of the variables represent categorical labels
2.  make the determination of the cluster means **nonrobust** to outliers\
    K-medoids algorithm
---
### What's the realtionship of K-means and EM-GMM?


## Some details
1. 1-of-K coding scheme\
   $r_{nk} \in \{0,1\}$, \
   if data point $\mathbf{x}_n$ is assigned to cluster $k$, $r_{nk} = 1$; otherwise $r_{nk} = 0$.
2. a batch verision\
   chinese: 批处理版本

## To be explored
1. Bayesian treatment using the framework of variational inference.\
   The number of components $K$ in the mixture could be inferred **automaticallly from the data**. 
2. Robbins-Monro procedure
    




## Reference
1. Bishop, Christopher M. 
   Pattern recognition and machine learning. 
   springer, 2006.
2. 