# Sega-Nomad-MAIN-Reproduction-PCB
Reproduction of the Sega Nomad's main board, created from scans provided by Villahed94, Sega's documentation, and community knowledge of the FC1004 style Genesis.
Additional features include TMSS bypass jumpers, SMS support and 32X support.

Build notes

# Production Notes
While Sega utlized a 2 layer PCB for the Nomad, it is best to order these as a 4 layer PCB in order to improve noise across the board

# BOM
Most of, if not all parts can be directly transplanted from a donor Nomad Main board, however, some alterations have been made, and they are as follows:

R5 + R6, FM DAC limiting resistors best changed to 0 ohms when modding audio

All large MLCC capacitors can have their value increased to 10uF to improve noise

|Component|Value|Note|
|:--------|:----|:---|
|C1|10uF|1206 X7R|
|C2|10uF|1206 X7R|
|C3|10uF|1206 X7R|
|C4|47pF|0603 C0G 315-5708 ONLY|
|C5|100pF|0603 C0G|
|C6|100pF|0603 C0G|
|C7|X|0603 C0G|
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
