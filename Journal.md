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



25 Aug 2026 8 - 12 AM


<img width="1393" height="519" alt="image" src="https://github.com/user-attachments/assets/9ee94542-e761-4509-9c4e-f21cb802d93c" />

thing got bad here because of my key matrix so now its hard to route

<img width="1179" height="436" alt="image" src="https://github.com/user-attachments/assets/bc06e081-6314-4c58-b239-9873b0fd1b70" />
then i routed keyswitches , led capacitors with eachother and it is hard because of my 8x8 matrix so i used bottom layer for routing row, led, diodes, capacitor and resistor and routing coloumns on top layer, it is like connect two wires vertically use top layer , if horizontally use bottom layer

i will say use 14x5 matrix routing will be easy

<img width="923" height="596" alt="image" src="https://github.com/user-attachments/assets/12d5e3ca-80b8-4979-bcb2-936f48289a59" />
then i connect routed nice nano with help of this
<img width="993" height="673" alt="image" src="https://github.com/user-attachments/assets/af27ce58-9017-4fbd-9b1d-adcf8f182d14" />

<img width="1494" height="527" alt="image" src="https://github.com/user-attachments/assets/6ab2880d-c839-43ff-9812-78da712dac6b" />
completed with jst connector for battery and a slider tu turn on and off


26 AUG 2026 9-11


<img width="796" height="540" alt="image" src="https://github.com/user-attachments/assets/d0f6e992-d33f-4b60-9cc3-ebe422f40572" />
SO I poured GND on my top and bottom layer
<img width="1366" height="562" alt="image" src="https://github.com/user-attachments/assets/c14be00e-83dd-438d-8e44-30f6798970e7" />
<img width="236" height="323" alt="image" src="https://github.com/user-attachments/assets/e0b314bd-1b41-41d2-9f3f-7db48d105af0" />
as u see a small area is left on bottom side of nice nano because of that red thing on nice nano that act as a anteena

<img width="1204" height="566" alt="image" src="https://github.com/user-attachments/assets/a4a8a81a-ae4e-4cab-9ff4-b9b794cadd8e" />
<img width="996" height="393" alt="image" src="https://github.com/user-attachments/assets/76b5257e-324c-4df2-8d04-271cd05c64ee" />
size of my keyboard


<img width="799" height="606" alt="image" src="https://github.com/user-attachments/assets/56f60bd9-b186-41be-8232-af214facb9ee" />
<img width="612" height="474" alt="image" src="https://github.com/user-attachments/assets/f2c79fec-cb9d-4be3-bef8-7fa5e6281e88" />

i got this error but i think this is issue of footprint 

<img width="1144" height="224" alt="image" src="https://github.com/user-attachments/assets/dcfe3690-8b0b-4b99-b637-6d74e1efd96f" />
<img width="1043" height="678" alt="image" src="https://github.com/user-attachments/assets/f064c2cb-5fc2-4b80-b5da-9979e6e3eec4" />
<img width="1289" height="243" alt="image" src="https://github.com/user-attachments/assets/6a1b00ea-e7ed-4ee0-83d9-3bfb424337e5" />
i read some documentation and found out we need to short rst with gnd to programe it so i do that
<img width="649" height="329" alt="Screenshot 2026-05-28 235440" src="https://github.com/user-attachments/assets/72009db4-d37a-45af-9d06-9fa4d2371d13" />

27 AUG 2026 8 - 9

<img width="813" height="681" alt="image" src="https://github.com/user-attachments/assets/408e8264-0337-47f4-b5ed-6d42bf26b647" />
Added 3d modal
<img width="1114" height="715" alt="image" src="https://github.com/user-attachments/assets/34f5cbc3-bb4f-4674-806b-6c653d0bc340" />
this have 2 pins on place of my led i think this modal internally include leds so i change this to

<img width="404" height="648" alt="image" src="https://github.com/user-attachments/assets/ad92c349-0c27-4e25-9b6c-f86690e0b3f6" />
this is new modal

<img width="1356" height="503" alt="image" src="https://github.com/user-attachments/assets/bf9733c1-2136-4320-8baa-a14401b4de64" />
overall

then i add other thing display , nano and other modal

<img width="1308" height="507" alt="image" src="https://github.com/user-attachments/assets/272dce06-2241-494e-a175-4bf22d45a07f" />

29 Aug 2026 4 hr

<img width="1399" height="533" alt="image" src="https://github.com/user-attachments/assets/645e2e9a-0ee0-488f-821f-8094fc35f15a" />
added random silkscreen quotes

<img width="1041" height="664" alt="image" src="https://github.com/user-attachments/assets/75f818dc-1cf1-465f-833e-a60b2a112a85" />
then i export 3d file step of this keyboard and import in onshape so that i can desigin my encloser case around it

<img width="1374" height="589" alt="image" src="https://github.com/user-attachments/assets/4d1dd9e4-4caa-4ec7-8263-c9b02034be21" />


<img width="1483" height="694" alt="image" src="https://github.com/user-attachments/assets/303c6a77-133b-45f6-96e5-6fa2a58be81d" />
after imorting in onshape i make a plane just below the top plane and then using project tool make a base for pcb

<img width="1458" height="686" alt="image" src="https://github.com/user-attachments/assets/3336ce91-e14c-4a61-aeb8-117f4b3ab78a" />
i also projected walls and mounting holes on this plane by project tool and pcb 

<img width="1308" height="636" alt="image" src="https://github.com/user-attachments/assets/49845d31-3c12-4d4a-a02d-95a68901913f" />
this is base or bottom part of my keyboard with extruted mounting holes this will make pcb float 

<img width="1379" height="662" alt="image" src="https://github.com/user-attachments/assets/70215568-4f5c-4ce5-9ea7-edc9abb89050" />
then i added keycap modals as it was difficult to work with raw keyswitches so this is my keyboard with electronics and base

<img width="1563" height="736" alt="image" src="https://github.com/user-attachments/assets/9df28671-c388-4f2c-8559-9d884858a861" />
then i make a sketch above top plane according to my pcb leaving space for keycaps encoder and display 
<img width="1526" height="745" alt="image" src="https://github.com/user-attachments/assets/24b09d86-0c1b-4a5d-9514-b78a7ec4a3be" />
this is top plate
<img width="1417" height="750" alt="image" src="https://github.com/user-attachments/assets/4742eb5a-8143-4d54-9bb6-5524fdedfaba" />
top plate with pcb
<img width="1536" height="773" alt="image" src="https://github.com/user-attachments/assets/0569ba1e-82fe-4942-a31d-891efe1484b5" />
whole thing together










