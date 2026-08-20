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

19 Augest 8AM - 10AM (2HR)

After few search and findings i made my matrix small now it is 8 x 8 means 8 rows with 8 coloumns using 16 gpio pins of nice nano and oled matrix was 14 x 5 using 19 gpio pins of nice nano with no encoder so i saved 3 pin

<img width="474" height="661" alt="image" src="https://github.com/user-attachments/assets/b29d83e9-c949-4c41-9fe1-f9dc89cde321" />
now this is 8 x 8 and include 61 keys of keyboard and one encoder

and i still have few pins left so i add a oled display
<img width="375" height="275" alt="image" src="https://github.com/user-attachments/assets/97cb640e-89c2-43c5-89e1-164ad0ab8564" />

i am trying to make a wireless keyboard so i searched for resources this is what i find this is for split keyboard but still helpfull
<img width="714" height="635" alt="image" src="https://github.com/user-attachments/assets/fbde6394-ce88-490b-a174-58f308eed9d8" />


<img width="1035" height="462" alt="image" src="https://github.com/user-attachments/assets/4ad58056-b887-41f4-85a7-456a8b819d9e" />
my connection of nice nano , olded and battry connector and on off switch

20 Aug 2026 9AM - 11AM

I started component placement today and i am stuck with placing keyswitch footprint at correct place (placing keyswitches in a row or coloumn) tutorial say use grid size 19.05 but that not worked for me then i did grid size of 19.05/8 and then it worked so i placed my keyswitchs , nice nano and display

<img width="1186" height="424" alt="image" src="https://github.com/user-attachments/assets/49a9634f-d173-40ad-a507-266f16d36983" />
i also placed diodes on bottom side to save space on top so it is easy to wire them later

<img width="1292" height="430" alt="image" src="https://github.com/user-attachments/assets/89fb3dba-e458-4834-8ade-35833d1e6537" />
after that i placed all the capacitor and skmini led on bottom side , i started with top placement but i find out that they are bottom mounted






