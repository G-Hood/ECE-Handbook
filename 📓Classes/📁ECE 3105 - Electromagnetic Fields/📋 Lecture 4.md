Last lecture we found two differential equations representing our wave equations:

$\LARGE \frac{\partial^2}{\partial z}\tilde V(z)-\gamma^2\cdot\tilde V(z)=0$

$\LARGE \frac{\partial^2}{\partial z}\tilde I(z)-\gamma^2\cdot\tilde I(z)=0$

where $\LARGE \gamma^2=(R'+j\omega L')(G'+j\omega C')$


$\LARGE v(z,\ t)=\text{Re}\{\tilde V(z)\cdot e^{j\omega t}\}$
$\LARGE i(z,\ t)=\text{Re}\{\tilde I(z)\cdot e^{j\omega t}\}$

$\LARGE \gamma=\alpha+j\beta$

$\LARGE \tilde V(z)=V_o^+\cdot e^{-\gamma z}+V_o^-\cdot e^{\gamma z}$
$\LARGE \tilde I(z)=I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z}$

Plugging these into the telegrapher's equation:
$\LARGE-\frac{\partial}{\partial z}\tilde V(z)=[R'\cdot+j\omega L']\cdot\tilde I(z)$

$\LARGE-\frac{\partial}{\partial z}(V_o^+\cdot e^{-\gamma z}+V_o^-\cdot e^{\gamma z})=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

$\LARGE-(-\gamma\cdot V_o^+\cdot e^{-\gamma z}+\gamma\cdot V_o^-\cdot e^{\gamma z})=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

$\LARGE\gamma\cdot V_o^+\cdot e^{-\gamma z}-\gamma\cdot V_o^-\cdot e^{\gamma z}=[R'\cdot+j\omega L']\cdot(I_o^+\cdot e^{-\gamma z}+I_o^-\cdot e^{\gamma z})$

we know that the terms with $\LARGE e^{\gamma t}$ and $\LARGE e^{-\gamma t}$ must balance out, so:
$\LARGE-\gamma\cdot V_o^-\cdot e^{\gamma z}=[R'\cdot+j\omega L']\cdot I_o^-\cdot e^{\gamma z}$

$\LARGE\frac{V_o^-\cdot \cancel{e^{\gamma z}}}{I_o^-\cdot \cancel{e^{\gamma z}}}=\frac{R'\cdot+j\omega L'}{-\gamma}$

$\LARGE \frac{V_o^-}{I_o^-}=-\frac{R'\cdot+j\omega L'}{\gamma}=-\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}$

And similarly we find 
$\LARGE \frac{V_o^+}{I_o^+}=\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}$

where we call this term the characteristic impedance $\LARGE Z_o$

$\LARGE V_o^+=|V_o^+|e^{j\phi^+}$ 

$\LARGE V_o^-=|V_o^-|e^{j\phi^-}$ 

$\LARGE v(z,\ t)=\text{Re}\{\tilde V(z)e^{j\omega t}\}=\text{Re}\left\{(V_o^+\cdot e^{-\gamma z}+V_o^-\cdot e^{\gamma z})e^{j\omega t}\right\}$

$\LARGE v(z,\ t)=\text{Re}\left\{(|V_o^+|e^{j\phi^+}\cdot e^{-\gamma z}+|V_o^-|e^{j\phi^-}\cdot e^{\gamma z})e^{j\omega t}\right\}$

$\LARGE v(z,\ t)=\text{Re}\{(|V_o^+|e^{j(\omega t+\phi^+)-(\alpha+j\beta) z}+|V_o^-|e^{j(\omega t+\phi^-)+(\alpha+j\beta) z}\}$

$\LARGE v(z,\ t)=\text{Re}\{(|V_o^+|e^{j(\phi^++\omega t)-(\alpha+j\beta) z}+|V_o^-|e^{j(\omega t+\phi^-)+(\alpha+j\beta) z}\}$

$\LARGE v(z,\ t)=|V_o^+|e^{-\alpha z}cos(\omega t-\beta z \phi^+)+|V_o^-|e^{\alpha z}cos(\omega t+\beta z \phi^-)$

Example:
if $G'=0$ and $R'=0$ then

$\LARGE Z_o=\sqrt\frac{R'+j\omega L'}{G'+j\omega C'}=\sqrt\frac{j\omega L'}{j\omega C'}=\sqrt\frac{L'}{C'}$

$\LARGE \beta=\text{Im}\sqrt{(R'+j\omega L')(G'+j\omega C')}=\text{Im}\{j\omega\sqrt{L'C'}\}=\omega\sqrt{L'C'}$
$\LARGE \alpha=\text{Im}\sqrt{(R'+j\omega L')(G'+j\omega C')}=\text{Im}\{j\omega\sqrt{L'C'}\}=0$

So if we want a transmission line with no loss, we need zero resistance and zero conductance.
