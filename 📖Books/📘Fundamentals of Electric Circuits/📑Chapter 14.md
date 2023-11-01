

## Review Questions
--------------------------
>[!question] 14.1
A zero of the transfer function
$$ H(s) = \frac{10(s+1)}{(s+2)(s+3)} $$
is at:
(a) 10          (b) -1          (c) -2         (d) -3

>[!success]- Solution
> Answer: b
> >[!example]- Explanation
> >In the above function, H(s) is our transfer function, where s is a complex variable in the frequency domain given by the Laplace transform. In the case of finding the zero/zero's of at transfer function we need to find a value 's' such that the function 'H(s)' is equal to 0. In the above equation, by inspection, we see that at s=-1, we get:
> >$$H(s) = \frac{10(-1+1)}{(-1+2)(-1+3)}$$
> >Which gives us:
> >$$H(s) = \frac{0}{2}$$
> >$$H(s) = 0\text{ at s= -1} $$

-------
## Practice Problems

>[!question] 14.1
>Find the transfer function v<sub>o</sub>/v<sub>i</sub> of the RC circuit below. Express it using: $$ \omega _0 = \frac{1}{RC} $$
>![[FoEC-Chapter14-Prob-14-1]]

>[!info]- Hints
>1. We know the transfer function is equal to: $$ \frac{v_o}{v_i} $$ So, start by finding a way to express both those terms individually. 
>2. How does Vout and Vin relate to the impedance?
>

>[!success]- Solution
>$$ H(j \omega) = \frac{\frac{j \omega}{\omega _0}}{1+\frac{j \omega}{\omega_0}} $$
>Where:
>$$ \omega _0 = \frac{1}{RC} $$
> 
> 
> >[!example]- Explanation Of Solution
> >In the given exercise, we have a simple RC circuit. We want to find the expression for the transfer function, given that: $$H(j \omega) = \frac{v_0}{v_i}$$
> >
> >To start, lets recognize how the output voltage and input voltage relate to impedance. Firstly, we know: $$V=IR$$
> >In this simple circuit, I is constant. So: $$V_o = I*R\text{ and } V_i = I*(R+C)$$
> >Plugging those values in to our transfer function we get:
> >$$ H(j \omega) = \frac{v_o}{v_i} = \frac{\cancel{I}*R}{\cancel{I}*(R+C)}=\frac{R}{R+C}$$
> >Now with our wonderfully derived expressions, we can put their complex equivalents:
> >$$\frac{R}{R+\frac{1}{j\omega C}} = \frac{R*j \omega C}{R*j \omega C+\frac{j \omega C}{j \omega C}} = \frac{R*j \omega C}{1+R*j \omega C}$$
> >Lastly, we need to express the function using: $$ \omega _0 = \frac{1}{RC} $$
> >So plugging into our equation:
> >$$
> 











$$\cancel{x}$$


