# Mixture Models and EM

Date: 2019/12/18

## Logic
1. A joint distribution $P(x,y)$ over **observed and latent variables**\
   $P(x) = \sum_{y}P(x|y)P(y)$\
   $x$ - observed\
   $y$ - latent (continuous, discrete)
2. Gaussian Mixture can be interpreted in terms of **discrete** latent variables.
3. Mixture Models
   - more complex probability distributios
   - cluster data\
     $J = \sum_{n=1}^N\sum_{k=1}^Kr_{nk}\|\mathbf{x}_n-\mathbf{\mu}_k\|^2$
4. Iteration - find the $r_{n,k}$ and $\mathbf{\mu}_k$\
   two-stage optimization



### What is K-means?


### What's the realtionship of K-means and EM-GMM?


## Some details
1. 1-of-K coding scheme\
   $r_{nk} \in \{0,1\}$, \
   if data point $\mathbf{x}_n$ is assigned to cluster $k$, $r_{nk} = 1$; otherwise $r_{nk} = 0$.

## To be explored
1. Bayesian treatment using the framework of variational inference.\
   The number of components $K$ in the mixture could be inferred **automaticallly from the data**. 
2. 
    




## Reference
1. Bishop, Christopher M. 
   Pattern recognition and machine learning. 
   springer, 2006.
2. 