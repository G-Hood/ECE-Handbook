---
aliases:
  - Classical Approach
  - Personal Approach
  - Relative Frequency
---


>[!summary] Introduction:
>Statistics is an extremely important concept to engineers, and is much more pervasive then one might initially think. As scientists and engineers, we don't necessarily describe how the world "is", we simply create models that give us the power to predict how the world will **behave**. These models are based on empirical data and statistics.
>
>>[!example] Example:
>>One example of this is with [[Ohm's Law]]. Where we say V= IR

## 1.1 What are the Odds?

>[!summary] Key Points
>- Probability is a number between 0 and 1
>- Tells how likely or unlikely an event is to occur with 1 being always and 0 being never, although most are between.

>[!summary]
>**Three Methods** 
>- **Personal Approach**: Making an informed assumption as a matter of opinion, based on the evidence available, mostly useful in highly unique situations without precedent to make an statistical determination. Pros: Highly Available | Cons: Not necessarily Accurate
>- **Relative Frequency**: $\frac{Occurrences}{Trials}$ This method uses repeated trials, dividing the number of times an event occurs by the number of times it could've occurred. Pros: Fairly Accurate | Cons: Restricted to Events with repeatable trials
>- **Classical Approach**- This method divides the number of way a specific event can occur, by the number of ways an experiment could proceed, given all events are equally likely. **Pros: Does Not Require Experiment | Cons: Only usable when events are equally likely**
>  >[!example] Three Methods with a Coin Flip
>  >A coin will be flipped once, call heads or tails?
>  >**Personal Approach: ** "I have a feeling it'll be heads"
>  >**Relative Frequency:** I flipped this coin 10 times and I got 6 heads, and 4 tails, so heads, as there is a 0.6 probability of heads, which is slightly higher than tails. $p=\frac{6}{10}$
>  >**Classical Approach: **There are two ways it could go, and 1 way it would be heads, and 1 way it would be tails, therefore it doesn't really matter which you pick. $p=\frac{n(A)}{n(S)}$
>  



## 1.2 All the Possibilities

>[!summary] Summary
>As seen with the classical method, in many cases to determine the probability we need to know everything that CAN happen. Thus we must define the **[[Sample Space]]**.
>![[Sample Space]]

>[!example] Example Sample Space
>A Gardener plants 3 flowers. After a year he wants to see how many grew, what are the possible outcomes:
>In this case the sample space would be ${\{yyy, yyn,yny, ynn, nyy, nyn, nny, nnn\}}$. y corresponding to having grown, n corresponding to it not having grown.
>[[Tree Diagram|Tool for Determining]] sample spaces


>[!example] Applying Sample Spaces to Classical Approach
>Using the above example, what is the probability that only two flowers grow?
>Given that the sample space **S** has 8 combinations, we can say $n(S) = 8$, for $n(A)$, we make a set of all the combinations where there is only 1 n. So $n(A) = 3$. Therefore using the Classical Approach the probability that $\frac{2}{3}$ flowers grow is $p = \frac{3}{8}$


>[!note] Unions and Intersection
>To describe sample spaces for the convolution of two or more sets, we use the $\cup$ operator and the $\cap$ operator.
>
>$\cup$ - **Union** - This is logically equivalent to the [[OR]] logic. This means the sample space is a combination of all Sample Points in the two sets. **Example**: $A = {1, 3, 5}$ and $B = {2, 4, 6}$. So $A \cup B = {1, 2} 










