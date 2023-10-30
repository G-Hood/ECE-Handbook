
## Symbols and Tables


#### Symbols

>[!summary] Different Set Symbols
>
Function | Symbol |
---|---|
AND | $$ p \land q $$ |
OR | $$ p \lor q $$ |
NOT | $$ \lnot p $$ |
XOR | $$ p \oplus q $$|

##### Function Truth Tables
###### AND - OR
>[!summary] AND - OR
>
p | q | $$ p \land q $$| $$ p \lor q $$|
---|---| ---| ---|
F | F | **F** | **F**
F | T | **F** | **T**
T | F | **F** | **T**
T | T | **T** |**T** 


###### XOR
>[!summary] XOR
>
p | q | $$ p \oplus q $$| 
---|---| ---|
F | F | **F** |
F | T | **T** | 
T | F | **T** | 
T | T | **F** |
###### NOT
>[!summary] NOT
>
p | -p
---|---|
F | T 
T | F 








## Section 1.1 

#### Logic and Propositions

[[Logic]] is the study of formal reasoning. Unlike in natural language, logic uses statements to have a well defined specific meaning. This is incredibly useful in applications of [[Artificial Intelligence]].

A [proposition](Proposition) is a statement that is either true or false. For example, "2 is an even number" is a proposition as it is either true or false. Questions or commands do not count as propositions, we cannot command "2" to be an even number, it either is or isn't. Same thing for a question, asking if 2 is an even number is not a proposition as it makes no statement, however it's response may be.

## Section 1.3 - Conditional Statements
![[Conditional Operation]]
## Section 1.4 - Logical Equivalence

A compound proposition is a [tautology](Tautology) if the proposition is always true. IE, if P is true, Q is true, if P is false Q is true. Basically, regardless of input the output is true.                                                                                                                                                                                               

## Section 1.6 - Logical Reasoning

[[Logic]] enables us to formally establish the truth of logical statements, doing so by assuming the truthfulness of a set of hypotheses. An argument is a set of [propositions](Proposition) consisting of 2 parts, a sequence of propositions which are hypotheses and a final proposition which asserts that the final proposition is true based upon the truthfulness of the hypotheses. IE, If our sequence of **hypotheses** is true, then the **conclusion** must be true, and thus the argument is valid.

>[!summary] Argument
>An argument is considered valid when the proposition and conclusion is a [tautology](Tautology). 
>$$ (p_1 \land p_{2} \land p_{3}\land \text{...} \land p_n) \rightarrow c $$
>(i.e.) If the above is a **tautology**, meaning the **proposition** and **c* (conclusion)*** are logically equivalent. The argument is valid.
>

## Section 1.7 - Predicates and Quantifiers

A [predicate](Predicate) is a logical statement where the truth value is a function of one more variables. This is very similar to methods/functions in coding. 
> [!example] Example
> ```cpp
> bool isEven(int x) {
>     if (x % 2 == 0) {
>         return true;
>     } 
>     else {
>         return false;
>     }
> }
> ```
> The above code takes in a parameter `x` and returns `true` if `x` is an even number or `false` if it is not. A predicate is exactly the same. As it is dependent on one or more variables.

Predicates also operate within [domains](Domain), which is defined as the **set of all possible values** which a variable might be. For example in the above code, as we are trying to find if a number is **even** or **odd**, this is a **property of integers**, so our **domain** would be the **set of all integers**.

Predicates can be used in various situations with more abstract variables. Think **Object Oriented Programming**.

> [!example] Example Predicate Abstract

Suppose we have the statement:
"The car has over 30,000 miles"

In this example:
> [!example] Example Predicate Abstract
> Suppose we have the statement:
> "The car has over 30,000 miles"
> 
> In this example:
> The **Car** is the **variable**, as we don't specify a specific car. If this was a function in code, we could pass in a car variable into a function that returns  true "if miles is greater than 30,000". So, the car is the variable and the **Set of All Cars in Existence** is the **Domain**. However, we can also limit the domain, say we only want to know the truthfulness of this statement for cars in the US, then the set would be all cars in the **US**.
> 

If all variables in a predicate have a defined/specific value, it becomes a proposition, as the truthfulness is well defined. However there is also another case.
#### Universal Quantifier
The [[Universal Quantifier]], denoted by '**∀**' allows us to assert that for all x, the output of the function is true. This is denoted by:
$$ ∀x P(x) $$
And is true when:
$$ ∀xP(x) \equiv P(x_1) \land P(x_2) \land \text{...} \land P(x_k) $$
Meaning that regardless of what value you put in for x, the **predicate** P(x) is always true. This only takes a single **Counter-example** to prove **false**.

#### Existential Quantifier

The [[Existential Quantifier]], denote by '**∃**' allows us to assert that for the conclusion P(x), there exists at least one value x that the statement is true for. This is denoted by:
$$∃xP(x) $$
And is true when:
$$ ∃xP(x) \equiv P(x_1)\lor P(x_2) \lor \text{...} \lor P(x_k) $$
Meaning that for the **variable x** and the **predicate** **P(x)**, if the domain is a finite set of elements, then there exists a value for x such that P(x) is true. This also shows that it is logically equivalent to the span of all values x, such that P(x). 

*Notice that for the [[Universal Quantifier]] and [[Existential Quantifier]], the only difference is the **universal** uses all **and**, and the **existential** is all **or**.*

## Section 1.8 - Quantified Statements

The [[Universal Quantifier]] and [[Existential Quantifier]] may be used in compound predicates or logical operations:
$$  ∃x P(x) \land \lnot Q $$

Which says that there exists a value x such that P(x) is true AND Q is false.

We can use the associative property to further clarifiy:
$$  ∃x (P(x) \land \lnot Q) $$

#### Bound/Free Variable

A variable x in the **predicate P(x)** is called a **free variable**, as the value x is free to be any value within the domain of X, and has no certain value. However, the **variable x** in the statement **∀x P(x)** is called a **bound variable** as the variable is bound to the quantifier.

>[!example] Bound vs Free Variable
>This is a lot more clear when considering our car example from section 1.7.
>
>If we are to take the original predicate, P(x), where we state "The car has more than 30,000 miles". We are saying that a car has 30,000 miles, however the car is not defined, so depending on what car we pass into the function, the validity of the argument will either be valid or invalid, and is yet to be determined.
>
>In the case of the statement ∀x P(x). We are saying "All cars have more than 30,000 miles". Thus we no longer have a function that we can test any car, and are rather testing every car to see if our statement is valid. Thus the truth value can be determined, as no variables are uncertain. 

 ## Section 1.9 - De Morgan's Law for Quantified Statements

