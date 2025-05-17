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

I used the RAND version but the code applied to the original datasets just
note that capitalization is different between the two datasets.

Health and Retirement Study, (RAND HRS Longitudinal File 2022 (V1)) public use dataset. Produced
and distributed by the University of Michigan with funding from the National Institute on Aging (grant numbers
NIA U01AG009740 and NIA R01AG073289). Ann Arbor, MI, (May 2025).


RAND HRS Longitudinal File 2022 (V1). Produced by the RAND Center for the Study of Aging, with
funding from the National Institute on Aging and the Social Security Administration. Santa Monica, CA (May
2025).

https://hrs.isr.umich.edu/data-products
