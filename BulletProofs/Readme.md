There is only one thing that we need to know for the entirety of this module

_Every Number can be represented as an Inner product of Two Vectors_

and also 

v|=[0,2**n)

Example:
5=<[1,0,1],[2**2,2**1,2**0]>
5 equals inner product of 2 vectors [1,0,1] and [2**2,2**1,2**0]

You might have notice that this is also how binary kinda works

5=101=>2^2+0*2^1+1^2^0

Lets take an example 

Lets prove that 5 is in the range of 0 to 2 ^ n _without showing 5_
from the previous example you know we Need atleast 3 bits to represent 5 
2^3=8
Therefore it's clear that 5 must be in the range of 0 to 2^n

Range proofs:
for a value v 
v=<a,2^n>
We need to prove that :
1)The assignment of a is correct 
2)We can commit to pederson commitments


