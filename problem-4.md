# Problem 4

#### Calculate pi using Randomness Method

Methodology: place a square on a place \(it's area is defined in the function\). Place a circle just within that square. Randomly place dots \(random coordinates\) within the square. Determine how many of those dots are inside the circle and how many outside. This will give you the area of the circle 

Answer in Python \(just copied from some super old notes--not sure if correct\)

```
#approximate pi using randomness
import random
def randomnessSimulation(number_points):
    
    area_of_square = 4
    points_in_circle = 0
    
    for i in range(number_points):
        x = random.uniform(-1,1)
        y = random.uniform(-1,1)
        
        if math.sqrt(x**2 + y**2) <= 1:
            points_in_circle += 1
    
    area_of_circle = (points_in_circle / number_points) * area_of_square
        
    print (area_of_circle)
    
randomnessSimulation(10000)
```

returns: 3.16

