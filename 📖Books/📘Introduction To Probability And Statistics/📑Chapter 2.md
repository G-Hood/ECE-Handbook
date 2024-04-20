
>[!summary] Chapter Summary



## The Foundation of Probability

>[!summary] Summary - Axioms of Probability
>Everything in probability is based on a few absolute rules/laws:
>
>**1.** $P [$[[Sample Space|S]]$] = 1$ | The probability of an event within the sample space occurring is 1.
>**2.** $P[A] \geq 0$ for every event A. | For any event within the sample space, the probability will always be greater than or equal to 0. No negative probabilities.
>**3.** Given [[📖Books/📘Introduction To Probability And Statistics/📑Chapter 1#^4e74a4|Mutually Exclusive]] events $\{A_1, A_2, _{...}, A_n\}$  whether finite or infinite. $P[A_1 \cup A_2 \text{ }{...} \cup A_n] = P[A_1]+P[A_2] + ... + P[A_n]$ | The sum of mutually exclusive events is equal to the probability of each event occurring independently.


>[!important] Derivations of Axioms
>Given the Axioms of Probability we can derive some other rules that are simply just consequences of these given 3 rules.
>**Mutually Exclusive**
>- $P[\varnothing] = 0.$ #return 
>- $P[A'] = 1 - P[A] | Given that the sum of all events $A$ in a sample space $S$ is 1. We can say that $A'$ is the probability of any event occurring except for event $A$, therefore the probability of $A$ not occurring, is the probability of any event within $S$ occurring minus the probability of $A$ occurring. This only applies when $S$ is entirely made of mutually exclusive events.
> >[!example]- 
> >In a game of rock paper scissors, given any input, there are 3 possible outcomes, you win, you tie, or you lose. Given you play rock, there is a $\frac{1}{3} chance of you winning. There the probability that you don't win is $1-\frac{1/3} = \frac{2}{3}$. 
>**Any Case**
>- $P[A_1 \cup A_2] = P[A_1] +P[A_2] - P[A_1 \cap A_2]$ | The Probability of any event occurring out of two subsets within the same sample space, is the probability of each occurring minus the intersection of the two events.
>>[!example]- Example
>>Given the set of numbers




