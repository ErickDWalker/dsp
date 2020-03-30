[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

**1. Investigate whether first babies are lighter or heavier than others**
first_weight = live[live["birthord"] == 1]["totalwgt_lb"]
other_weight = live[live["birthord"] != 1]["totalwgt_lb"]

first_mean_weight = first_weight.mean()
other_mean_weight = other_weight.mean()

print("First mean weight:", first_mean_weight)
print("Other mean weight:", other_mean_weight)

Output: First mean weight: 7.201094430437772
Other mean weight: 7.325855614973262

**First babies' mean weight is lower than the mean weight of babies born later**

**2. Cohen's effect size on weight**
CohenEffectSize(first_weight, other_weight)

**3. Difference in pregnancy length for first baby vs other babies**
Cohen's effect size is 0.0289 for pregnancy length of first baby vs others, which is a smaller effect size than that seen for
weight of first baby vs others (-0.0886).



