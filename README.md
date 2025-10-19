### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**
<img width="313" height="293" alt="image" src="https://github.com/user-attachments/assets/caac4f42-1649-4baf-8a4a-0ba8d71b557b" />

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:25009524
*/

**RTL LOGIC UP COUNTER**
<img width="977" height="325" alt="image" src="https://github.com/user-attachments/assets/04f54747-636a-4e16-b676-6940f8dae1da" />

**TIMING DIAGRAM FOR IP COUNTER**
<img width="1060" height="664" alt="image" src="https://github.com/user-attachments/assets/db6b7d6c-db61-4334-b8ed-0db8ab309c88" />

**TRUTH TABLE**
<img width="707" height="359" alt="image" src="https://github.com/user-attachments/assets/be20aa89-33e6-4571-ae59-060430b1bb32" />

**RESULTS**
