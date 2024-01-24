# Transmission Lines

- Transmission Lines exist in a spatial dimension, with Resistance, Conductance, Capacitance, and Inductance having units of $\frac\Omega m$, $\frac1{\Omega m}$, $\frac Fm$, and $\frac Hm$
- These are measured per unit length, and the length of a transmission line needs to be accounted for when calculating its overall Impedance.
- Any structure or cable that guides an electromagnetic wave can be considered a transmission line.
  
  ![[2024-01-24]]
  
Using KVL:

$\LARGE v(z,\ t)-(R'\Delta z)i(z,\ t)-(L'\Delta z)\frac{\partial i}{\partial t}-v(z+\Delta z,\ t)=0$
$\LARGE v(z,\ t)-v(z+\Delta z, t)=\Delta z(i(z,\ t)R'+\frac{\partial i}{\partial t}L')$

$\LARGE-\frac{v(z+\Delta z, t)-v(z,\ t)}{\Delta z}=i(z,\ t)R'+\frac{\partial i}{\partial t}L'$

$\LARGE-\frac{\partial}{\partial z}v(z,\ t)=R'\cdot i(z,\ t)+L'\cdot\frac{\partial}{\partial t}i(z,\ t)$ 

We can find a similar equation using KCL instead of KVL:

$\LARGE-\frac{\partial}{\partial z}i(z,\ t)=G'\cdot v(z,\ t)+C'\cdot\frac{\partial}{\partial t}v(z,\ t)$

## Telegrapher's Equations

$\LARGE \frac{\partial}{\partial z}v(z,\ t)=\frac{\partial}{\partial z}\tilde V(z)=\frac{\partial}{\partial z}\text{Re}\{\tilde V(z)\cdot e^{j\omega t}\}=\text{Re}\{\tilde V(z)\cdot j\omega t\cdot e^{j\omega t}\}$

Applying this to the equation found with KVL:

$\LARGE-\frac{\partial}{\partial z}v(z,\ t)=R'\cdot i(z,\ t)+L'\cdot\frac{\partial}{\partial t}i(z,\ t)$ 

$\LARGE-\frac{\partial}{\partial z}\tilde V(z)=R'\cdot \tilde I(z)+L'\cdot\frac{\partial}{\partial t}\tilde I(z)$

$\LARGE-\frac{\partial}{\partial z}\tilde V(z)=[R'\cdot+j\omega L']\cdot\tilde I(z)$

$\LARGE-\frac{\partial^2}{\partial z^2}\tilde V(z)=[R'\cdot+j\omega L']\cdot\frac\partial{\partial z}\tilde I(z)$

and we find a similar equation doing the same process for the equation found by KCL:

$\LARGE-\frac{\partial^2}{\partial z^2}\tilde I(z)=[G'\cdot+j\omega C']\cdot\frac\partial{\partial z}\tilde V(z)$

substituting one equation into the other, we find:

$\LARGE\frac{\partial^2}{\partial z^2}\tilde V(z)=[R'\cdot+j\omega L'][G'\cdot+j\omega C']\cdot\tilde V(z)$

$\LARGE\frac{\partial^2}{\partial z^2}\tilde I(z)=[R'\cdot+j\omega L'][G'\cdot+j\omega C']\cdot\tilde I(z)$

choosing the propagation constant:
$\LARGE\gamma=\sqrt{(R'+j\omega L')(G'+j\omega C')}$

$\LARGE \frac{\partial^2}{\partial z}\tilde V(z)-\gamma^2\cdot\tilde V(z)=0$

$\LARGE \frac{\partial^2}{\partial z}\tilde I(z)-\gamma^2\cdot\tilde I(z)=0$

the propagation constant is complex:
$\LARGE\gamma=\alpha+j\beta$

where $\LARGE\alpha$ is an amount of gain or attenuation, and $\LARGE\beta$ is the phase change.

## General Solution

$\LARGE \tilde V(z)=V_o^+\cdot e^{-\gamma z}+V_o^-\cdot e^{\gamma z}$

$\LARGE \tilde I(z)=I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z}$

where $V_o^+$ and $I_o^+$ are waves traveling backwards to the source, while $V_o^-$ and $I_o^-$ are waves traveling forward from the source.

substituting this back into a previous equation:
$\LARGE-\frac{\partial}{\partial z}\tilde V(z)=[R'\cdot+j\omega L']\cdot\tilde I(z)$

$\LARGE-\frac{\partial}{\partial z}(V_o^+\cdot e^{-\gamma z}+V_o^-\cdot e^{\gamma z})=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

$\LARGE-(-\gamma\cdot V_o^+\cdot e^{-\gamma z}+\gamma\cdot V_o^-\cdot e^{\gamma z})=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

$\LARGE\gamma\cdot V_o^+\cdot e^{-\gamma z}-\gamma\cdot V_o^-\cdot e^{\gamma z}=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

and through some black magic sorcery, we find that:
$\LARGE \frac{V_o^+}{I_o^+}=\frac{(R'+j\omega L')}{\gamma}=\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}$

$\LARGE \frac{V_o^-}{I_o^-}=-\frac{(R'+j\omega L')}{\gamma}=-\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}$

