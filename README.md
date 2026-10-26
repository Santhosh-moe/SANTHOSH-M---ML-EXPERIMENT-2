## DATE : 01/09/2026







## AIM: 






Compute descriptive statistics and empirical probabilities; generate samples from 
distributions. 







## ALGORITHM (brief): 







Use pandas.Series for statistics; numpy.random for sampling.







## THEORY: 







Descriptive statistics and sampling basics used throughout ML.








```

## INPUT :


# EXPRIMENT 2
import numpy as np
import pandas as pd
heights = np.array([160,165,170,180,155,168,172,169,158])
s = pd.Series(heights)
print("Mean:", s.mean())
print("Median:", s.median())
print("Std dev:", round(s.std(),3))
print("Variance:", round(s.var(),3))
print("P(height> 170):", (s>170).mean())
sample = np.random.normal(loc=s.mean(), scale=s.std(), size=10)
print("Random sample (10) from normal around mean:", np.round(sample,2))



## OUTPUT :


Mean: 166.33333333333334
Median: 168.0
Std dev: 7.762
Variance: 60.25
P(height> 170): 0.2222222222222222
Random sample (10) from normal around mean: [176.88 166.19 164.79 167.15 159.1  175.4  172.78 170.16 162.91 159.06]



```





## RESULT


Students learn central tendency, spread, and simple empirical probability estimation.
