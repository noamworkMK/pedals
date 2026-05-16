 Pitch Shifter:

System Overview
A frequency-tracking pitch shifter  The design avoids digital DSP in favor of a CD4046 Phase-Locked Loop (PLL) and CD4017 decade counter 
for interval sequencing.

im very connected to music and rock culture, and its all started when i talked with my friend about how expansive effect pedal are. and then i thought, maybe i can build one, so from there i searched for like a month on how to buld them, about the electronics of the audio, and the logic. and i asked myself how can i make it. and then i found kicad as almost the only free softwere that worked for me, and i learned how to use it, this project has alot of versions some of them are really bad, but thats how i learned to design a pcb.

the pcb design: 
this pcb design had a lot of changes, at first i had a 2 layers board, unorgenised and to big to be in the enclouser, and then i made it smaller, changed some foorpeint, rerouthed the pcb, added fillings, and i almost sent it for prodaction like that. and then i felt that something is misssing, and that i wanted to create a intresting pedal that will be good and easy, so in this version i addad relay switch to create a bypass and added caps and, more diods, and resistors to protect the parts from overload, backcurent, and stuff that willl ruin the board. and i changed the board size and redone the traces again to finaly fit my expactation and the enclouser. 

<img width="3114" height="1338" alt="Screenshot 2026-05-09 135032" src="https://github.com/user-attachments/assets/63a81df6-2f90-4d47-830b-3afd8978d4ba" />
<img width="1295" height="902" alt="Screenshot 2026-05-15 005828 png" src="https://github.com/user-attachments/assets/5a3378ba-a735-4dc7-b8ec-c98351dbf16d" />
<img width="1330" height="1014" alt="pcb" src="https://github.com/user-attachments/assets/c5cc4fd4-c8e5-40df-81e8-5b9d05b6ea13" />

the leyers of the pcb: 
<img width="1324" height="932" alt="L-GREEN" src="https://github.com/user-attachments/assets/6bbf089f-e382-46de-ae71-1a9b3280feef" />
<img width="1325" height="998" alt="L-BLUE" src="https://github.com/user-attachments/assets/199aa695-f441-477e-b775-a908da01a40f" />
<img width="1316" height="985" alt="L-RED" src="https://github.com/user-attachments/assets/ab5c975e-f29c-433c-97fd-7c1255005b0b" />
<img width="1301" height="958" alt="L-ORANGE" src="https://github.com/user-attachments/assets/17b9d9a9-9f84-4b76-8586-0132ab82fa49" />






the circuit: 
The circuit takes an audio, signal shifts its pitch down and outputs it with 5 selectable pitch steps controlled by a push button. The core chips are a CD4046 (handles the pitch shifting) and a CD4017 counter (steps through the 5 settings). A TL072 op-amp buffers the input signal, and five NSL-32 optocouplers that i swiched to VTL5C4 in prodaction becouse of avilablity. this optocouplers (optical) do the switching between pitch steps without noise, becouse there is not current passing between them.


<img width="1611" height="1144" alt="scheamatic" src="https://github.com/user-attachments/assets/c6a03774-ad88-4ccd-a274-d73abba6a262" />

logic schematics:

<img width="1059" height="1025" alt="LOGIC SCH" src="https://github.com/user-attachments/assets/b07080de-3aaf-4bf6-bde1-3d3c836f4b88" />

audio schematics:

<img width="601" height="823" alt="audio SCH" src="https://github.com/user-attachments/assets/939c7b95-3fdb-4135-8a59-0fc52dcc8eba" />

the battery compartment: 
i sd designed a 9v battary compartment in solidworks that will fit exactly in the enclouser
<img width="1184" height="646" alt="Screenshot 2026-05-15 005842" src="https://github.com/user-attachments/assets/91b2a20d-0b5b-422a-867d-3d68458ede02" />

assembly:
i also created a 3d assambly of the pedal in solidworks, the assembly is partial becouse it would take me a lot of time to do every thing and its mainly for fitting and concepts. but the main parts are in there.

<img width="1755" height="1008" alt="assmbly 5" src="https://github.com/user-attachments/assets/85b83df0-8a6c-403d-8575-7b43fe38f763" />
<img width="1328" height="681" alt="assm2" src="https://github.com/user-attachments/assets/7e1c0bf6-dedd-4175-8403-46989ee03b46" />
<img width="1219" height="806" alt="essembly pitch" src="https://github.com/user-attachments/assets/558ade8d-1956-4d10-b7dc-31f65e264dd6" />

Technical Specifications:

Frequency Synthesis: CD4046 PLL tracks input frequency; CD4017 logic handles interval division/multiplication.
Analog Interface: VTL5C4 Vactrols integrated for smooth interval transitions.
Calibration: 5x 50k  trimmers for precise frequency offset tuning.
Input Stage: TL072 op-amp buffer for high-impedance guitar signal integrity.
Bypass: Relay-based switching system for transparent operation.

<img width="1227" height="961" alt="image" src="https://github.com/user-attachments/assets/a92dfc9a-b199-4dd4-9999-b63002b2a3c5" />
<img width="1199" height="727" alt="image" src="https://github.com/user-attachments/assets/49b96976-ef20-4f34-b6bd-00a8acf141f4" />
<img width="1219" height="806" alt="essembly pitch" src="https://github.com/user-attachments/assets/f64ec656-e651-43fe-94b4-35c75dd25dcc" />

