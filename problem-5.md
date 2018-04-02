# Problem 5

#### Calculate pi using Wallis with a given tolerance for the answer value

This means that the program will continue to loop until the difference between the last calculated value and the present calculated value are less than the input tolerance. 

This is probably an EXCELLENT interview question since it tests knowledge of loops and logical definitions. 

Answer in Python \(just copied from some super old notes--not sure if correct\)

```
def WallisPi(tolerance):
    halfPi = 1
    i = 0
    difference = 1
    while difference > tolerance:
        oldHalfPi = halfPi
        halfPi = halfPi * (2*(i+1))**2 / ((2*i+1)*(2*i+3))
        difference = abs(halfPi - oldHalfPi)
        i=i+1
    print("iterations: ", i)
    return halfPi*2

WallisPi(.0000001)
```

Returns: iterations:  1982

                3.141196513041758



Remember this value isn't exact since we put in a loop that runs until a tolerance of .0000001 is reached

