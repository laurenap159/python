# Problem 1

#### Calculate pi using Leibniz Method : pi/4 = 1/1 - 1/3 + 1/5 - 1/7 + 1/9 ...



Answer in Python \(just copied from some super old notes--not sure if correct\)

```
def LeibnizPi(terms):
    pi = 0
    for i in range(1, terms + 1):
        pi = pi + 1 / ( (2*i-1) * (-1)**(i-1))
    return pi * 4

LeibnizPi(10000)
```

returns: 3.1414926535900345

remember this value isn't exact since we put in a loop that runs 10,000 times

