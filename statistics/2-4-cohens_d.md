[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

#REPLACE THIS TEXT WITH YOUR RESPONSE
firsts.totalwgt_lb.mean(), others.totalwgt_lb.mean()

CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)

resp = nsfg.ReadFemResp()
list(resp)


hist = thinkstats2.Hist(resp.totincr)
thinkplot.Hist(hist, label='totincr')


hist = thinkstats2.Hist(resp.age_r)
thinkplot.Hist(hist, label='age_r')

hist = thinkstats2.Hist(resp.numfmhh)
thinkplot.Hist(hist, label='numfmhh')

hist = thinkstats2.Hist(resp.parity)
thinkplot.Hist(hist, label='parity')

hist.Largest(10)

NHiInc = resp[resp.totincr < 14]
HiInc.parity.mean(), NHiInc.parity.mean()

#much higher effect size
CohenEffectSize(HiInc.parity, NHiInc.parity)