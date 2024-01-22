# Bipolar Junction Transistors

![[Notes/📓Classes/📁ECE 3204 - Analog Electronics/2024-01-22|2024-01-22]]
$\LARGE I_C=I_S\cdot e^{\frac{V_{BE}}{V_T}}(1+\frac{V_{CE}}{V_A})$

for large $V_A,$ $\LARGE\frac{V_{CE}}{V_A}\approx0$ and $\LARGE I_C=I_S\cdot e^{\frac{V_{BE}}{V_T}}$

- BJTs are Voltage Controlled Current Sources.
- We give an input voltage $V_{BE}$ and are given an output current $I_C$.
- We then run $I_C$ through a resistor to get an output voltage.

## Transconductance

$\LARGE g_m=\frac{\partial I_C}{\partial V_{BE}}=\frac{I_C}{V_T}$

$\LARGE g_o\triangleq$ output conductance $\LARGE=\frac1{r_o}=\frac{\partial I_C}{\partial V_{CE}}=\frac{I_C}{V_A}$

$\LARGE r_\pi\triangleq$ base emitter resistance $\LARGE=\frac\beta{g_m}$

$\LARGE\beta\triangleq$ base-collector current gain $\LARGE=\frac{I_C}{I{\beta}}\approx100$

$\LARGE A_o=$ intrinsic gain $\LARGE=\frac{g_m}{g_o}=\frac{V_A}{V_T}$

## Small Signal Model

![[2024-01-22 1]]
KCL @ Collector:
$\LARGE v_og_o+g_mV_{BE}=0,\ \ \ v_i=V_{BE}$
$\LARGE \frac{v_o}{v_i}=-\frac{g_m}{g_o}$

b