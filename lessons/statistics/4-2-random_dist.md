[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

random_pmf_array = np.random.random(1000)

thinkplot.pmf(thinkstats2.Pmf(random_pmf_array), linewidth = 0.1)
thinkplot.Config(xlabel = "Random variate", ylabel = "PMF")

thinkplot.cdf(thinkstats2.Cdf(random_pmf_array))
thinkplot.Config(xlabel = "Random variate", ylabel = "CDF")
