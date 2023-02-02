Strassens multiplication is a recursive algorithm for multiplying n*n matrices ( here , 2*2 matrices)
The time complexity for :
1) Strassens multiplication --> O(n^2.8) . 
2) Matrix multiplication --> O(n^3) . 
 
The time complexity is less compared to matrix multiplication . 
There will be 2 matrix A and B , to calculate A X B , we need to calculate using seven multiplications .
The seven multplications are : 
1) p1 = a * (f - h )
2) p2 = (a + b ) * h  
3) p3 = (c + d ) * e  
4) p4 = d * (g - e)
5) p5 = (a + d)*(e + h)
6) p6 = (b - d)* (g + h)
7) p7 = (a - c ) * (e + f)
 
To calculate Matrix C (also known as A X B) :

r = p5 + p4 - p2 + p6

s = p1 + p2 

t = p3 + p4 

u = p5 + p1 - p3 - p7


![GDB online Debugger _ Compiler - Code, Compile, Run, Debug online C, C++ - Google Chrome 02-02-2023 14_08_48](https://user-images.githubusercontent.com/72621930/216273393-06735d72-94c3-42c0-a6b8-d29ce3856928.png)

