
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
>- $P[A'] = 1 - P[A]$ | Given that the sum of all events $A$ in a sample space $S$ is 1. We can say that $A'$ is the probability of any event occurring except for event $A$, therefore the probability of $A$ not occurring, is the probability of any event within $S$ occurring minus the probability of $A$ occurring. This only applies when $S$ is entirely made of mutually exclusive events.
> >[!example]- 
> >In a game of rock paper scissors, given any input, there are 3 possible outcomes, you win, you tie, or you lose. Given you play rock, there is a $\frac{1}{3} chance of you winning. There the probability that you don't win is $1-\frac{1/3} = \frac{2}{3}$. 
>**Any Case**
>- **General Addition Rule:** $P[A_1 \cup A_2] = P[A_1] +P[A_2] - P[A_1 \cap A_2]$ | The Probability of any event occurring out of two subsets within the same sample space, is the probability of each occurring minus the intersection of the two events.
>>[!example]- Example
>>Given the set of numbers $\{1, 2, 3,4,5,6,7,8,9,10\}$. Subset $A_1$ is all odd numbers {1,3,5,7,9}$. Subset $A_2$ is all prime numbers $\{1,3,5,7\}$. Subset $A_3$ is all even numbers $\{2,4,6,8,10\}$. 
>>To find $P[A_1 \cup A_2]$ we find the individual probabilities, minus the probabilities they have in common. That is: $P[A_1] = \frac{5}{10}$, $P_[A_2] = \frac{4}{10}$, and $P[A_1 \cap A_2] = \frac{4}{10}$ 
>>Therefore $P[A_1] + P[A_2] = \frac{5}{10 }+ \frac{4}{10} - \frac{4}{10}$
>>
>>In the case of $P[A_2] + P[A_3]$, we see $P[A_2] = \frac{4}{10}$, $P[A_3] = \frac{5}{10}$, and from observation we see that $A_2$ and $A_3$ have no numbers in common from the sample space, thus $P[A_2 \cap A_3] = 0$. 
>>Therefore $P[A_2] + P[A_3] = \frac{4}{10} + \frac{5}{10} - \frac{0}{10} = \frac{9}{10}$


## Conditional Probability

>[!summary] Conditional Probability
>In cases where probability is not mutually exclusive, the probability that one event occurs may be higher or lower given that another event has already occurred. 
>
>**Intuition**: Consider the weather on any given day, if it's cloudy there is a higher probability that it rains, as we know rain precipitates from clouds. If it's sunny and clear, intuitively we know it's less likely to rain. 
>
>**Definition**: $P[A_2|A_1] = \frac{P[A_1 \cap A_2]}{P[A_1]}$
>That is to say, the probability that event $A_2$ occurs, given that $A_1$ has already occurred is equal to the intersection of it $A_1$ and $A_2$ divided by the probability that $A_1$ occurs.
>>[!example]- Example
>>Recall the weather example, in data for weather during any week:
>>- Monday - Rainy, Cloudy
>>- Tuesday - Cloudy
>>- Wednesday - Sunny, Cloudy
>>- Thursday - Sunny
>>- Friday - Sunny
>>- Saturday - Rainy, Cloudy
>>- Sunday, Cloudy
>>  
>>  Using the dataset we can intuitively say that it rained $\frac{2}{7} days during the week. So the $P[Rain]$ during the week is $\frac{2}{7}$, however say it's a cloudy day and we want to predict if it'll rain. Well, intuitively we can see it was cloudy on $\frac{5}{7}$ days. On days in which it was cloudy it rained twice.  






