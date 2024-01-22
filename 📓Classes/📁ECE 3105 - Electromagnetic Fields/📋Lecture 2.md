# Phasors

- No time variation
- Not scalers or vectors - just complex numbers

Time varying signal:
$\LARGE A(t,\ \omega)=A_m(\omega)\cdot cos(\omega t+\Psi(\omega))$

Phasor signal:
$\LARGE C(\omega)=A_m\cdot e^{j\Psi(\omega)}$

Converting phasors to time domain:
$\LARGE A(t,\ \omega)=\text{Re}\{C(\omega)\}=\text{Re}\{A_m\cdot e^{j\Psi(\omega)}\}$

### Examples

$\LARGE A_m\cdot cos(\omega t)\longrightarrow A_m\angle0$

$\LARGE A_m\cdot cos(\omega t+\theta)\longrightarrow A_m\angle\theta=A_m\cdot e^{j\theta}$

$\LARGE A_m\cdot sin(\omega t)\longrightarrow A_m\angle-90°$

![[2024-01-22|250]]
$\LARGE V_s(t)=V_o\cdot sin(\omega t+\theta_o)=V_o\cdot cos(\omega t+\theta_o-90°)$
$\LARGE =\text{Re}\{V_o\angle(\theta_o-90°)\}=\text{Re}\{V_o\cdot e^{j(\theta_o-90°)}\}$

### Transmission Lines

$\LARGE c=3\cdot10^8$
$\LARGE \beta = \frac\omega c$

if $f=60\ Hz,\ \omega=277$
$\LARGE \beta=\frac{277}{300\cdot10^6}=10^{-6}$

$\LARGE \beta x$ for 1 meter cable $=10\cdot10^{-6}=10^{-5}$ radians

\*\*\* IRL, we choose $\beta$ such that $\beta x$ is small

