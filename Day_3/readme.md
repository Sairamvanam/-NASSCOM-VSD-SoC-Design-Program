## Design Library cell using Magic Layout and ngspice characterization
The below command will create an folder called vsdstdcelldesign in the openlane directory.
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/34ea9371-f812-4f11-8d02-582c57235150)
The file inside the vsdstdcelldesign are :
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/e71c7891-659f-415b-9480-4d1d58d7afd8)

Then we need to copy the tech file to the  vsdstdcelldesign folder.for that we use command 
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/a57c2640-e475-458e-8f28-32e308d1cbc2)
here we wont create an inverter from scrach,we will do spice extraction as well as post layout spice simulation of inverter design.
to invoke the layout in magic we use command **magic -T sky130A.tech sky130_inv.mag &** 
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/e2de3d5a-7d0d-4038-a6bb-727abe022a95)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/4816eb84-5885-4eae-8dd4-66a658840763)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/3705c2b2-caaf-4979-86cc-3ea67bb1d1c7)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/f31b49f4-3e9c-4750-ad53-1a06df1b5583)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/94a132ef-1b4e-4a4e-87bc-52de08eaffc1)
###  Inception of Layout A CMOS fabrication process
fabrication steps are : 
1.selecting a substrate
2.creating active regions for transistors
3.N-well and P-well formation
4.Formation od gate
5.Lightly droped drain formation
6.Source and drain formation
7.formation of interconnects
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/8e381926-ba30-4ade-ab52-d7fdbe0fc65f)
The above image shows th final output after following above all steps.

### Sky130 Tech File Labs
we can extract the .LEF files by using following commands:
extract all
ext2spice sky130_inv into sky130_inv.ext:
ext2spice

after execution of above commands we can se " sky130_inv.ext and sky130_inv.spice " in the vsdstdcelldesign folder.
the sky130_inv.ext file is containing the following contents
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/57d8b9dc-f8ce-470f-b664-bc969a0d0bc6)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/8f76ddeb-8589-4314-82c2-b4fd111a7563)
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/5aafa58e-e272-4af2-924b-143d19c1d48a)
