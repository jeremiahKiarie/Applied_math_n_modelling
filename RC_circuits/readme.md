## RC CIRCUIT MATH MODEL
In this folder, you will find a math model for RC circuits. <br>
We will be focusing on an RC discharging circuit as shown in the image below:
<div style="display: flex; align-items: center;">

  <img src="Resources\rc_discharge_circuit.webp" alt="RC Discharging Circuit" width = "300" style="margin-right: 20px;"/>
    <p style="max-width: 400px;">The circuit consists of a resistor (R) and a capacitor (C) connected in series, with the capacitor fully charged.</p>  
</div>

<script type="text/javascript" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>
Kirchhoff's voltage law states that the sum of the potential differences (voltage) around any closed loop in a circuit must equal zero.
Starting from the lower left corner and moving counterclockwise, we can write the equation for the circuit as follows:
$$ V_c + V_r = 0 $$

Where:
- $ V_c \quad \rightarrow \quad$ is the voltage across the capacitor
- $ V_r \quad \rightarrow \quad$ is the voltage drop in the resistor
Rearranging the equation gives us:
$$ V_c = -V_r $$   
Using Ohm's law, we can express the voltage drop across the resistor as:
$$ V_r = I \cdot R $$
Substituting this into the previous equation gives us:
$$ V_c = -I \cdot R $$
Electric current (I) is defined as the rate of flow of electric charge (Q) with respect to time (t).<br>
Now, we can express the current in terms of the capacitor's charge:
$$ I = \frac{dQ}{dt} $$
Substituting this into the equation gives us:
$$ V_c = -\frac{dQ}{dt} \cdot R $$
Capacitance $C$ is defined as the amount of electric charge $Q$ stored per unit voltage $V$ across the plates of a capacitor:
$$ C = \frac{Q}{V} $$
Rearranging this gives us:
$$ Q = C \cdot V $$
Thus, the voltage across the capacitor can be expressed as:
$$ V_c = \frac{Q}{C} $$
Substituting this into the equation gives us:
$$ \frac{Q}{C} = -\frac{dQ}{dt} \cdot R $$
Rearranging this equation leads us to the differential equation:
$$ \frac{dQ}{dt} + \frac{1}{RC} Q = 0 $$   
This is a first-order linear ordinary differential equation. The solution to this equation can be found using the method of separation of variables or integrating factor method. The general solution is given by:
$$ Q(t) = Q_0 e^{-\frac{t}{RC}} $$
Where:
- $ Q_0 \quad \rightarrow \quad$ is the initial charge on the capacitor at time $ t = 0 $.
The voltage across the capacitor can be expressed as:
$$ V(t) = \frac{Q(t)}{C} = \frac{Q_0}{C} e^{-\frac{t}{RC}} = V_0 e^{-\frac{t}{RC}} $$
Where:
- $ V(t) \quad \rightarrow \quad$ is the voltage across the capacitor at time $ t $.
- $ C \quad \rightarrow \quad$ is the capacitance of the capacitor.
- $ Q(t) \quad \rightarrow \quad$ is the charge on the capacitor at time $ t $.

The current in the circuit can also be expressed as:
$$ I(t) = \frac{dQ}{dt} = -\frac{Q_0}{RC} e^{-\frac{t}{RC}} = -I_0 e^{-\frac{t}{RC}} $$
Where:
- $ I(t) \quad \rightarrow \quad$ is the current in the circuit at time $ t $.
- $ R \quad \rightarrow \quad$ is the resistance in the circuit.