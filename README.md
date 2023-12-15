# BSE_DSM_Statisctic_project



## PROJECT OUTLINE:

### Data summary 

n ~ 450 
d ~ 100

X1 X2 ... Xt

Input data from fred:

will list all sources and describtions here
...

y1 y2 ... yt

Target y = log(BASKET_px(t)) - log(BASKET_px(t-1))


split 20% for test
Random Intervals as Test set, should be fine even tho we have a Timeseries (we only predict 1 timestamp m/m)




Problem: Very high correlation in Covariates
Problem: We have an autocorrelated timeseries, but put yt-1 as one of our input features for Xt should fix that 



## Part 1:
    Ols 
    Lasso with CV
    Ridge with CV
    Adaptive Lasso with CV
    Lasso with EBIC
    
    BMA
    Test all models on our test set
    
    
    
## Part 2:
    Use PCA and GMMs for dim reduction
    
    5 - 50 K for GMM 
    
    Try best method from part 1 again
