[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)


resp = nsfg.ReadFemResp()
hist = thinkstats2.Hist()

for x, y in preg_map.items():
    if len(y) >= 2:
        pd1 = preg.loc[y[0:2]].prglngth
        pd2 = np.diff(pd1)[0]
        hist[pd2] += 1

thinkplot.Hist(hist)
pmf = thinkstats2.Pmf(hist)
pmf

pmf.Mean()