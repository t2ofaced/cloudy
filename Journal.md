17 Augest 2026 5 PM - 6 PM ( 1hr )

First of all I am really sorry for my bad english this is not my first/second language. And i do not know how this thing works all this github etc  

I want to make a 60% keyboard like thiss

<img width="794" height="344" alt="image" src="https://github.com/user-attachments/assets/f700b3b3-78ac-48dd-bd87-bcb29ebb8fc9" />

but with few extra thing like e link display, encoders and extra buttons along with this 60% keyboard in short combination of keyboard and a hackpad like this

<img width="569" height="418" alt="image" src="https://github.com/user-attachments/assets/42fa07b5-7894-43c9-aef5-9c48c27d9b51" />

<img width="1280" height="705" alt="image" src="https://github.com/user-attachments/assets/4413d74e-2d8e-4730-bcb1-3f9b79b99005" />

resources i used

Thought about RPI ZERO 2 W as most keyboard or hackpad i see use this but i wanted a wireless keyboard which means i need to add battery stuff charging discharging etc on pcb that will inc cost and complexity so i am using nice nano
<img width="801" height="438" alt="image" src="https://github.com/user-attachments/assets/f8e9d08d-0fe0-48b0-9755-3bf975c01b03" />
<img width="641" height="635" alt="image" src="https://github.com/user-attachments/assets/ddbb03fc-718a-48d7-a4bd-6304392896b1" />
this is soo cool

also things i want from this keyboard - wireless , rgb , e link display and encoders and few function keys like in a hackpad


18 Augest 9 - 11 pm ( 2hr )

I research and i found what i am using so for keyswitches 
<img width="837" height="238" alt="image" src="https://github.com/user-attachments/assets/0628a38b-1d01-406c-8da3-03a5caba85be" />
mx solderable 
RGB
<img width="505" height="346" alt="image" src="https://github.com/user-attachments/assets/1a18b56d-2d38-42bf-96ee-199a8e30e546" />
Sk6812 mini

stared with my 14 X 5 matrix for my 60% keyboard
<img width="925" height="405" alt="image" src="https://github.com/user-attachments/assets/b500e745-df7d-417e-aa51-61362e6a4ef5" />
plce 1n4148 diodes for anti ghosting , it is to stop weird thing when press 2 key at same time this take very long time 

then leds
<img width="1335" height="657" alt="image" src="https://github.com/user-attachments/assets/5263cb55-ef12-4880-9aa2-58d23e33c83e" />
here i use 1 bulk capacitor and 1 ceramic capacitor with each led this one also take long time

This took around 2 hr as i placed 61 keys , capacitors , diodes and leds
ohh no when i see i need display, encoder and function btn too but now i dont have gpio pin of nice nano to connect my things i need to search about it




