# Creating a JackKnife Function in R



In your pre-class work you have created the following function: 


## Jackknife of the Mean!

- Have an estimator \(\hat{\theta}\) of parameter $\theta$  
  want the standard error of our estimate, $se_{\hat{\theta}}$
- The jackknife approximation:
    + omit case $i$, get estimate $\hat{\theta}_{(-i)}$
    + Take the variance of all the $\hat{\theta}_{(-i)}$
    + multiply that variance by $\frac{(n-1)^2}{n}$ to get $\approx$ variance of $\hat{\theta}$
- then $se_{\hat{\theta}}=$ square root of that variance



Your goal for this lab will be to extend the concept of `mean.jackknife`, so that it works in more situations than just the mean. 