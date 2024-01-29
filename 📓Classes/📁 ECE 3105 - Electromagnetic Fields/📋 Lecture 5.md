# Air Line

We assume the conducting material in an air line is a good conductor with little resistance, so
$\LARGE R'=0\ \frac{\Omega}{m}$

And we assume the insulating gap in an air line is air with little conductance
$\LARGE G'=0\ \frac{S}{m}$

Because of these conditions, air lines are an ideal & lossless transmission line.

$\LARGE \gamma=\sqrt{(R'+j\omega L')(G'+j\omega C')}=\sqrt{(j\omega)^2L'C'}=j\omega\sqrt{L'C'}$
$\LARGE\gamma=\alpha+j\beta\longrightarrow\alpha=0,\ \ \ \beta=\omega\sqrt{L'C'}$

$\LARGE \lambda=\frac{2\pi}{\beta}=\frac{2\pi}{\omega\sqrt{L'C'}}$

$\LARGE Z_o=\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}=\sqrt\frac{j\omega L'}{j\omega C'}=\sqrt\frac{L'}{C'}$

We can assume these conditions are true when R' and G' are negligible, or when
$\LARGE R'<<\omega L',\ \ \ \ \ G'<<\omega C'$

# Physical Properties

## Coaxial



$\LARGE C'=\frac{2\pi\epsilon_s}{ln(\frac ba)}\ \frac Fm,\ \ \ \ \ \epsilon_s=\epsilon_r\epsilon_o,\ \ \ \ \ \epsilon_o=8.85\cdot10^{-12}\ \frac Fm$

$\LARGE L'=\frac{\mu_o ln(\frac ba)}{2\pi}\ \frac Hm,\ \ \ \ \ \mu_o=4\pi\cdot10^{-7}\ \frac Hm$

$\LARGE G'=\frac{2\pi\sigma_s}{ln\frac ba}\ \frac Sm$

$\LARGE R'\approx 0.1\ \frac\Omega m$

Assuming lossless:
$\LARGE Z_o=\sqrt{\dfrac{\frac{\mu_o ln(\frac ba)}{2\pi}}{\frac{2\pi\epsilon_s}{ln(\frac ba)}}}=2\pi ln(\frac ba)\sqrt{\frac{\mu_o}{\epsilon_s}}$

Typically $\LARGE\epsilon_r\approx2.25,\ \ \ \sigma_s=5.9\cdot10^{-5}$
