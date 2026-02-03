# Sega Nomad MAIN Reproduction PCB
Reproduction of the Sega Nomad's main board, created from scans provided by Villahed94, Sega's documentation, and community knowledge of the FC1004 style Genesis.
Additional features include TMSS bypass jumpers, SMS support and 32X support.

IMAGES

# Build Notes
These PCBs are tested to work with with a stock VENUS SUB pcb, building these requires skills in microsoldering, QFP soldering, hot air rework, and Mega Drive troubleshooting.
It is highly recomendded you start with a set of known working parts from a donor mega drive. VA1, VA1.8 and VA3 model 2 sega genesis can provide all of the nescecary custom chips needed for this build.
Support is not officilly provided by neither RGBeter nor Villahed94 with building or debugging these PCBs.

# Production Notes
While Sega utlized a 2 layer PCB for the Nomad, it is best to order these as a 4 layer PCB in order to improve noise across the board
If you wish NOT to include the SRES bypass, add the following bodge wires in order to connect the original 315-5684 based SRES circuit.
IMAGE

# BOM
Most of, if not all parts can be directly transplanted from a donor Nomad Main board, however, some alterations have been made, and they are as follows:

R5 + R6, FM DAC limiting resistors best changed to 0 ohms when modding audio

All large MLCC capacitors can have their value increased to 10uF to improve noise

|Component|Value|Note|
|:--------|:----|:---|
|IC1|PLCC 68000|CPU|
|IC2|68K RAM|WORK RAM|
|IC3|FC1004/FF1004|MAIN ASIC|
|IC4|VIDEO RAM|VRAM|
|IC5|QFP Z80|Z80 CPU|
|IC6|Z80 RAM|ZRAM|
|IC7|LM809|SRES BYPASS ONLY|
|C1|10uF|1206 X7R|
|C2|10uF|1206 X7R|
|C3|10uF|1206 X7R|
|C4|47pF|0603 C0G 315-5708 ONLY|
|C5|100pF|0603 C0G|
|C6|100pF|0603 C0G|
|C7|22pF|0603 C0G|
|C8|1000pF|0603 C0G|
|C9|N/A|DOES NOT EXIST|
|C10|100pF|0603 C0G|
|C11|100pF|0603 C0G|
|C12|33pF|0603 C0G|
|C13|N/A|DOES NOT EXIST|
|C14|10uF|1206 X7R|
|C15|10uF|1206 X7R|
|C16|10uF|1206 X7R|
|C17|10uF|1206 X7R|
|C18|10pF|0603 C0G|
|C19|47pF|0603 C0G|
|C20|10uF|1206 X7R|
|C21|33pF|0603 C0G DO NOT POPULATE|
|C22|100pF|0603 C0G|
|C23|33pF|0603 C0G|
|C24|100pF|0603 C0G|
|C25|0.1uF|0603 X7R|
|C26|0.1uF|0603 X7R|
|C27|0.1uF|0603 X7R|
|C28|N/A|DO NOT POPULATE|
|C29|100pF|0603 C0G|
|C30|0.1uF|0603 X7R|
|C31|N/A|DOES NOT EXIST|
|C32|N/A|DO NOT POPULATE|
|C33|N/A|DOES NOT EXIST|
|C30|1uF|0603 X7R SRES BYPASSS ONLY|
|CE1|47uF 6v|SMD ELEC, CAN REPLACE WITH TANTALUM|
|CE2|47uF 6v|SMD ELEC, CAN REPLACE WITH TANTALUM|
|CE3|100uF 6v|SMD ELEC, CAN REPLACE WITH TANTALUM|
|CE4|47uF 6v|SMD ELEC, CAN REPLACE WITH TANTALUM|
|D1|SOD-923 DIODE|SRES BYPASS ONLY|
|OSC1|MCLK OSCILATOR, SQUARE PACKAGE|CHECK REGION|
|R1|150R|0603|
|R2|220R|0603|
|R3|2.2K|0603|
|R4|220R|0603|
|R5|0R|0603 DAC LIMITING RESISTOR|
|R6|0R|0603 DAC LIMITING RESISTOR|
|R7|2.2K|0603|
|R8|4.7K|0603|
|R9|100R|0603|
|R10|100R|0603|
|R11|2.2K|0603|
|R12|2.2K|0603|
|R13|5.6K|0603|
|R14|5.6K|0603|
|R15|5.6K|0603|
|R16|4.7K|0603|
|R17|4.7K|0603|
|R18|4.7K|0603|
|R19|1.2K|0603|
|R20|1.2K|0603|
|R21|1.2K|0603|
|R22|4.7K|0603|
|R23|1.0K|0603|
|R24|330R|0603|
|R25|330R|0603|
|R26|2.2K|0603|
|R27|100K|0603|
|RA1|4.7K|5X1206 BANK|
|RB1|2.2K|4X0603 BANK|
|RB2|100R|4X0603 BANK|
|RB3|100R|4X0603 BANK|
|RB4|100R|4X0603 BANK|
|RB5|100R|4X0603 BANK|
|RB6|100R|4X0603 BANK|
