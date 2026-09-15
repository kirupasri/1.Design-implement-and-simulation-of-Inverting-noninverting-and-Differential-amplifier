 /># 1.Design-implement-and-simulation-of-Inverting-noninverting-and-Differential-amplifier

**AIM:**
To design , implement and simulate  an inverting, non- inverting and differential amplifiers

**APPARATUS  and SOFTWARE REQUIRED:**
S.No	Name of the Apparatus	Range	Quantity
1.	Function Generator	3 MHz	1
2.	DSO	30 MHz	1
3.	Dual RPS	(0 – 30) V	1
4.	Op-Amp	µA741	1
5.	Bread Board		1
6.	Resistors	1K,10K	2
7.	Connecting wires and probes	As required	
8.  LT SPICE software

**THEORY:**
Op-amp in open-loop configuration has a very few application because of its enormous open-loop gain. Controlled gain can be can be achieved by taking a part of output signal to the input with the help of feedback. This is called as Closed- Loop Configuration. The three basic types of closed-loop amplifier configuration are:
1.	Inverting amplifier.
2.	Non-inverting amplifier.
3.	Differential amplifier.
The entire configuration can be operated with either AC or DC input.

**INVERTING AMPLIFIER:**
This is the most widely used op-amp. Here, the output voltage Vo is feedback to the inverting input terminal through the Rf – R1 network. The negative sign in gain indicates the phase shift of 180ο.
The circuit closed-loop voltage gain is Avcl= -RF / R1

**NON - INVERTING AMPLIFIER:**
If signal is applied to the non-inverting input terminal of op-amp without inverting the input signal such a circuit is called non-inverting amplifier. Here the output is feedback to the inverting input terminal. The phase shift of input signal does not occur in non-inverting terminal.
The circuit closed-loop voltage gain is ACL = 1 + ( RF / R1)

**DIFFERENTIAL AMPLIFIER**
A circuit that amplifies that amplifies the difference between two input signals is called as differential amplifier. It is useful in instrumentation amplifier. If the two input signals are the same, the output should be zero. Differential amplifier with a single op-amp has the exact gain of an inverting amplifier and it is given as
𝐴	= 	𝑉𝑜/(V2-V1) = −𝑅𝑓/R1

**DESIGN:**

**Inverting amplifier:**
    Gain is     A = -Rf/R1
        Take  A = 10
        Rf =10 R1
        Choose R1 = 1kΩ, Rf=10kΩ
        
**Non inverting amplifier:**
    Gain is    A = 1+ Rf/R1
      Take A = 2
      Rf = R1
      Choose Rf = 10kΩ, R1=10kΩ
      
**Differential amplifier**
  Gain is 𝐴=	𝑉𝑜/(𝑉1− V2)= − 𝑅𝑓/𝑅1
Take  A = 10
 Rf =10 R1
Choose R1 = 1kΩ, Rf=10kΩ

**PROCEDURE:**
**Inverting and Non-inverting amplifier:**
1.	Select R1 as a constant value and choose a value of Rf.
2.	Connect the circuit as per as the circuit diagram.
3.	Apply the constant amplitude input voltage to the circuit.
4.	Measure the output voltage amplitude for different value of V1 from DSO.
5.	Calculate the practical Voltage for different value of V1& compare it with theoretical output.
6.	Practical gain & theoretical voltage should be approximately equal.
7.	Plot the graph of the input wave versus output wave for any one practical case.
   
** Differential amplifier:**
1.	Select the value of R1, R2, R3 & Rf such that R1=R2 and R3=Rf.
2.	Connect the circuit as per as the circuit diagram.
3.	Provide constant input voltage Vin1 to Non-inverting terminal of op-amp through R1 & constant input voltage Vin2 to inverting terminal of op-amp through R2.
4.	Measure the output voltage using DSO.
5.	Calculate the theoretical Vo and compare it with practical Vo.
6.	Practical output & theoretical calculation should be approximately equal.
7.	Plot the graph of the input wave versus output wave for any one practical case.
 
**PIN DIAGRAM:**
<img width="623" height="293" alt="image" src="https://github.com/user-attachments/assets/b3b8c725-7db4-4256-b33e-611b52c75913" />


**INVERTING AMPLIFIER:**

  **CIRCUIT DIAGRAM**
<img width="776" height="378" alt="image" src="https://github.com/user-attachments/assets/949d82ff-be10-44cf-8908-093d455e9bd7" />


  **MODEL GRAPH:**
<img width="532" height="372" alt="image" src="https://github.com/user-attachments/assets/20b4d10a-f39e-466a-aeaa-ff7715492ec5" />


  **TABULATION:**
 
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/56257f72-e74c-400d-b1ef-c40810a183ce" />

**MODEL CALCULATION:**

**NON INVERTING AMPLIFIER:**
  **CIRCUIT DIAGRAM**
<img width="733" height="340" alt="image" src="https://github.com/user-attachments/assets/9090674b-aa87-4fbf-8243-2577c3bfaf2c" />


  **MODEL GRAPH:**
<img width="467" height="306" alt="image" src="https://github.com/user-attachments/assets/ce830b1b-9223-46a3-87e3-8c860bf16779" />


  **TABULATION:**
  
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/774ad5c2-9c2f-4dcd-b3f2-5d38a5832d68" />


  **DIFFERENTIAL AMPLIFIER:**
  **CIRCUIT DIAGRAM**


<img width="748" height="442" alt="image" src="https://github.com/user-attachments/assets/ef43798a-6bc6-412c-9b77-9c6ea5a4673c" />




  **MODEL GRAPH:**


<img width="722" height="315" alt="image" src="https://github.com/user-attachments/assets/d9f19d04-a4ba-481f-a60b-2e25e93350b7" />



  **TABULATION:**

<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/faf60a36-ffd3-43df-b9d5-410ed94d8bdb" />
**GRAPH:**
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/0d87feca-8800-4fa3-9c77-66a77601888a" />
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/bebd5fc4-b281-4b93-9601-88d8b6856b53" />

**LT-SPICE Tool:PROCEDURE:**
•	Double click on LT-Spice icon.
•	New schematic window open.
•	Pick and paste the required component from the library and draw the circuit diagram .
•	Complete the connection.
•	Save the file by giving file name.
•	Click on the run option ->click advanced open ->select Ac analysis->enter the amplitude time delay stop time value.
•	Click on the run option ->simulation window opens->place the probe ->output graph is obtained.
 
  **LT SPICE**
  **CIRCUIT and Waveform**
  <img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/c679eb08-8751-41df-a721-5f016ffa615d" />

<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/e8d3a646-44ec-4a3d-a8d5-bf19685330fb" />

<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/2e430dec-c053-4095-a786-cf4b3ca53688" />


**RESULT:**
Thus the Inverting, Non-Inverting and Differential Amplifiers are designed and simulated performance was successfully tested using op-amp IC 741 and LT SPICE.
 






