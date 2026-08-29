# Project-LAS: A Low-cost, Sustainability-friendly Security Design for Urban Communities
Origin: Operational extension of the STEM Framework at the UNESCO Center for Peace Summer Camp
Global Framework: UN Sustainable Development Goal 11(Sustainable Cities) and SDG 10 (Reduced Inequalities)
Core Hardware: Analog Solid State BC547 NPN Architecture

## Executive Summary and Design Philosophy

The motive behind this project extends back to a UNESCO summer program I attended on July/August 2025. The STEAM (STEM) classes were centered around considering how STEM based solution could be used to tackle SDGs. Our first session involved a short simple presentation of any idea that aims to solve an SDG; My team presented an underwater plastic filtration robot.
I was aware that the idea we proposed was idealized and loses appeal when evaluating the hurdles involved with developing solutions to environmental problems, but its focus on tackling problems related to the world around us was undeniable.
As the end of the class approached, I felt more and more exposed to the tangible and radical side of STEAM. I also got to see and control a miniature robot using code, which was fun.

Somewhere in the beginning of the summer of 2026, I started to play around with an electric circuit project that I had competed with within my team. I examined the parts. I was reminded of how widely available and cost-effective the parts and design we used were. Then, while I was using AI to better understand my academics, the idea came to mind:
I have seen and heard that security measures in underdeveloped areas have high costs as a barrier to addressing the safety and wellbeing of the residents. I could illustrate the electric circuit design and make it publicly available.
It could contribute to sustainable urban development. I think Project LAS has the potential to make protection more accessible and its simplicity makes it easier to distribute and maintain.

## Physical Fabrication & System Prerequisites
<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/d02c3acf-ca92-44d8-a682-35925b9d1119" />

During the assembly of the electric circuit, my team had gathered the material prerequisites: A wood board for a platform, a suitable battery, a laser module, an LDR, and LDE and 5V buzzer, a BC547 transistor, fixed resistor, three mirror shards and bottle caps, and copper wires. We had used screws to fasten the bottle caps; a hot glue gun for the mirrors shards; and a soldering tool to connect all the electrical components.
The soldering tool needed to be periodically powered on and off, to maintain the optimal temperature melting temperature without damaging the circuit. We applied the molten metal methodically to ensure the soldered joints would be structurally competent. It was handled with great caution, as it was capable of irritating skin and causing heat-burns in the case that the molten metal makes contacts with skin.
The mirrors need to be aligned to reflect the laser light at an incident angle of 45 degrees to surround the house on the quadrilateral sides, which makes it a suitable example for common living spaces which are rectangular, and minimize changes in the reflected light’s elevation. The selected LDR required the full illumination of the low-power laser, so we needed to align it with high-precision. 
We pierced bottle caps in the center and calibrated the positions of the mirror shards before holding them in place to be fixed with hot glue. The materials we used were common and mostly cheap, making it an accessible technology for communities. Afterwards the laser still had minor misalignments, so we gradually corrected the angular deviations as a final measure by gently pressing the shards in different directions.

## Semi Conductor Physics & Circuit Logic
<img width="920" height="607" alt="image" src="https://github.com/user-attachments/assets/95e2918b-1592-4aa2-adc2-00369b4a5e12" />

The transistor is used as a switch: in which the Buzzer, LED bulb, and LDR are connected in series to the Collector Terminal. Meanwhile the Base Terminal and the LDR are connected in parallel to each other, setting up a current divider circuit between them. 
While the switch is closed and the laser is not obstructed, photons -from the laser- incident on the LDR cause the electrons in the Silicon atoms to jump from the valance band to the conduction band. This increases the number density, n, of charge carriers which leads to a decrease in the LDR’s Resistance, R, with reference to the transport equation (I = nAeV) and ohm’s law (R = I / V). 
When the laser is blocked by a hand(trespasser), the LDR’s Resistance will increase due to the decrease in light intensity. The increase in Resistance will lead to less current flowing through the LDR and a greater current moving through the Base Terminal of the transistor. The increased current flowing through the Base Terminal allows more current to flow through Buzzer and LED bulb to the Collector Terminal. As a result, the light and sound from the LED and Buzzer will alert the homeowner.


## Diagnostic Calibration & Environmental shielding

We noticed that the despite the laser being completely unobstructed, there was some current leaking through the LDR and causing the buzzer and LED to still trigger with minor intensity. We suggested that it could be due to the laser not having sufficient light intensity. 
A potentiometer can be used as a counter-measure. It would be placed in-front of the Base terminal allowing us to adjust the total resistance across the fixed resistor. This, in turn, allows us to adjust the current flowing through the LDR. By calibrating the variable resistor so that current doesn’t leak into the Base Terminal while the laser is incident on the LDR, the transistor will restrict current from flowing to the Collector terminal. The buzzer and LED will stop receiving power when there’s no intrusion and therefore optimize the signal-to-noise ratio.
The LDR was also exposed to ambient lighting, which may have lowered the baseline resistance of the LDR; since ambient lighting is not predictable, however; the circuit will reduce dependence on the environment its used, if it is shielded from ambient lighting. As a result, the signal-to-noise ratio will remain consistent regardless of the presence or absence external light sources and the system will be more reliable.

