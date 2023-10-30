# Part A
#### What are Power Electronics?

Power electronics are electronics that allow for the control and conversion of electric power. Basically, a power electronic is a electronic device that allows for the conversion of electrical power from one form to numerous others. Examples include the full-bridge rectifier which is used to convert an AC signal to DC signal. An inverter which converts a DC current to an AC current. 

Common devices that use power electronics include: 
- The electric car, which uses power electronics to control the electricity between the motor and the battery, allowing for the operator to manage the speed and acceleration of the electric vehicle. Power electronics also play a role in regulating the charge of the battery itself. 
- House-hold induction cooker, heaters that heat up food when placed in a pan of the proper material. These devices use a regular AC power supply, such as the one you'd get through the plug on your wall, and convert this into a even higher frequency AC signal.

#### What is DC/DC Converter

>[!caution] Improve
A DC to DC converter is an electronic which converts the voltage from the output of a device such as a battery to a voltage more suitable for the target electronic. One example of this is a Laptop, the battery of a laptop, is usually just one big voltage source, however, many of the components in a computer require different voltages to operate. z a DC/DC converter may be employed to supply those components with their needed supply.


#### DC/DC Converter required for this project

There are numerous different types of DC/DC converters, however for our project we will want to make use of a Buck-Boost Converter. A buck-boost converter allows for the device to step up or step down the output voltage. In our given project, we are using a **Solar Panel**, which depending on the weather conditions, can either be outputting higher than needed or lower than needed voltage. Thus a Buck-Boost Converter, will allow for increased output when solar conditions are less then needed, or lowered output when conditions are outputting greater voltage then needed.

#### Converter





# Part B
#### Inductor DCR

In every electrical component, there are parasitic elements (the non-ideal  
elements). What is inductor DCR and how would this impact the circuit efficiency?  
What is capacitor ESR? Look through the data sheets for the 3 different MOSFETS,  
2 different diodes in your parts kit, and discuss the major differences between  
them? Which MOSFET and diode would lead to higher efficiency for the circuit?


Inductor DCR is the resistance of an inductor at ~0Hz. In an ideal inductor the resistance scales with frequency, being 0 at 0 Hz and increasing as frequency increases. However, in actual inductors there exists a parasitic resistance which is determined by the inherent resistance of the coil, and naturally, scales with the length of the coil. This can be observed when plugged into the formula for resistivity:

$$ \rho = R\frac{A}{l} $$
Or likewise:
$$ R = \rho \frac{l}{A}$$
Where we observe rho is the resistivity of the given material, A is the cross-sectional area, and l is the length. As such we observe that given a material and a constant cross-sectional area, the resistance of the coil will scale linearly with the length.

In our case we are likely working with copper, one of the most common, cheaper, and lowest resistive materials, with a resistivity of 16.78 nanoOhm meters.

As a type of resistance DCR causes dissipation of heat in our circuit, which is a loss of efficiency. We can measure this loss, by plugging our specifics into the Q-factor formula. Where:

$$ Q = \frac{X_L}{R} $$
or 
$$ Q= \frac{\omega L}{R} $$

In the case of our Wireless Sensor Node, ensuring high efficiency is key to allowing for maximized battery life. As the efficiency increases less power will be dissipated as heat, and less energy will be needed to keep the node running.

#### Capacitor ESR

Capacitor ESR stands for "Equivalent Series Resistance". Much like the inductor DCR, it is the product of the material used, the manufacturing process of a capacitor, and other internal elements of the capacitor. In the case of capacitors this leads to parasitic inductance as well as general material resistance by the electrodes and dielectrics used to form the capacitor. Like the inductor DCR this leads to voltage drop and power dissipation through heat, which lowers the efficiency of our circuit.


#### Data


# Part C

#### Inductor Saturation

Inductor saturation is when the magnetic field created by the inductor is no longer able to hold additional charge. The occurrence of which is dependent on the core material of the inductor.