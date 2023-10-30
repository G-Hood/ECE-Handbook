
>[!caution] Questions
>- [ ] What is a MOSFET
>- [ ] How does Doping effect the P/N Material
>- [ ] How does a small voltage to the base cause a huge gain
>- [ ] What determines the threshold voltage
>- [ ] Whats a Power Fet
>- [ ] How distinguish between enhanced and depletion FET
>- [ ] PFET - Vsg | NFET- Vgs

## MOSFETS

>[!important] Stuff Ball Says is Important (or I find interesting)
> - MOSFETS Require 2 sources, one for the gate, one for the source
> - Are actually Bi-Directional. They have an inherent parasitic diode.
> - Things that are Electrically insulating tend to be thermally insulating
> - Class A amplifier have single Transistor, low efficiency
> - Thermal considerations in circuit design
> - Fringing Effect on Non Ideal MOSFETS
> - Pinch off effect on Non Ideal MOSFETS
> - Big oxide is used to reduce fringing effects, acts as insulator to big n-type wells
> - Source and Drain inversed, source off while drain on and vice versa
> - Space Charge regions around the Wells
> - Dr. Ball disagrees with textbook, doesn't agree with doping
> -  


#### Summary
>[!summary] [[MOSFETS]]
><u>**M**</u>etal-<u>**O**</u>xide-<u>**S**</u>emiconductor <u>**F**</u>ield <u>**E**</u>ffect <u>**T**</u>ransistors
>
>In simplest terms, a MOSFET is a [[Voltage Controlled Switch]], aka a [[Field Effect Transistors]]. This a type of transistor in which the voltage is able to alter the resistivity of the path between the source and the drain. **WHAT DOES THIS MEAN/DO**
>Is essentially a voltage controlled resistor.

>[!example] Applications
> - Logic Gates
> - Sensors
> - Converters (Switching converters)
> - Memories
> - CPU
> - Digital Cameras (Entirely MOSFET Based)


>[!Summary] Fun-Facts!
>- Field-Effect Transistors are the most used device in [[Integrated Circuits]].
>- In the last 40 years, the exponential increase in computer power has a direct correlation to the ability to shrink the size of a FET.
>- Initially started being fabricated in the 1950s, however they say limited use due to manufacturing difficulties.
>- P-type condition region - PMOS
>- N-type conduction region - NMOS
>- CMOS has become the dominant technology in industry due to its low power consumption


#### Structure

![[ONEMOSSYBOI.png]]
*MOSFET less complicated*
**The** MOSFET, is a lot simpler than it looks or sounds, in this example we see a N-channel MOSFET, meaning negatively doped. From this picture we see n+ indicating that the transistor has been doped with a material such as phosphorus, giving it extra electrons. 

![[MOSFET NnP.png]]
![[MOSFET NnP.png]]
*N-channel and P-channel MOSFET*

In the above picture we see an example of two types of MOSFETS


N-type under bias (what)

Repels the holes to expose electrons,



$$ Q_G = -Q_D $$
$$ Q_D = qAN_AW $$
