
### 16.1.1

- The n-channel transistors for integrated circuits are all fabricated from the same p-type subtrate material. Which is connected to the most negative potential in the circuit, IE Ground.
- In many transistors however, the source terminal will not be zero volts. Which creates a reverse biased pn junction between the source and sbstrate.
- When the source and body terminals are of different voltage potential, the threshold voltage of the transistor is a function of the source-to-body voltage. Thus the [[Body Effect]] is an important factor to consider when determining logic of circuits.
#### Key Equations
##### **Current-Voltage Relation**

>[!summary] Regions
>**Biased in Non-Saturation Region | (v<sub>GS</sub> >= V<sub>TN</sub> and v<sub>DS</sub> <= (v<sub>GS</sub> - V<sub>TN</sub>)**
 i<sub>D</sub> = K<sub>n</sub>\[2(v<sub>GS</sub>-V<sub>TN</sub>)v<sub>DS</sub>-V<sup>2</sup><sub>DS</sub>] 
 **Biased in Saturation Region | v<sub>GS</sub> >= V<sub>TN</sub> and v<sub>DS</sub> >= (v<sub>GS</sub> - V<sub>TN</sub>) **
 i<sub>D</sub> = K<sub>n</sub>(v<sub>GS</sub> - V<sub>TN</sub>)<sup>2</sup>(1+λv<sub>DS</sub>) 
 *(Note that λ is most often 0, thus the latter of the equation is typically left out)*
 
 
 
 
 
>[!summary] Transistion Point
>Represents the separation between the saturation and non-saturation regions and is equal to the Drain to Source Voltage.
>v<sub>DS</sub> = v<sub>DS</sub>(sat) = V<sub>GS</sub>-V<sub>TN</sub>
>

 >[!summary] Conduction Parameter
 >K<sub>n</sub> - NMOS Transistor Conduction Paramter
 >$$ K_n = ( \frac{1}{2} μ_n C_{ox})(\frac{W}{L})=\frac{k^{'}_n}{2}\frac{W}{L} $$
 >
 >In the case of these circuits, λ, is presumed to be 0 unless otherwise stated.
 
 
 
 
 
 
 
 
 
 
 
 

