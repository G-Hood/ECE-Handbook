# BJT Amplifiers

![[2024-01-29]]
## Common Emitter
![[2024-01-29_0|1000]]
KCL @ Base
$\LARGE \frac{v_{b}-v_s}{R_S}+\frac{v_{b}}{R_E}+\frac{v_be}{r_\pi}=0$

KCL @ Emitter
$\LARGE \frac{v_{eb}}{r_\pi}+\frac{v_e}{R_E}+g_mv_{be}+\frac{v_e-v_o}{r_o}+\frac{v_e-v_o}{R_C}=0$

$\LARGE \frac{v_o}{v_i}=-\frac{R_1//R_2//[(\beta+1)R_E+r_\pi]}{R_S+R_1//R_2//[(\beta+1)R_E+r_\pi]}\cdot\frac{g_m}{1+g_mR_E}\cdot (R_C//(r_o(1+g_mR_E))$

![[2024-01-29_1]]
$\LARGE G_m=$ Transconductance of whole circuit
$\LARGE G_m=\frac{\partial i_o}{\partial v_i}|_{v_o=0}=\frac{g_m}{1+g_mR_E}$

$\LARGE R_T=$ Driving Point Resistance
$\LARGE R_T=\frac{\partial v_o}{\partial i_o}|_{i_i=0}$ (open circuit input)

$\LARGE A_V=G_m\cdot R_T$

