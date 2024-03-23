Lets say we have an equation which is 

x*y +4 = 10

Our first constraint is 

output1==x*y

Our second constraint is 

output2 == output1 + 4

And our third constraint is 

Equality constraint i.e ==10


We can tell now that every equation has a left-input a right input and a output 

Such that 
left(L)*right(R)=Output(O)
With three vectors 
We get <L,v>*<R,v>=<O,v>
v is the variable vector
v=[1,x,y,output]

so we can say that 

our 
constraint 1:x*y==output 

L=[0,1,0,0]//x
R=[0,0,1,0]//y
O=[0,0,0,1]//output1

and our constraint2 is((output1+4)*1=10)

L=[4,0,0,1]//output1+5
R=[1,0,0,0]//1
O=[10,0,0,0]//10

now create polynomials for each using lagrange's interpolation

L1[1]=0(look at first constraint,first element of l)
L2[1]=0(look at second constraint,first element of l)


To use Lagrange interpolation to find a polynomial that passes through two given points, (1,0) and (2,4), you would construct a polynomial of degree one less than the number of points, in this case, degree 1 because you have two points.

The general form of Lagrange interpolation for two points, given by (x0, y0) and (x1, y1), is:

\[ P(x) = y0 * \frac{x - x1}{x0 - x1} + y1 * \frac{x - x0}{x1 - x0} \]

Given your points (1,0) and (2,4), you can substitute these values into the Lagrange interpolation formula:

\[ P(x) = 0 * \frac{x - 2}{1 - 2} + 4 * \frac{x - 1}{2 - 1} \]

Simplifying:

\[ P(x) = 0 * (x - 2) + 4 * (x - 1) \]
\[ P(x) = 4x - 4 \]

So, the Lagrange polynomial passing through the points (1,0) and (2,4) is \( P(x) = 4x - 4 \).



