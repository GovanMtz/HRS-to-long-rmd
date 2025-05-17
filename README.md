# HRS-to-long-rmd
The Health and Retirement Study is not instantly user-friendly in R, even though the RAND products are not in perfect ready-to-use condition. 
This RMD aims to make using this dataset as panel data easier.

I was motivated to do this mini data cleaning project as using this dataset is very easy in Stata, however, it is not so easy to use in 
R or Python. In Stata I was even struggling to load the HRS dataset due to it being so large. For reference the stata code that accomplishes what
I wanted to do in R is the following:

```{stata}
reshape long r@shlt, I(hhidpn)
j(wave)
```

Most people using this dataset are using Stata, and tutorials on how to clean the data simply said 
the dataset could not easily be used in R. While I don't think what I have provided is the most efficient way to reshape
this dataset the code has still been helpful to me as I can at least load the data into R while Stata runs out of memory on my laptop.
