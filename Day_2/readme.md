#  Chip Floor Planning considerations
### 1. Define Width and height of core and die 
![image](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/66ba399f-a413-43fc-82e7-2d9330e032e2)
![Screenshot (85)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/f39ef017-9a36-473e-b7a8-49e198ff7901)
![Screenshot (86)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/c00e85f7-eb31-4d34-9810-d0ebb3590160)
![Screenshot (87)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/7a37cc23-bb68-437a-99a7-e29a8e4188f5)
![Screenshot (88)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/394e0cc9-c540-4022-99f2-5f7fd49dede1)
![Screenshot (90)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/7e415b9c-cb69-49b3-a019-5231b44992ab)

The circuit which we design will sit in the core area.Initially we must keep some space in the core area because few more cells will be added in CTS and Routing stages.for this reason,we usually mention U.F in range of 0.6 to 0.8 .
### Utilization Factor
It is defined as the ratio of **area occupied by the netlist ** to **Total area of the core**.   
generally, we mention U.F = 0.6 that means  60% is used for placing the cells and remaining 40% is used for routing purpose.
If u.f = 1 ,then it means that core is completely occupied and addition of extra cells is not possible.
### Aspect Ratio
It is defined as ratio of Height and Width.
Aspect Ratio decides the shape. If A.R =1 ,that signifies Square shape.If A.R is other than 1 It will be Rectangle.
![Screenshot (94)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/b3821c1f-3d50-4eec-8621-1a354e0659e4)
![Screenshot (96)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/41834b1a-b766-4258-bf53-d7d3d2f17340)
from above figure,
U.F = 2 unitts X 2 units / 4 units X 2 units 
    = 4/8 => 0.5 
    =>50 %

### 2. Concept of Pre-Placed Cells
![Screenshot (97)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/c2c90a2f-4640-423b-8b13-43578573cfe4)
![Screenshot (98)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/000beb37-dda0-42ed-b552-a0473bfecc3a)
![Screenshot (99)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/aa87324c-4712-402f-8af3-6e39c7456f45)

The position of Pre -placed cells are fixed by the user.EDA tool cannot change the position of these cells and it cannot replace these cells automatically. These cells are placed before the PNR .
The prr placed cells are implemented Once and can re-use as many times required in the design.
**black box :** we cannot see the internal circuit,we only know the input and output ports of the design.
### 3. Decoupling Capacitors
![Screenshot (106)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/adefb33a-b3d9-419b-be20-a678d6cdd0dd)

### 4. Powerplanning
![Screenshot (113)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/111780a6-fe9c-4271-9c7b-9fd4a559d5c2)

### 5. pin placement
![Screenshot (117)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/773d8bd8-cd33-43b1-bbaa-7dbadc5e5356)
![Screenshot (118)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/d89d3191-d02b-4dff-ab56-69a177eeca11)
![Screenshot (119)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/46234b67-08e9-4ccf-90c4-2dd86f308abe)
![Screenshot (122)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/2bbdd3cf-eb12-4db8-8c16-5376f248c9f5)
![Screenshot (125)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/a9c9f41c-35aa-482b-a626-1cee2808df13)

