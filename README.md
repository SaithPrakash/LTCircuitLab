# LTCircuitLab
A curated collection of Linear Integrated Circuit (LIC) simulations and projects using LTSpice. Includes schematics, analysis, and simulations for various LIC applications
# Experiment-1
Question : If the circuit has a power of 50µ, how would you go about performing DC, transient, and AC analysis? Also, what do you think would happen if we vary the width of each MOSFET?;

Aim : To find DC operating point,find gain using transient analysis and AC analysis.

Components : CMOSN,resistors,DC power supply.

Theory : A Common-Source (CS) Amplifier is a fundamental MOSFET-based circuit used for voltage amplification. It operates in the saturation region, where a small input voltage variation at the gate controls a larger drain current. A load resistor at the drain develops the output voltage, making the amplifier suitable for signal processing. Key components include a MOSFET, biasing resistors, coupling capacitors, and a power supply. The amplifier's gain, bandwidth, and stability depend on MOSFET parameters and circuit design, with width variations affecting current drive and frequency response.

Procedure :

# design

![Screenshot 2025-02-17 200405](https://github.com/user-attachments/assets/53d45bdb-205c-4e6d-b9c6-a3122078f882)


# case 1:

• Establish the circuit connections.

• Connect a 1kΩ resistor (RD) to the drain of the MOSFET.

• Apply a 0.9V voltage source to the gate of the MOSFET, with its source terminal grounded

• Connect a 1.8V voltage source (VDD) to the resistor RD.

• Set the MOSFET's channel length to 180n and width to 1u.

• Conduct DC analysis, transient analysis, and AC analysis by applying a sine wave to the gate voltage source.

 # case 2:

•Consider the power as 50u and calculate the drain current (Id).

•Set the MOSFET's length to 180n and adjust the width until the calculated Id value is achieved.

•Perform DC analysis, transient analysis, and AC analysis by applying a sine wave to the gate voltage source.

# Case 1

1) DC ANALYSIS:

   ![Screenshot 2025-02-17 211010](https://github.com/user-attachments/assets/74eee6de-e002-48d0-8c8e-9a9a19f633e4)

    Values obtained from the DC Analysis are shown inthe  Figure below  : 

   ![Screenshot 2025-02-17 200351](https://github.com/user-attachments/assets/fc439d2e-1c06-4b6c-9344-d9f24dede37f)


2) Transient Analysis:

   V2 is a sine wave with a DC offset of 0.9V, an amplitude of 50m, and a frequency of 1kHz.
   
   Graph:
   
   ![Screenshot 2025-02-17 200845](https://github.com/user-attachments/assets/da201a75-05e8-4ea2-a519-cac1c2460dd4)
   
3) AC Analysis:

   ![Screenshot 2025-02-17 212743](https://github.com/user-attachments/assets/96573cc0-c1bf-44f3-8e5c-1458212eb417)

   Graph:

   ![Screenshot 2025-02-17 201040](https://github.com/user-attachments/assets/98d60c16-0677-47e3-8a3c-cd6764a3e207)

# Case 2:

# Calculation:

Given power = 50u,
VDD = 1.8V,

Using the formula for power:
Power = Voltage × Current,

We can rearrange to find the drain current (Id):
P = VDD × Id
Id = P / VDD

Substituting the values:
Id = 50u / 1.8V

Id = 2.77 × 10-5 A.

1) DC ANALYSIS:

   ![Screenshot 2025-02-17 201436](https://github.com/user-attachments/assets/26320d82-548d-4676-a3b4-8095b18565d6)

    Values obtained from the DC Analysis are shown in The Figure below  : 

   ![Screenshot 2025-02-17 201457](https://github.com/user-attachments/assets/3c7ed655-4d6d-41b7-a3fd-b986560bbe52)

2) Transient Analysis:

   V2 is a sine wave with a DC offset of 0.9V, an amplitude of 50m, and a frequency of 1kHz.

   Graph:
   
   ![Screenshot 2025-02-17 202004](https://github.com/user-attachments/assets/0a07093a-384b-46bd-9c1c-3bf99b96d5d1)
   
3) AC Analysis:
   
   !![Screenshot 2025-02-17 212743](https://github.com/user-attachments/assets/5a6c213c-fd2e-4807-9c01-9e68ed3a2afd)

   Graph:

   ![Screenshot 2025-02-17 202153](https://github.com/user-attachments/assets/a3598e5a-857d-4529-9f14-4f339b42c21f)

# Result

1) DC Analysis:

•The calculated drain current (Id) aligns with the expected value based on the given power and voltage, with Id = 1.52735 × 10-4 A.
•By adjusting the MOSFET’s channel dimensions (length = 180n and width = 1u), the required current was successfully achieved.
•The circuit operates as expected under DC conditions.

2) Transient Analysis:

•The transient response graph illustrates the circuit’s behavior over time.
•The response is smooth, without any unexpected delays or distortions.
•The circuit shows good responsiveness to changes, indicating stability.

3) AC Analysis:

•The AC response graph confirms that the circuit stays stable across different frequencies.
•The gain (4.8 dB) at 50u power and the phase shift (almost 180°) are in line with theoretical predictions.
•The circuit consistently performs well across the tested frequency range.

# Inference

•The experiment shows that by choosing the right size for the MOSFET, we can easily control the drain current.

•Impact of Adjusting the Width:
The width of M1 has a direct effect on Id. When the width is increased, the drain current (Id) goes up, and when the width is reduced, Id goes down.
The circuit worked well in all three types of analysis—DC, transient, and AC—proving that it’s stable and reliable.

•In the end, the design performed as expected, aligning with the theory, and showing that it's practical.









