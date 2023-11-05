#### 4.1
- Discusses signals, analog circuits, and amplfiers
- Magnitude of an analog signal can take on any value with value and vary, IE CT signal
- Analog Circuits process analog signals 
- Linear Amplifier creates an output signal directly proportional to the input signal, which has been magnified.
- Chapter coves analysis and design of linear amps using MOSFETS.
- Small Signal analysis allows us to linear the ac equivalent circuit.
- Use super position to solve dc and ac analysis of linear amps.
- Use graphical technique, dc load line, and ac load line.
>[!error] Key Relationships
>
>- i<sub>D1</sub> = i<sub>D2</sub> | if Biasing into Saturation region, to solve for a variable the current through both MOSFETs must be the same, thus we can set the equations of iD equal to one another and solve for the unknown.
>- 


>[!summary] 4.1 Summary
>
>This chapter goes over 


#### 4.1.1

- Transistor must be biased in SATURATION for the output voltage to be a linear function of input voltage.
- TOTAL G to S voltage is the sum of V<sub>GSQ</sub> and V<sub>i</sub>. 
- As Vi increases, the instantaneous value of v_gs increases, and the bias point moves up the load line.
- A larger v<sub>GS</sub> creates a larger drain current and a smaller v<sub>DS</sub>
- For the negative v<sub>i</sub> (NEGATIVE PORTION OF SINE WAVE), the instantaneous value of v<sub>GS</sub> goes below the [Quiescent Value](Quiescent.md)
- Smaller V<sub>GS</sub> m equals smaller drain current and increased v<sub>DS</sub>
- 

![[Fig41NeamanAnalysis.png]]
![[FIGURE42NEAMANCIRCUITANALYSIS.png]]