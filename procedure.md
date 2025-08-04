### Procedure

### COMPONENTS

Transistors, Bread board, resistors, capacitors, inductance coil, dc power supply, C.R.O, connection wires etc

<h3>1. DESIGNING</h3>

<p><strong>Selection of transistor:</strong> Use high-frequency transistor <strong>BF195</strong>, NPN transistor.</p>

<p><strong>Component specification:</strong></p>
<ul>
  <li><strong>I<sub>C</sub> (MAX):</strong> 30 mA</li>
  <li><strong>V<sub>CEO</sub> (MAX):</strong> 20 V</li>
  <li><strong>β<sub>MIN</sub>:</strong> 36</li>
  <li><strong>β<sub>MAX</sub>:</strong> 125</li>
</ul>


### Design of amplifier section

$\textbf{dc\ bias\ conditions}$ 
$$V_{CC} = 12\,V \qquad I_C = 1\,\text{mA}$$  
$$V_{CE} = 0.5 V_{CC} = 6\,V$$  
$$V_{RE} = V_E = 0.1 V_{CC} = 1.2\,V$$  
$$V_{RC} = V_C = 0.4 V_{CC} = 4.8\,V$$

### Design of $R_C$  

$$V_{RC} = I_C R_C = 4.8\,V \quad \text{then} \quad R_C = 4.8\,k\Omega \quad (\text{use 4.7k std})$$

### Design of $R_E$

$$V_{RE} = I_E R_E = 1.2\,V \quad \text{then} \quad R_E = 1.2\,k\Omega$$


### Design of $R_1$ and $R_2$.

$\text{Assume the current through } R_1 = 10 I_B \text{ and that through } R_2 = 9 I_B$

$$I_B = \frac{I_C}{\beta} = \frac{1\,\text{mA}}{50} = 20\,\mu\text{A}$$

$$V_{R2} = 9 I_B R_2 = V_{BE} + V_{RE} = 0.7 + 1.2 = 1.9\,V$$

$$R_2 = \frac{1.9\,V}{9 \cdot 20 \cdot 10^{-6}} = 9.1\,k\Omega \quad (\text{Select 10K std})$$

$$V_{R1} = 10 I_B R_1 = V_{CC} - V_{R2} = 12 - 1.9 = 10.1\,V$$

$$R_1 = \frac{12.8\,V}{10 \cdot 27 \cdot 10^{-6}} = 47\,k\Omega$$

**Selection of capacitors** :  All capacitor values may be taken 1μF

 

**Design of feedback network**: Required frequency of oscillation $f=455KHz$
$\text{We have Frequency of oscillation } f = \frac{1}{2\pi \sqrt{L_e C}}, \text{ where } L_e = L_1 + L_2$

$$\text{so,} \quad f = \frac{1}{2\pi \sqrt{L_e C}} = 455\, \text{KHz}$$

$$\text{Let } C = 0.1\,\mu F, \text{ then } L_{eq} = L_1 + L_2 = 1.22\, \mu H \quad (1\, \mu H \text{ std})$$


<h2>Procedure for simulator</h2>

<ol>
  <li>
    Begin by arranging the components on the virtual breadboard as shown in <strong>Animation 1</strong>. Refer to the visual guide carefully to place each component in its correct position.
  </li>

 
<div style="display: block; margin-left: auto; margin-right: auto; text-align: center; width: fit-content;"><img src="./images/connection1.gif" alt="Animation 1" style="max-width: 300px; height: auto;"><p style="text-align: center; font-size: smaller; font-style: italic;"></p></div>


  <li>
    To connect the components, click on one end of the wire and then click on the corresponding point on the breadboard to complete the connection. Repeat this step to interconnect all necessary components.
  </li>

  <div style="display: block; margin-left: auto; margin-right: auto; text-align: center; width: fit-content;"><img src="./images/connection2.gif" alt="Animation 2" style="max-width: 300px; height: auto;"><p style="text-align: center; font-size: smaller; font-style: italic;"></p></div>
  
  <li>
    Follow the <strong>connection diagram</strong> to ensure the circuit is completed correctly. Double-check that all connections are made as shown in the schematic.
  </li>
  <li>
    Once the circuit is fully connected, click the <strong>"Show CRO"</strong> button in the simulator interface. This will display the waveform output on the virtual Cathode Ray Oscilloscope (CRO).
  </li>
</ol>


<h3>To Change the Component Value</h3>

<ol>
  <li>
    Select the component whose value you want to modify by clicking on it within the simulator.
  </li>
  <li>
    Use the slider on the right-hand side of the simulator to adjust the value (e.g., resistance, capacitance) as needed for the experiment.
  </li>
</ol>

<h2>Result</h2>

<p>
  Amplitude and frequency of sine wave from Hartley Oscillator = …… V, …… Hz.
</p>


<h3>WORKING</h3>
<p>The connections are made as shown in fig.</p>


<div style="float: right; margin-left: 20px; display: flex; flex-direction: column; align-items: center;">
<img src="./images/figure2.jpg" alt="Figure 2" style="max-width: 300px; height: auto;"> <p style="text-align: center; font-size: smaller; font-style: italic;"></p> </div>


<p>The collector of the transistor is connected to the positive terminal of the power supply (V<sub>CC</sub>) through the resistance R<sub>C</sub>. The resistances R<sub>1</sub> and R<sub>2</sub> are connected in series with the power supply. The resistance R<sub>E</sub> and the capacitor C<sub>E</sub> are connected in the emitter circuit. The negative terminal of the power supply and emitter resistance R<sub>E</sub> is earthed.</p>

<p>An inductance coil L connected in parallel with the capacitor C forms the tank circuit. The centre tap of coil L is earthed.</p>

<p>After making connections, the power supply is switched on. The frequency of oscillations is measured using a C.R.O.</p>


