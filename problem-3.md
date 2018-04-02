# Problem 3

#### Calculate pi using Archimedes Method : cir = 2pi\*r



Answer in Python \(just copied from some super old notes--not sure if correct\)

```
#Archimedes approach C=2pi*r
import math

def archimedesPi(num_sides):
    r=1
    #if r=1, the pi = c/2
    #approximate c using the circumference of a polygon with many sides
    #cir of poly = # sides * side length
    
    theta = (math.radians(360)) / (2 * num_sides )
    
    side = 2 * (math.sin(theta))
    
    piCircum = (num_sides * side) / 2
    
    print (piCircum)
    
archimedesPi(10000)
```

returns: 3.141592601912665

Remember this value isn't exact since we put in a loop that runs 10,000 times

