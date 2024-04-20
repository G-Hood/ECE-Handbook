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

>[!abstract] Unions and Intersection
>To describe sample spaces for the convolution of two or more sets, we use the $\cup$ operator and the $\cap$ operator.
>
>$\cup$ - **Union** - This is logically equivalent to the [[OR]] logic. This means the sample space is a combination of all Sample Points in the two sets. **Example**: $A = \{0, 1, 3, 5\}$ and $B = \{0, 2, 4, 6\}$. So $A \cup B = \{1, 2, 3, 4, 5, 6\}$ 
>
>$\cap$ - **Intersection** - This is logically equivalent to the [[AND]] logic. In this case the set is defined by the set of sample points common to both events. **Example:** $A = \{0, 1, 3, 5, 10\}$ and $B = \{0, 2, 4, 6, 10\}$. So $A \cap B = \{0, 10\}$ 


>[!summary] Mutually Exclusive Events
>
>Any two events which cannot occur at the same time, such that:
>$S_m \cup S_n = \varnothing$ and $S_m \cap S_n = \varnothing$ where $m \neq n$. #return 
>
>As they have no intersection we have the consequence that for **ONLY** mutually exclusive events: **P(A or B) = P(A) + P(B)**
>>[!example] Example of Mutually Exclusive Events
>>In an accident prone society, researchers at OSHA want to know the probability of someone dying on the job. As people can't die twice, the probability of dying on the job, is the sum of all ways people die on the job divided by the people who don't.

^4e74a4

## 1.3 Permutations and Combinations

>[!summary] Summary
>As the size of experiments get too large, we employ alternate methods for calculating probability, rather than describing the entire sample space. These methods are:
>**Permutations:** The arrangement of objects in a specific order. 
>**Combinations:** A set of objects regardless of order.
>
>**In Other Words:** With a combination we have N many options, and a bag with 3 slots, so we want to know how many different combinations of those options we can put in our bag. With a permutation we have N many options, and a [[Stack|stack]] with 3 slots, so we want to know how many different configurations of that stack we can make.

>[!summary] Calculating Permutations
>
>Intuitively to calculate permutations, we consider the slots. In the first slot, we can choose any of the objects in the set, in the second slot we can choose any object in the set minus 1 which is in the first slot. And continue. Putting this into a formula we get: $_nP_r = \frac{n!}{(n-r)!}$. Where n is the number of objects and r is the number of slots. This works because, following the logic above, we multipy our options **n** for the first slot, **n-1** for the second slot, etc, until we run out of slots. Where we can just divide by the remaining objects, so that after all slots are filled $(n-r)!$ cancels out any remaining multiplication done by $n!$.

>[!summary] Calculating Combinations
>Calculating Combinations follows a similar logic to permutations. That is: $_nC_r = \frac{n!}{r!(n-r)!}$ We use the same logic of finding the number of objects we can choose for each slot, and multiply it by the next minus 1. However we also divide by the factorial of the number of slots. Basically removing the arrangement from the problem such that each set only occurs once.

>[!important] Relationship Between Combinations and Permutations
>As they share similar characteristics we can describe their relationship as:
>$_nP_r = _nC_r *r!$
>and
>$_nC_r = \frac{_nP_r}{r!} = \frac{n!}{r!(n-r)!}$

>Intuitively we can recall a [[Binary Tree]] and [[Binary]]. If there is 1 option, there is one way to order it, if we have two numbers, it can be {0,0}, {0,1},{1,0},{1,1}. Add a third number and we double it.


>[!summary] Permutations of Indistinguishable Objects
>**Formula**: $\frac{n!}{n_1!*n_2!* ... *n_k!}$
>
>**Explanation:** Given m, n, i, 







