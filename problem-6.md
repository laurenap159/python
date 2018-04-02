# Problem 6

#### Encrypt a string by shifting every character 2 places then decrypt that string

Answer in Python \(just copied from some super old notes--not sure if correct\)

```
def encrypt(someString):
    
    firstPart = ''
    secondPart = ''
    
    for i, letter in enumerate(someString):
        if i % 2 == 0:
            firstPart += letter
        else:
            secondPart += letter
            
    finalOutput = firstPart + secondPart
    return finalOutput
    
encrypt('comehere')
```

Returns: 'cmhroeee'

```
def decrypt(someString):
    
    firstPart = ''
    secondPart = ''
    finalOutput = ''
    
    middle = (len(someString) + 1) // 2
    firstHalf = someString[:middle]
    secondHalf = someString[middle:]  
    
    for i, letter in enumerate(someString[:middle]):
        #finalOutput += someString[i]
        #finalOutput += someString[i + middle]
        
        #add position i from first string to final Output
        finalOutput += firstHalf[i]
        #add position i from second string to final Output
        finalOutput += secondHalf[i]
    
    return finalOutput
    
decrypt("cmhroeee")
```

Returns: 'comehere'

