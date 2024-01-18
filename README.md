# TimeComplex

This package was created to evaluate functions for time complexity. The function runs an algorithm over and over with randomized input sizes to judge the time complexity.
PYPI:
<https://pypi.org/project/SpaceTimeComplex/>

## Example

```python

import SpaceTimeComplex

def looper(today,stringer):
    for x in range(today):
        print(x)
    
    for y in stringer:
        print(y)

def testone(n):
    for x in range(len(n)):
        for y in range(len(n)):
            for z in range(len(n)):
              two = y
              one = x
              three = z


real = SpaceTimeComplex.RealTime() # Create the class

testSet = real.generateTestSet() #generate a test set

testSet1 = [[4,"stnr=gwege"], [12,"sagsdgg"], [3,"esfsfsseafesfsefsef"], [45,"stnrefgseege"], [17,"sagwetjtwfwe"], [34,"esfsfssem"],[41,"stn"], [53,"sakhhksdgg"], [24,"esjfjkkfsefsef"], [70,"stnwete"], [7,"sagwefwewsdfsdffwe"], ] 
# format of array. 2d array with each test set inside. You can make your own or just generate one with generateTestSet(). Each inner array is the postional arguements for the inserted argument.

real.complexGuess(looper,testSet1) #guess the complexity of a function. Returns the guess and a plot

```

![Figure_1](https://github.com/hodge-py/SpaceTimeComplex/assets/105604814/bfe0246f-ac30-418b-b171-48bb1e3093ce)

![Screenshot 2024-01-16 010936](https://github.com/hodge-py/SpaceTimeComplex/assets/105604814/0521a2d7-9254-47f2-8b6f-d408038e33b1)

## Example of the non-log function graphed. Green $O(n^{.94})$ and red $O(n^{2.7})$

![grapher](https://github.com/hodge-py/SpaceTimeComplex/assets/105604814/0c784075-e11a-4c7c-9721-7e534353cba9)

This is in respects to time (ms). When accounting for just the growth of input, the inputs will increase in a linear and polynomial fashion.

## Jupyter Lab

The package can also be used in jupyter notebooks.
