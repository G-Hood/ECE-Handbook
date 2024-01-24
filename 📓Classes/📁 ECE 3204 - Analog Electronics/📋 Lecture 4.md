# MOS (Metal Oxide Semiconductor) Transistors

![[Power/AAA Excalidraw/2024-01-24|2024-01-24]]

In NMOS linear/triode region:
$\LARGE I_{DS}=\mu C_{ox}\frac{W}{L}[(V_{GS}-V_{TH})V_{DS}-\frac{V_{DS}^2}{2})]$

In NMOS saturation region:
$\LARGE I_{DS}=\frac12\mu C_{ox}\frac{W}{L}(V_{GS}-V_{TH})^2(1+\lambda V_{DS})$

## MOS Construction
![[2024-01-24_0]]
### Which terminal is the drain?

With bipolar devices, the circuit designer decides.

NMOS: DRAIN is the HIGHEST potential between drain and source terminals
- electrons flow from low to high
PMOS: DRAIN is the LOWEST potential between drain and source terminals
- holes flow from high to low

## PMOS vs NMOS

Instead of using separate equations for NMOS and PMOS, just reverse the subscripts used for NMOS when solving PMOS circuits, also - always use the absolute value of the threshold voltage

NMOS Rules:

| $\LARGE V_{GS}>V_{TH}$ | $\LARGE V_{GD}<V_{TH}$ | $\LARGE V_{DS}<V_{GS}-V_{TH}$ |
| :--: | :--: | :--: |
| On | Saturation | Linear/Triode |
| $\LARGE I_{DS}=\mu C_{ox}\cdot$ | $\LARGE \frac12\frac{W}{L}(V_{GS}-V_{TH})^2(1+\lambda V_{DS})$ | $\LARGE\mu [(V_{GS}-V_{TH})V_{DS}-\frac{V_{DS}^2}{2})]$ |

## Small Signal Model

![[2024-01-24_1|500]]
$\LARGE g_m=\frac{\partial I_{DS}}{\partial V_{GS}}=k'V_{DS}^\text{sat}=\mu C_{ox}\frac WL(V_{GS}-V_{TH})=\frac{2I_{DS}}{V_{DS}^\text{sat}}=\sqrt{2I_{DS}\mu C_{ox}\frac WL}$

$\LARGE V_{DS}^\text{sat}=V_{ov}=V_{GS}-V_{TH}=\sqrt\frac{2W\cdot I_{DS}}{\mu C_{ox}L}$

$\LARGE k'=\mu C_{ox}\frac WL$

$\LARGE g_o=\frac{\partial I_{DS}}{\partial V_{DS}}=\lambda\cdot I_{DS}\longrightarrow r_o=\frac{1}{g_o}=\frac{1}{\lambda\cdot I_{DS}}$

Triode:
$\LARGE g_{ds}=\frac{\partial I_{DS}}{\partial V_{GS}}=\mu C_{ox}\frac WL(V_{DS}^\text{sat}-V_{DS})\longrightarrow r_{ds}=\frac{1}{g_{ds}}$

![[2024-01-24_2]]






