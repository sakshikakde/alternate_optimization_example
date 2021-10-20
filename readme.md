# Alternate Optimization using Pytorch
This a python notebook to understand alternate optimization approach for a simple function in two variables.
## References
1) Pytorch as general optimizer: https://towardsdatascience.com/how-to-use-pytorch-as-a-general-optimizer-a91cbf72a7fb
2) Alternate minimization problem: https://kusemanohar.info/2019/10/15/alternating-minimization/

## Problem
We need to minimize a function f(x, y) for x and y defines as follows
```math
f(x, y) = 2*x^2 + 2*x*y + 2*y^2 - 6y
```
## Solution
### Numerical solution
The solution is      
```math
x = 2    
y = -1    
f(x, y) = -6
```
Refer reference 2) for details.
### Alternate mimimization
1) Initialize a value of x
2) For the fixed value of x, optimize f(x, y) for y(keeping x constant)
3) For the optimzed value of y(y*), optimize f(x, y) for x(keeping y* constant)
#### Obtained solution
```
x =  2.0051544      
y =  -1.1908405       
f(x, y) = -5.9291       
```
As we can see, the solution is quite accutate as compared to the numerical solution.
