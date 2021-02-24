# Simulation of Memristors using PSPICE

In this repo I simulate the effect of 4th basic circuit element called "Memristor" using the following circuit.

![alt text](img0.png)

## Introduction
In 1971, Leon Chua hypothesized the fourth fundamental circuit component while attempting to build up a missing constitutive relationship between the electrical charge and the
magnetic flux to complete the symmetry. Chua named this speculative nonlinear gadget, memristor (memory + resistor) since it showed the hysteresis property of the-then
ferromagnetic center memory furthermore the dissipative qualities of a resistor. Plainly, in such gadgets, the nonlinear resistance can be remembered inconclusively by controlling the stream of the electrical charge or the magnetic flux. The memristor was proposed to have a memresistance, M and a function defined as dM=Mdq.

![alt text](https://github.com/Mr-TalhaIlyas/Memristor-Simulation-via-MATLAB/blob/master/screens/img1.png)



## Experiments

First make the PSPICE circuit of the above digram.

![alt text](img1.png)

MbreakP Specified Parameters:

![alt text](eq1.png)

Setting these values as follows:

![alt text](eq2.png)

DbreakZ as Zener diode with following parameters:

![alt text](eq3.png)

It gave the following shape of pinched hysteresis loop

![alt text](img2.png)

Curves of Vgs and Id are as follows;

![alt text](img3.png)

Modifying the above circuit for now as follows;

![alt text](img4.png)

It gives the following output of pinched hysterics loop;(Capacitor Initial Voltage=-3V)

![alt text](img5.png)

Curves of Vgs and Id are as follows;

![alt text](img6.png)

Looking closely why the current is zero from 0.36 secnds to 0.651 seconds lets look at the Vgs and Vds voltage curves (Here Vth=-1V)

![alt text](img7.png)

Above graph shows that form 0sec to 0.4 sec 

![alt text](eq4.png)

So,

![alt text](eq5.png)

Which means that the MOSFET is in Triode/Ohmic region, but after 0.4 sec as Vgs starts dropping from its peak value and falls below Vgs i.e.

![alt text](eq6.png)

Which means it goes into Cut-off region so;

![alt text](eq7.png)

![alt text](img8.png)

Between vgs – vthh and vds and Id seperate

![alt text](img9.png)

Vds vs Vgs and Vds vs Id