---
title: "cloudy"
github: "https://github.com/t2ofaced/cloudy"
description: "A custom designed 60% Keyboard that  usesnice nano v2 clone pro micro nrf52840 development board as mcu becuause it give me freedom of wireless kayboard this keyboard also includes 1 enoder and 1 display and it is fully rgb thanks to SK6812MINI-E SMD leds and its pcb is desigined in kicad and case in Onshape"
created_at: "2026-09-09"
total_time: "26h 36m"
---

# August 17, 2026: 5:00 PM - 6:00 PM
<!-- fabricate:entry 998 -->

First of all I am really sorry for my bad english this is not my first/second language. And i do not know how this thing works all this github etc  

I want to make a 60% keyboard like thiss

<img width="794" height="344" alt="image" src="https://fabricate.hackclub-assets.com/cb0532c15c41d5ebda941edaee37e7a45b1d9e2d4e8d4bf51b2caf787912a4ea/image-png/f700b3b3-78ac-48dd-bd87-bcb29ebb8fc9.png" />

but with few extra thing like e link display, encoders and extra buttons along with this 60% keyboard in short combination of keyboard and a hackpad like this

<img width="569" height="418" alt="image" src="https://fabricate.hackclub-assets.com/d2f7a705200c3cafba3f793b415a0bf4159856581b63a583eadb4ee80f30105d/image-png/42fa07b5-7894-43c9-aef5-9c48c27d9b51.png" />

<img width="1280" height="705" alt="image" src="https://fabricate.hackclub-assets.com/9da7ccdfcba3f88906d72dcd880159530b93cb2fa0e1b7325a6fd239f0390bca/image-png/4413d74e-2d8e-4730-bcb1-3f9b79b99005.png" />

resources i used

Thought about RPI ZERO 2 W as most keyboard or hackpad i see use this but i wanted a wireless keyboard which means i need to add battery stuff charging discharging etc on pcb that will inc cost and complexity so i am using nice nano

<img width="801" height="438" alt="image" src="https://fabricate.hackclub-assets.com/82b05158dfcfeac02fb4fb4ed448b277bce90fa64917888ade4914ac70aaf98d/image-png/f8e9d08d-0fe0-48b0-9755-3bf975c01b03.png" />

<img width="641" height="635" alt="image" src="https://fabricate.hackclub-assets.com/ca53e3d096ab025d11c2536609c2801c9c7ca6f97a96732602114d90420eb8d8/image-png/ddbb03fc-718a-48d7-a4bd-6304392896b1.png" />

this is soo cool

also things i want from this keyboard - wireless , rgb , e link display and encoders and few function keys like in a hackpad

**Total time spent: 1h**

# August 18, 2026: 9:00 PM - 11:00 PM
<!-- fabricate:entry 999 -->

I research and i found what i am using so for keyswitches 

<img width="837" height="238" alt="image" src="https://fabricate.hackclub-assets.com/286a8c6b4d2616b9a3830f6e71cac72c471af86be5175c164d744dc79aab986e/image-png/0628a38b-1d01-406c-8da3-03a5caba85be.png" />

mx solderable 
RGB

<img width="505" height="346" alt="image" src="https://fabricate.hackclub-assets.com/a7cd45bda2261ad675dc955d0c2c716dcd05f8288b94ba958e11c7b8505baed9/image-png/1a18b56d-2d38-42bf-96ee-199a8e30e546.png" />

Sk6812 mini

stared with my 14 X 5 matrix for my 60% keyboard

<img width="925" height="405" alt="image" src="https://fabricate.hackclub-assets.com/4053972e9ab817e447361064d4ed08e1b28fed4f84bdaa62fb9c63f66679c9a8/image-png/b500e745-df7d-417e-aa51-61362e6a4ef5.png" />

plce 1n4148 diodes for anti ghosting , it is to stop weird thing when press 2 key at same time this take very long time 

then leds

<img width="1335" height="657" alt="image" src="https://fabricate.hackclub-assets.com/280244aab9238eb786551438e79f4be42c4ed25dca6e585d26861c87ca3efa39/image-png/5263cb55-ef12-4880-9aa2-58d23e33c83e.png" />

here i use 1 bulk capacitor and 1 ceramic capacitor with each led this one also take long time

This took around 2 hr as i placed 61 keys , capacitors , diodes and leds
ohh no when i see i need display, encoder and function btn too but now i dont have gpio pin of nice nano to connect my things i need to search about it

**Total time spent: 2h**

# August 19, 2026: 8:00 AM - 10:00 AM
<!-- fabricate:entry 1000 -->

After few search and findings i made my matrix small now it is 8 x 8 means 8 rows with 8 coloumns using 16 gpio pins of nice nano and oled matrix was 14 x 5 using 19 gpio pins of nice nano with no encoder so i saved 3 pin

<img width="474" height="661" alt="image" src="https://fabricate.hackclub-assets.com/0ce807b8c675947b3bd3823b6262c2888a399b1b430b52dd555681aec72761d7/image-png/b29d83e9-c949-4c41-9fe1-f9dc89cde321.png" />

now this is 8 x 8 and include 61 keys of keyboard and one encoder

and i still have few pins left so i add a oled display

<img width="375" height="275" alt="image" src="https://fabricate.hackclub-assets.com/18d0836f4100bc07423a73926268be850405794ed45665652870d99c56f10cfe/image-png/97cb640e-89c2-43c5-89e1-164ad0ab8564.png" />

i am trying to make a wireless keyboard so i searched for resources this is what i find this is for split keyboard but still helpfull

<img width="714" height="635" alt="image" src="https://fabricate.hackclub-assets.com/6e086b48ca073d5429f212bdb9efbc69bf0f02bced429e977b63293fd6ce67f0/image-png/fbde6394-ce88-490b-a174-58f308eed9d8.png" />

<img width="1035" height="462" alt="image" src="https://fabricate.hackclub-assets.com/36921acdce157e47285b3a5c6a16bac89f737524af084222f408db1c34b4f088/image-png/4ad58056-b887-41f4-85a7-456a8b819d9e.png" />

my connection of nice nano , olded and battry connector and on off switch

**Total time spent: 2h**

# August 20, 2026: 9:00 AM - 11:00 AM
<!-- fabricate:entry 1001 -->

I started component placement today and i am stuck with placing keyswitch footprint at correct place (placing keyswitches in a row or coloumn) tutorial say use grid size 19.05 but that not worked for me then i did grid size of 19.05/8 and then it worked so i placed my keyswitchs , nice nano and display

<img width="1186" height="424" alt="image" src="https://fabricate.hackclub-assets.com/7fe2cb10a9225070515df2b5e19a4714c095c7d321802dc9b880bf668a006655/image-png/49a9634f-d173-40ad-a507-266f16d36983.png" />

i also placed diodes on bottom side to save space on top so it is easy to wire them later

<img width="1292" height="430" alt="image" src="https://fabricate.hackclub-assets.com/dbb972f55e02a0c8fa91c286f7d9288dcce991487739aa45168339386910fa38/image-png/89fb3dba-e458-4834-8ade-35833d1e6537.png" />

after that i placed all the capacitor and skmini led on bottom side , i started with top placement but i find out that they are bottom mounted

**Total time spent: 2h**

# August 25, 2026: 8:00 AM - 12:00 PM
<!-- fabricate:entry 1002 -->

<img width="1393" height="519" alt="image" src="https://fabricate.hackclub-assets.com/1312b040620f7573c74bbca8d9204e98c460ea7b88ef9b6b355a45f7e1ee7d3f/image-png/9ee94542-e761-4509-9c4e-f21cb802d93c.png" />

thing got bad here because of my key matrix so now its hard to route

<img width="1179" height="436" alt="image" src="https://fabricate.hackclub-assets.com/9babe8d65db7cc3d0b284e396a0b823391882648b2d6581868c64f12b61d1f82/image-png/bc06e081-6314-4c58-b239-9873b0fd1b70.png" />

then i routed keyswitches , led capacitors with eachother and it is hard because of my 8x8 matrix so i used bottom layer for routing row, led, diodes, capacitor and resistor and routing coloumns on top layer, it is like connect two wires vertically use top layer , if horizontally use bottom layer

i will say use 14x5 matrix routing will be easy

<img width="923" height="596" alt="image" src="https://fabricate.hackclub-assets.com/219aa373eda1cb646870819a0d442fe2f8962710961aa87419a361b0152f8945/image-png/12d5e3ca-80b8-4979-bcb2-936f48289a59.png" />

then i connect routed nice nano with help of this

<img width="993" height="673" alt="image" src="https://fabricate.hackclub-assets.com/69ec10d92041afaa6e41f74e934f4cd6834c016a7d03c9cb143a0f96630ce5b2/image-png/af27ce58-9017-4fbd-9b1d-adcf8f182d14.png" />

<img width="1494" height="527" alt="image" src="https://fabricate.hackclub-assets.com/7220135db9fe425f3f5b87c2eafe1b41bbe0bfe8a96c9394890c82dccf915282/image-png/6ab2880d-c839-43ff-9812-78da712dac6b.png" />

completed with jst connector for battery and a slider tu turn on and off

**Total time spent: 4h**

# August 26, 2026: 9:00 AM - 11:00 AM
<!-- fabricate:entry 1003 -->

<img width="796" height="540" alt="image" src="https://fabricate.hackclub-assets.com/9449166126f53b1be125e193d81e6125d71af7f1ee27c44cfd97a98fef8efac3/image-png/d0f6e992-d33f-4b60-9cc3-ebe422f40572.png" />

SO I poured GND on my top and bottom layer

<img width="1366" height="562" alt="image" src="https://fabricate.hackclub-assets.com/7fa1ac2ff35c12a2304c47f927cb3d7e87455c74c7ef5c6da20142b01b3facbe/image-png/c14be00e-83dd-438d-8e44-30f6798970e7.png" />

<img width="236" height="323" alt="image" src="https://fabricate.hackclub-assets.com/b52d6535f5f1a418b678f555fe1a7f780110a415b29ee154603ae9c27e1903cf/image-png/e0b314bd-1b41-41d2-9f3f-7db48d105af0.png" />

as u see a small area is left on bottom side of nice nano because of that red thing on nice nano that act as a anteena

<img width="1204" height="566" alt="image" src="https://fabricate.hackclub-assets.com/c0ce71f05c12d56f77be75daa01eb1a0b915c3d04ed06d4d2f1e6abb72b99010/image-png/a4a8a81a-ae4e-4cab-9ff4-b9b794cadd8e.png" />

<img width="996" height="393" alt="image" src="https://fabricate.hackclub-assets.com/a3e3e30b47091fca5cda239870cafd8312e127695061ea0bd31abe507e9da0db/image-png/76b5257e-324c-4df2-8d04-271cd05c64ee.png" />

size of my keyboard

<img width="799" height="606" alt="image" src="https://fabricate.hackclub-assets.com/2103e151daa897f89fb5eafebb68e77c06d5bd41309a68cc3bde2f66817504fb/image-png/56f60bd9-b186-41be-8232-af214facb9ee.png" />

<img width="612" height="474" alt="image" src="https://fabricate.hackclub-assets.com/75dc583dad2465d8f04f1b40da971963365404fbc389b70a24e714bf5f4048b5/image-png/f2c79fec-cb9d-4be3-bef8-7fa5e6281e88.png" />

i got this error but i think this is issue of footprint 

<img width="1144" height="224" alt="image" src="https://fabricate.hackclub-assets.com/edc764acb5c79e60e81c5ccbf74c603bb71db7ade8688232cc394850df9f1f20/image-png/dcfe3690-8b0b-4b99-b637-6d74e1efd96f.png" />

<img width="1043" height="678" alt="image" src="https://fabricate.hackclub-assets.com/ee91ec4f176cfa5b385e046afcde7df73f54991b3406d0349de7b740341364ae/image-png/f064c2cb-5fc2-4b80-b5da-9979e6e3eec4.png" />

<img width="1289" height="243" alt="image" src="https://fabricate.hackclub-assets.com/c9ba72617182deb9be86adfb5f2c211cf0fe2e442fa52fa1a8e6be2df619ba31/image-png/6a1b00ea-e7ed-4ee0-83d9-3bfb424337e5.png" />

i read some documentation and found out we need to short rst with gnd to programe it so i do that

<img width="649" height="329" alt="Screenshot 2026-05-28 235440" src="https://fabricate.hackclub-assets.com/b64d0b8821d9634348f372d21c217e5f9621c80bf1ab1732cf6403ca085c6223/image-png/72009db4-d37a-45af-9d06-9fa4d2371d13.png" />

**Total time spent: 2h**

# August 27, 2026: 8:00 AM - 9:00 AM
<!-- fabricate:entry 1004 -->

<img width="813" height="681" alt="image" src="https://fabricate.hackclub-assets.com/aec044d1fdc085401db0f80a766ae82c8fef0e8554cf0cdf1bcfd9707d0d357b/image-png/408e8264-0337-47f4-b5ed-6d42bf26b647.png" />

Added 3d modal

<img width="1114" height="715" alt="image" src="https://fabricate.hackclub-assets.com/4e99b3cc53fe399b6b8515d2d4c7010dacd2133edb4ed40fd413e630e11a555a/image-png/34f5cbc3-bb4f-4674-806b-6c653d0bc340.png" />

this have 2 pins on place of my led i think this modal internally include leds so i change this to

<img width="404" height="648" alt="image" src="https://fabricate.hackclub-assets.com/036ae00170475c7d2e64105f6bdc3d987d3b73c073537152521f4f43430b6e58/image-png/ad92c349-0c27-4e25-9b6c-f86690e0b3f6.png" />

this is new modal

<img width="1356" height="503" alt="image" src="https://fabricate.hackclub-assets.com/bb166c667b3afe7a14156e2f1d831f6f74da97ade8327c9472668ba0b4e53f2d/image-png/bf9733c1-2136-4320-8baa-a14401b4de64.png" />

overall

then i add other thing display , nano and other modal

<img width="1308" height="507" alt="image" src="https://fabricate.hackclub-assets.com/156dd2cc55553da54dae39d468b0962fd9b91526df08002eed97acd4fd293a45/image-png/272dce06-2241-494e-a175-4bf22d45a07f.png" />

**Total time spent: 1h**

# August 29, 2026: random hrs
<!-- fabricate:entry 1005 -->

<img width="1399" height="533" alt="image" src="https://fabricate.hackclub-assets.com/e9fea93ac01021cf3ef380260897786a7297c97a7fa3653cdc537e7d85978f7f/image-png/645e2e9a-0ee0-488f-821f-8094fc35f15a.png" />

added random silkscreen quotes

<img width="1041" height="664" alt="image" src="https://fabricate.hackclub-assets.com/2f4759810778da025dbdce33fc2f60d82e0a30daa7f4356139753941e66b59d9/image-png/75f818dc-1cf1-465f-833e-a60b2a112a85.png" />

then i export 3d file step of this keyboard and import in onshape so that i can desigin my encloser case around it

<img width="1374" height="589" alt="image" src="https://fabricate.hackclub-assets.com/eb103fb47a691d2bde64b21bcdb45ccabcd1c40bda87b7e01e500fb923121413/image-png/4d1dd9e4-4caa-4ec7-8263-c9b02034be21.png" />

<img width="1483" height="694" alt="image" src="https://fabricate.hackclub-assets.com/f1efdaed38263ef9a07b7b772f89f423cc40f54995ce79f8ea132832fb086b0e/image-png/303c6a77-133b-45f6-96e5-6fa2a58be81d.png" />

after imorting in onshape i make a plane just below the top plane and then using project tool make a base for pcb

<img width="1458" height="686" alt="image" src="https://fabricate.hackclub-assets.com/01866529a6e2f1f2f9da95179160e0b4b83748334ddac95ec2fda5ea17ae2a73/image-png/3336ce91-e14c-4a61-aeb8-117f4b3ab78a.png" />

i also projected walls and mounting holes on this plane by project tool and pcb 

<img width="1308" height="636" alt="image" src="https://fabricate.hackclub-assets.com/ce200378a79fb9156282dc1a7ae474a2d9740d2a1bb75ae49b3022ace8d81c78/image-png/49845d31-3c12-4d4a-a02d-95a68901913f.png" />

this is base or bottom part of my keyboard with extruted mounting holes this will make pcb float 

<img width="1379" height="662" alt="image" src="https://fabricate.hackclub-assets.com/48f30c477bd1e74116f91ba7d4886c02c026bc952670209b6a44c387a1321b6e/image-png/70215568-4f5c-4ce5-9ea7-edc9abb89050.png" />

then i added keycap modals as it was difficult to work with raw keyswitches so this is my keyboard with electronics and base

<img width="1563" height="736" alt="image" src="https://fabricate.hackclub-assets.com/a000b6578e9175419806b60be9a3a3e32cab523cd364ca65d8b11e662ed04b48/image-png/9df28671-c388-4f2c-8559-9d884858a861.png" />

then i make a sketch above top plane according to my pcb leaving space for keycaps encoder and display 

<img width="1526" height="745" alt="image" src="https://fabricate.hackclub-assets.com/80f99c604ebffd216fce31e9ee6a34d71cb53cf69a11da85fd86577631cb3f01/image-png/24b09d86-0c1b-4a5d-9514-b78a7ec4a3be.png" />

this is top plate

<img width="1417" height="750" alt="image" src="https://fabricate.hackclub-assets.com/073e95273c0542bcf966f47411643553ae0a168b9a1804524fe6f36599f0f76e/image-png/4742eb5a-8143-4d54-9bb6-5524fdedfaba.png" />

top plate with pcb

<img width="1536" height="773" alt="image" src="https://fabricate.hackclub-assets.com/783d1cf83538f62f6c7a2a281bf68faa9d0c56cf31895413d13095cc7d887990/image-png/0569ba1e-82fe-4942-a31d-891efe1484b5.png" />

whole thing together

**Total time spent: 4h**

# September 1, 2026: 9:00 AM - 1:00 PM
<!-- fabricate:entry 1006 -->

so i forget about type c hole in my keyboard case so i did that

<img width="1301" height="625" alt="image" src="https://fabricate.hackclub-assets.com/081d9ea2a6aa45a92e325a49cca1b4983da0868a4a0de5ad1f5cc5549aef42a6/image-png/bb0f2693-0052-4b2e-8bb0-4410f7d3b0c5.png" />

<img width="1395" height="625" alt="image" src="https://fabricate.hackclub-assets.com/12f9457d0488983d6dd10551ff725e6bb7848c256e4a6f8ae444bbee70d3af62/image-png/858783bb-aa6a-426a-a753-84b3c7bd97ec.png" />

then i searched about firmware first i thought i will go with zmk as it is popular and nice nano suggest this

<img width="1162" height="625" alt="image" src="https://fabricate.hackclub-assets.com/75e1f67c6ed9571c20fa4275d4a4aa4a5ccb6ac395a338180ce58e605bb64cec/image-png/3a529ef0-a082-4a09-8f13-515bc171b362.png" />

<img width="999" height="667" alt="image" src="https://fabricate.hackclub-assets.com/3ea2a8b74cb439189026e71ae1c3b5ef8ae05cc9b86d081bcc6e78ff32a018d5/image-png/e6e022d8-4ee4-4f3d-aeb5-7df57ecbf0fd.png" />

but keeb website sugeests rmk so i searched about that too and i decided to move on with rmk

<img width="828" height="668" alt="image" src="https://fabricate.hackclub-assets.com/0257177f5e00c587ba8b4e5457088fe02002ebdb7d4c000106e5061f2a6be43f/image-png/12af6669-3255-417e-abc0-0e5d664caf16.png" />

i used this rmk project template repo on github i used it as a template and made a new github repo

<img width="1348" height="639" alt="image" src="https://fabricate.hackclub-assets.com/66463d7f9acdda880601c88bc240aba2b72b9e7fa87d54fc58db29c02c6cf76e/image-png/06b8dff2-4517-422c-a2fa-e838ee467fe0.png" />

<img width="1173" height="634" alt="image" src="https://fabricate.hackclub-assets.com/d1c9154ee42d10575e7131fda412f0fb8f33317c7e77932479c188945538c49f/image-png/d910592b-565c-4181-aecf-a54fcf5de0e8.png" />

default config of this file
i updated it according to my config 

<img width="796" height="571" alt="image" src="https://fabricate.hackclub-assets.com/e5be2185a803c12f77928af291abee7b70d4b9faf9cbf8b33194362d2692f70f/image-png/524037ac-521c-4df9-a604-9263c5a147a8.png" />

<img width="1413" height="941" alt="image" src="https://fabricate.hackclub-assets.com/9ef39120cf0c4bb5ec98c6fbd8687c7dd8e73138c8701fa4278e2f94b85fe51d/image-png/51c1f294-eaf4-41ca-b779-1d50ffaf346b.png" />

<img width="1401" height="459" alt="image" src="https://fabricate.hackclub-assets.com/8b96fd26fb2545fdbc099e6ad8704ec406026c60f45db218690747f919160bef/image-png/8e1f6d52-59ba-423a-8dee-1f85c7948014.png" />

gave error and i debug it

<img width="1131" height="648" alt="image" src="https://fabricate.hackclub-assets.com/7168634457a7c70d4ef896d616c87bbcee1b0bd44148dab16920ed9e8fd3c476/image-png/77982ccf-fd98-4d72-9847-8cdc20b9e6e9.png" />

some spelling error it was

<img width="1188" height="664" alt="image" src="https://fabricate.hackclub-assets.com/bc9374fa29d4a7fb2098298759f3adc6b50493eab392f4fc45c45ca194f46f23/image-png/a98a37b7-c37f-42b1-8ec9-a7e678aa28bc.png" />

so now it is completed uf2 file is actual firmware 

**Total time spent: 4h**

# September 5, 2026: 10:30 AM - 12:00 PM
<!-- fabricate:entry 1007 -->

so first i search all the component i need and made a bom.csv and put all the component and price in the bom.csv file 

<img width="1519" height="925" alt="image" src="https://fabricate.hackclub-assets.com/f92e928688b1693c61bf7e1573f6a7733f6df86388a20df1346bab3d19122987/image-png/0d4d7f15-5a03-4ea5-886f-e0bbe36eda2b.png" />

and when i was searching component i found that my bulk cap need some space so i removed some part of my top plate

<img width="807" height="382" alt="image" src="https://fabricate.hackclub-assets.com/1aaaac316b9385fa615a89e3bf910b5ac21c97128930a2c2d9d625b3502a5df4/image-png/1de23a02-4ab6-4358-b80f-e7c08dfd65e1.png" />

<img width="647" height="553" alt="image" src="https://fabricate.hackclub-assets.com/bae9702956608035acaaacf2fa95c5090b8134b2d2418dcf8793366a0d559db1/image-png/60a734d4-6d65-4ece-8c61-f70a7e2b8485.png" />

<img width="506" height="340" alt="image" src="https://fabricate.hackclub-assets.com/b558300bff09f79792a82d9f669bf91a4df529943924773bfd78a3e059f8181a/image-png/1d8d362b-1c4f-4008-a112-b988dce89eec.png" />

and then exported and updated my repo 
also made my Journal better

**Total time spent: 1h 30m**

# September 8, 2026: 3:00 PM - 6:00 PM
<!-- fabricate:entry 1008 -->

So i found that my keyboard is too big to print in most common 3d printers so i sliced it in 2 parts so now i have total 4 parts 2 for top plate and 2 for base plate

<img width="1305" height="558" alt="image" src="https://fabricate.hackclub-assets.com/66ea96ecf6d241c6e6709107065c2f8b37a3859f97096538c366998ce11595f9/image-png/d084eca7-90e6-4bff-b460-831b2b36a7cf.png" />
This is Base-A left part of Base plate

<img width="1201" height="518" alt="image" src="https://fabricate.hackclub-assets.com/5c5303b5503da0dd9cff7ac448e8d371f7e17d06601c0f12e6f3396adecdc656/image-png/365d9750-9625-4185-ac72-d6c2620c7d49.png" />
This is Base-B right part of Base plate

<img width="1217" height="604" alt="image" src="https://fabricate.hackclub-assets.com/175c93e40a67d67cee05949d552b851bcb2a82fd5105456ca56feb1b3ee88f72/image-png/192cd7f3-b401-4165-b982-cf305629d441.png" />
This is Base plate A and B part with each other

<img width="1415" height="809" alt="image" src="https://fabricate.hackclub-assets.com/c02759e2e0a3edff18eee1f5dc96d879ec2c53100172eb46ea8a6650ed61a6ed/image-png/a88b9afe-a3ac-4d48-9b48-669ce90531bf.png" />
This thing holds the A and B part with each other 


<img width="1157" height="529" alt="image" src="https://fabricate.hackclub-assets.com/e7e0298c6a7c088ed43cf3c75bfb7d91829f55e69b1c8f100f3d77fce2db5de6/image-png/4eedcdd9-2eb3-44de-b47d-589b3bb0dbba.png" />
This is Top-A left part of Top plate

<img width="1289" height="625" alt="image" src="https://fabricate.hackclub-assets.com/bce62767b709db23a282132a089537b69630cb848d53ee34976e02a9e883db6b/image-png/b26e20c6-dbda-4898-8304-31f29fbd0d00.png" />
This is Top-A left part of Top plate

<img width="1368" height="669" alt="image" src="https://fabricate.hackclub-assets.com/eb0e01ad142a83d21c7787c003949b589368da49ab74650ebc0c4a9cfd570f00/image-png/263f44bd-bc6d-43c9-9467-01b2a132519c.png" />
This is Top plate A and B part with each other

<img width="1173" height="603" alt="image" src="https://fabricate.hackclub-assets.com/36c515e20f21ba1cf4e683868a906336be14bf3686307698e1acf488824b0785/image-png/1b5bc090-fb96-45f2-a696-b6c9a780a963.png" />
This thing holds the A and B part with each other 

I hope this is the final change and update in this model


<img width="869" height="598" alt="image" src="https://fabricate.hackclub-assets.com/adea87c99a3b823dd4eda7adccceb4dc0d86a19362152422c32d1809aa265530/image-png/c25d1d5d-775c-4613-ab9f-7275df9d2d40.png" />
<img width="720" height="591" alt="image" src="https://fabricate.hackclub-assets.com/ceb2a1d0b236ee0aa12ff851787da0dae7a95504cf417172e24cff0d6c8d6020/image-png/b8f3ea33-c7bb-4132-b40e-2b181260596d.png" />

afther that i reviwed PCB routing and made some high current track thick

<img width="1258" height="688" alt="image" src="https://fabricate.hackclub-assets.com/a4669464abbe428674d058876ee041517b61a45406b811dc1a76c7f54840c90d/image-png/225493bd-a8c8-442d-b0c4-d6f5b353202c.png" />
final one more rule check and manual review and done

**Total time spent: 3h**

# October 23, 2026: Updates
<!-- fabricate:entry 1111 -->

Uploaded .step of your entire assembly, including the pcb with the case and i was not able to lower the cost of this keeboard so , i will buy nice nano v2 myself which is around $8 so now my bom will be $124
![](https://fabricate.hackclub-assets.com/c153e77ca876c063d575440c3ea390ff88f2c3cbe12097099b0d0ff89a1ad5e4/image-png/image.png)
![](https://fabricate.hackclub-assets.com/d9ce0ba48f98d078bf9faacb92b1552f30f8a5ec2bfdc95c5284e91da786a2c6/image-png/image.png)

**Total time spent: 6m**
