# CS450 Assignment 2 Jiadong Hong

## Part 1 Theoretical Problems

### Question 1

![image-20231031123919179](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031123919179.png)
$$
C_1 = \{[1,3,2]^T\}\\
C_2 = \{[1,4,7]^T, [2,5,8]^T\}
$$

### Question 2

**In general, for any vector x, does it hold that **
$$
∥x∥_1 ≥ ∥x∥_2 ≥ ∥x∥_∞
$$
Since the concept of the norm is: 

![image-20231031124916494](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031124916494.png)

**Proof:** Let x be an arbitrary vector. 

**∥x∥₁ ≥ ∥x∥∞:** 

The L₁ norm (∥x∥₁) is defined as the sum of the absolute values of the vector's components. 

The L∞ norm (∥x∥∞) is defined as the maximum absolute value of any component in the vector. 

Since the sum of absolute values is always greater than or equal to the maximum absolute value, we have ∥x∥₁ ≥ ∥x∥∞. 

**∥x∥₂ ≥ ∥x∥∞:**

The L₂ norm (∥x∥₂) is defined as the square root of the sum of the squares of the vector's components. 

The L∞ norm (∥x∥∞) is still defined as the maximum absolute value of any component in the vector. 

Since the square root of a positive value is always greater than or equal to the value itself, we have ∥x∥₂ ≥ ∥x∥∞. Hence, for any vector x, ∥x∥₁ ≥ ∥x∥₂ ≥ ∥x∥∞.

**QED**

### Question 3

![image-20231031125415115](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031125415115.png)

![1b8fd3ee836c73b7b6e6ebbb4be4e4d](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\1b8fd3ee836c73b7b6e6ebbb4be4e4d.jpg)

### Question 4

![image-20231031135749642](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031135749642.png)

![](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031135759308.png)

![94a3dd01c796bcbcc8ada3a3ea717c6](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\94a3dd01c796bcbcc8ada3a3ea717c6.jpg)



![697334bd70a8b3a8736498afb06e03c](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\697334bd70a8b3a8736498afb06e03c.jpg)

**（e）**

![60a7f336ee0946440ef1a3b6795b807](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\60a7f336ee0946440ef1a3b6795b807.jpg)

### Question 5

![image-20231031195525204](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231031195525204.png)

![982af74f4c9c78c19b848a91886ddc1](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\982af74f4c9c78c19b848a91886ddc1.jpg)

![image-20231102190159481](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102190159481.png)

![4027c15790bed8305dac3bf16074105](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\4027c15790bed8305dac3bf16074105.jpg)

![237caa56d5828b4ced860792b9cc851](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\237caa56d5828b4ced860792b9cc851.jpg)

![image-20231102190213205](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102190213205.png)

![67216d592f3f4b34393d14bf89f7c7c](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\67216d592f3f4b34393d14bf89f7c7c.jpg)

![image-20231102190104893](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102190104893.png)

![b8c4dc0fa3d6fc0bd38604f16cb0567](C:\Users\Jiadong Hong\Documents\WeChat Files\wxid_8u2i17dq6v7v22\FileStorage\Temp\b8c4dc0fa3d6fc0bd38604f16cb0567.jpg)

## Part 2: Programming Problems

![image-20231102193354100](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102193354100.png)

det(A) = 0

The determinant of matrix A is equal to 0, which means that A is singular. 

When a matrix is singular, it implies that the system of linear equations Ax = b may have infinitely many solutions or no solution at all, depending on the specific values of b.

b = [0.1] [0.3] [0.5]

Since A is singular, there are either no solutions or infinitely many solutions to the system Ax = b, depending on whether the vector b is in the column space of A.

In this case, we can represent b as a linear combination of the columns of A (assuming it's possible):

b = 0.1 * [0.1] + 0.3 * [0.4] + 0.5 * [0.7]

This equation is consistent, which means that there are infinitely many solutions to the system Ax = b. In other words, there are infinitely many x vectors that satisfy the equation Ax = b. These x vectors can be found by varying the weights (0.1, 0.3, and 0.5) in the linear combination above.

![image-20231102194151788](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102194151788.png)

(b) Numerical Instability: In exact arithmetic, Gaussian elimination should theoretically work for non-singular matrices. However, in practice, especially with large or ill-conditioned matrices, it might suffer from numerical instability due to the accumulation of round-off errors, especially when the pivots are very small relative to other matrix elements.

(c)

![image-20231102213728277](C:\Users\Jiadong Hong\AppData\Roaming\Typora\typora-user-images\image-20231102213728277.png)

The condition number of this system is actually too large to convince the answer is correct.