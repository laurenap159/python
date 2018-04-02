# Problem 2

#### Calculate pi using Wells Method : pi/2 = 2/1 \* 2/3 \* 4/3 \* 4/5 \* 6/5 \* 6/7 \* 8/7 \* ...



Answer in Python \(just copied from some super old notes--not sure if correct\)

```
def WellsFormula (terms):
    pi = 1
    for i in range (1, terms):
        pi = pi * (2*i)**2 / ( (2*i - 1) * (2*i + 1))
    return pi * 2
WellsFormula(1000000)
```

returns: 3.141591868191682

Remember this value isn't exact since we put in a loop that runs 1,000,000 times

