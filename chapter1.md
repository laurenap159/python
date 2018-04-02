# Problem 0

#### Determine if input is near 100.

Cases to remember:

* negative values
* if near 100, what to do?
* less than nearest hundred
* greater than nearest hundred

Answer in Python \(just copied from some super old notes--not sure if correct\)

```
x = int(input("Please enter value to test if near hundred: "))
y = 100
remainder = x % y
print (remainder)

if (remainder >= 0 and remainder < 10 and x >= 90 or remainder > 90 and remainder <= 99 and x >= 90 ):
    isNearHundred = True

else: 
    isNearHundred = False

print (isNearHundred)
```



