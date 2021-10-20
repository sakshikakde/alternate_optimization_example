# Alternate Optimization using Pytorch
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
f(2, -1) = -6
```
Refer reference 2) for details.
### Alternate mimimization
1) Initialize a value of x
2) For the fixed value of x, optimize f(x, y) for y(keeping x constant)
3) For the optimzed value of y(y*), optimize f(x, y) for x(keeping y* constant)


