$$ \phi _k[n]=e^{j \omega _k n} $$


###### I'm So Lost (Questions)
- What does a Fourier Series do?
- What is is k?
- Why do we have so many different variables? (k, n, N, a)
- How do we take the sum?
- How do I get started on a problem?
- **What is N**
	   *N is the period of the DTFS, it represents the period of sampling. Basically how many times we sample the continuous signal in a single period. DTFS becomes a better and better approximation of CTFS as N approaches infinity*
- Sampling period? 

# Equations
#### Eigen Function Property

>[!summary] Summary
> If we put a complex exponential into the system, the result is a complex exponential at the same complex frequency, simply multiplied by an appropriate **complex factor** or **constant**
> 
> $$ e^{j \omega _k n}  -> e^{j \omega _k n} \sum_{r=- \infty} ^{+\infty} h[r]e^{-j \omega _k r} $$
> 
> 

>[!important] **Important Equations**
**[[Frequency Response]]** #frequency_response
$$H(\omega _r) = e^{j \omega _k n} \sum_{r=- \infty} ^{+\infty} h[r]e^{-j \omega _k r} $$ **[[Fundamental Frequency]]** $$ \omega _0 = \frac{2 \pi}{N} $$ **[[Synthesis Equation]]** #synthesis_equation$$ x[n] = \sum_{k=N_0} ^{N_0+N-1} a_ke^{jk \omega _0 n} $$


## Synthesis Equation
Given the below equation:
$$ x[n] = \sum_{k=N_0} ^{N_0+N-1} a_ke^{jk \omega _0 n} $$
	We see that for values k = 0, 1, 2, ..., N-1. The equation is going to be periodic, you can prove this using [[Euler's Formula]]. So given an infinite number of k's the output will repeat. Thus, if we want to construct our signal *x\[n]*, we simply need to find k for values from **k= 0 to N-1**. A property showing this can be given by:
	
	$$ e^{jk \omega _0 n} = e^{j(k+N) \omega _0 n} $$
	Which essentially says that given our **Period "N"** at any point where k, the value on each side of the equation is going to be exactly the same. As the equation is periodic.



## Analysis Equation

Given the analysis equation below:

$$ a_k = \frac{1}{N} \sum_{n=N_0}^{N _0 +N-1} x[n] e^{-jk \omega _0 n} $$
>[!caution] Differences Between CT and DT
>In Continuous Time and Discrete Time there are a few key important differences that allow us to better analyze DT.
>
>**Similarities Between CT & DT**
>$$ x[n] \space\space\space\space\space \text{periodic in n} $$
  $$ e^{jk \omega _0n} \space\space\space\space\space \text{periodic in n} $$
>
>**Exclusive to DT**
>$$e^{jk \omega _0n} \space\space\space\space\space \text{periodic in k}$$
>$$a_k \space\space\space\space\space \text{periodic in k}$$
>
>In DT their is periodicity in the Fourier coefficients. This is the major difference, that makes DT Fourier's different from CT Fourier's.






## Solving DTFS

To solve Discrete Time Fourier Series, you need

## Analyzing Fourier Series

To solve or analyze a Fourier Series of a discrete time signal we start by approximating a continuous time signal.

## Representing a Discrete Time Aperiodic signal
	Periodically replicate an aperiodic signal, the periodic and aperiodic signal are identical for one period. Its the fourier series representation of the periodic signal that represents the aperiodic signal.

###### Practice
d
##### Answers
d


### Practice
