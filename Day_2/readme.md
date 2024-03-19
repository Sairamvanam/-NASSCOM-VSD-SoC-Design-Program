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
