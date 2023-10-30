
## Discrete Random Variables

>[!summary] Summary
>Discrete random variables are the foundation for modeling the behavior or a process or characteristic we are interested in.

>[!example] Example: Imperfections
>We are interested in the number of surface imperfections on a computer chip. The characteristic we are interested in is the number of surface imperfections. Let Y be the number of surface imperfection on a computer chip. The possible values for Y are:
>
>Y = 0 (no imperfections)
>Y = 1 (one imperfection)
>Y = x (x imperfections)

>[!example] Coin Flips
>
>When flipping a coin there are two possible outcomes {Head, Tail}.
>
>The random variable in a coin flip can be defined as:
$$\begin{cases} 0 & \text{if tails is observed}\\ 1 & \text{if heads is observed} \\ \end{cases}$$
>Or:
$$\begin{cases} -1 & \text{if tails is observed}\\ 1 & \text{if heads is observed} \\ \end{cases}$$
>Or even more abstract values:
$$\begin{cases} 0 & \text{if tails is observed}\\ 3e^{-2.3} & \text{if heads is observed} \\ \end{cases}$$
All work

![[Pasted image 20231011174318.png]]
This can best be understood by considering a 6 sided dice. When rolling the dice, ideally there is an equal 1/6 chance of any given side being rolled. However, each given side has its own value ranging from 1-6 corresponding to the number of dots on the side. So the probabilities of occurrence are equal but the variables' value is different and in this case independent.

#### Practice Question
The **[[Cumulative Distribution Function| cumulative distribution function(CDF)]]**, of a discrete random variable X, denoted as F(x), is defined by:
$$ F(x) = P(X\leq x) \text{ for any x} $$
For a [[Discrete Value | discrete random variable]] X, F(x) statisfies the following propertys:
1. 
$$ F(x_0) = P(X \leq x_0) = \sum_{x\leq x_0}f(x)$$
This property states that for a discrete value x0, The probability that X is less than or equal to x0, is equal to the sum of all x less than or equal to x0. Basically, the probability X is less than or equal to x0 is equal to the sum of the probabilities of all x less than or equal to x0.

2. $$ 0 \leq F(x) \leq 1 \text{ for any value of x}$$
The probability must always be between 0 and 1. 
3. $$ \text{If } x \leq y\text{, then } F(x) \leq F(y) \text{ (Non-decreasing)} $$
Since this is summing all probabilites less than or equal to x0, if y is greater than x, then the probability of y will always be greater than x. As y is just the probability of x plus all the probabilities in between.
4. $$ \lim_{x -> x_0 ^+} F(x) = F(x_0) \text{ Right-continous}$$
dd



This is a CDF

