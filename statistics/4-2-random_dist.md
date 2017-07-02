[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> 

import numpy as np
randnum = np.random.random(1000)

pmf = thinkstats2.Pmf(randnum)
thinkplot.Pmf(pmf, linewidth=0.1)

CDF = thinkstats2.Cdf(randnum)
thinkplot.Cdf(CDF)

