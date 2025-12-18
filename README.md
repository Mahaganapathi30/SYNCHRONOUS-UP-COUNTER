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

<img width="1920" height="1080" alt="Screenshot 2025-12-17 194917" src="https://github.com/user-attachments/assets/93c8d005-b192-4261-ad32-0063b2e2c500" />


/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:
*/

**RTL LOGIC UP COUNTER**


<img width="1920" height="1080" alt="exp 11 RTL diagram" src="https://github.com/user-attachments/assets/a07ce64a-8773-405c-b642-22a03dc49c39" />

**TIMING DIAGRAM FOR IP COUNTER**


<img width="1920" height="1080" alt="exp 11 waveform" src="https://github.com/user-attachments/assets/4d28b9ba-2ee5-4945-b0f9-cf1c819af7d9" />


**TRUTH TABLE**


![exp11](https://github.com/user-attachments/assets/b832034d-6aac-426b-a0a0-792ee6b80f84)


**RESULTS**

Thus the program was implement 4 bit synchronous up counter and validate functionality.



