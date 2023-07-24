# Utilizing_through_sinelaw

$$ [INTRODUCTION] $$

These are some ways to utilize sine law with 'easy and self-evident natures of a triangle'.
![삼각형](https://github.com/psjdavid/utilizing_for_sinlaw/assets/94748252/7e03b5de-c561-4964-9c60-0c6b40d92052)


$$ [UTILIZING] $$

$$1. \sin B \times c = \sin C \times b$$

$$2. \sin B : \sin C = b:c$$

For this, we can solve the Ratio between two sine values with two line values.\
If there's a question like 'c=4, b=6. Solve the ratio between sin B and sin C.', we should take account of 'sine law'first.\
Then the standard approach is like this; 

$$\frac{6}{\sin B}=\frac{4}{\sin C}$$

$$\sin C \times 6 = \sin B \times 4$$

$$\sin C : \sin B = 4 : 6$$

$$\therefore \sin B : \sin C = 3 : 2$$

But with the method above, we can find the ratio between sin B and sin C is 3 : 2 easily because the raio between line band line c is ratio 3 : 2.\
Before, we couldn't know relation between 'the ratio between angles B and C' and 'the ratio between lines c and b'.\
However, we do not olny know the relation, but also calculate them!\
I will update this repository whenever it needs to be modified. Thnak you.



$$[PROOF]$$

$$1.\ 2R=\frac{b}{\sin B}=\frac{c}{\sin C} \ (\because \sin law, R\ is\ for\ radius)$$

$$\therefore \sin B \times c = \sin C \times b$$

$$2.\ \sin B \times c = \sin C \times b (\because proof.1)$$

$$\therefore \sin B : \sin C = b:c$$

$$Q.E.D.$$



$$[CODE]$$


The codes are like this;

    import math as m
        
    def same(a,b):  #remove rounding error with epslion(>0)
      if abs(a-b)<0.001:
        print('they are same')
      else:
        print('they are different')

    #Creating imaginary triangle. You can change the constant number below whenever you want.
    b=3.464 #√12
    c=2
    BD=2
    DC=2
        
    B= 60 #angle_ABC 
    C= 30 #angle_ACB
    alpha= 60 #angle_BAD
    beta= 30 #angle_DAC
       
    first_1 = (m.sin(m.radians(B)))*c
    first_2 = (m.sin(m.radians(C)))*b
        
    same(first_1, first_2)
        
    second_1 = (m.sin(m.radians(B))/m.sin(m.radians(C)))
    second_2 = b/c
        
    same(second_1, second_2) 

$$ [Execution\ Result] $$

they are same\
they are same

\>>>

For these proof and coding, we find this 'formula' works! I hope you utilize this concept in useful ways!
