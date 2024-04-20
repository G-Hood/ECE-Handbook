
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
>>  Using the dataset we can intuitively say that it rained $\frac{2}{7} days during the week. So the $P[Rain]$ during the week is $\frac{2}{7}$, however say it's a cloudy day and we want to predict if it'll rain. Well, intuitively we can see it was cloudy on $\frac{5}{7}$ days. On days in which it was cloudy it rained twice. So, while on any given day the probability of rain is $\frac{2}{7}$. If it's cloudy we can say $P[Rain|Cloudy] = \frac{\frac{2}{7}}{\frac{5}{7}}=0.4$  thus on a day it's cloudy, we have a $\frac{2}{5}$ chance of rain vs a $\frac{2}{7}$ chance on any day. 

## Independent Probabilities

>[!summary] Independent Probabilities
>In some cases we have probabilities where the outcome of one has no impact on the other. 
>
>**Intuition:** If we want to calculate the probability of winning the jackpot of a Powerball drawing. We calculate the probability of all our numbers being drawn. The ticket has 5 numbers drawn from one pool of ball, and a single number from a second pool of balls. Whatever balls are drawn from the first pool, has no effect on what is drawn from the second pool. Therefore we have independent probabilities, which both play a role in determining our likelihood of winning.
>
>**Definition:** $P[A_1 \cap A_2] = P[A_1]P[A_2]$
>That is, a probability is independent if the intersection of the two events, is the product of the two independent probabilities. 
>>[!example]- 
>>In a game of Monopoly, you role 2 dice. What is the probability that you get double 6's. Well intuitively, we know that there is a $\frac{1}{6}$ chance of rolling a 6. This is true for both dice. Thus to find the intersection {6,6}, we can simply multiply the individual probabilities: $\frac{1}{6} * \frac{1}{6} = \frac{1}{36}$. We can further understand this result, by looking at the total number of pairs of numbers, we have 36 possibilities of pairs and only 1 of them is both 6's. We could also apply this principle to both dice rolling odd numbers.  
>
>This definition also works for a collection of any number of sets:
>$P[A_1 \cap A_2 \text{....} \cap A_n] = P[A_1]*P[A_2]\text{...}*P[A_n]$

>[!caution] Checking for Independence
>It is not always clear if two events are independent. Two events are only independent if:
>$P[A_2|A_1] = P[A_2]$ Given that $P[A_1] \neq 0$
>	*and*
>$P[A_1|A_2] = P[A_1]$ Given that $P[A_2] \neq 0$


>[!summary] Multiplication Rule
>**Definition:** $P[A_1\cap A_2] = P[A_2|A_1]P[A_1]$
>
>The multiplication rule allows us to find the probability of any two events occurring simultaneously, regardless of if they are independent.

## Bayes' Theorem

>[!summary] Bayes' Theorem
>
>Allows us to find the probability $P[A|B]$ when the data available does not fit the requirements to apply the definitions we previously defined.
>
>Given a collection of [[📖Books/📘Introduction To Probability And Statistics/📑Chapter 1#^4e74a4|mutually exclusive]] events $A$ where the Union of all $A$ makes up the [[Sample Space]] $S$, and B an event such that $P[B] \neq 0$.
> 
>**Definition:** $P[A_j | B] = \frac{P[B|A_j]P[A_j]}{\sum _{i=0} ^n P[B|A_i]P[A_i]}$
>
>

