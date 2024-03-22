## Cell Design and Characterization Flow
A standard cell, refers to a pre-designed and characterized logic cell that performs a specific function. These cells are used as building blocks for designing more complex digital circuits. Standard cells are typically characterized by their functionality, timing characteristics, power consumption, and area. 
![Screenshot (131)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/0c782b64-cded-43d8-af1f-683be5b31f89)
![Screenshot (133)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/b7a008be-031b-4fe8-80f5-097baf31a434)
Library consits of different cell with different functionality as-well-as different sizes and of different threshold voltages.
## Cell design Flow
cell design flow is divided into 3 stages.These stages are:

1.Inputs : These are the inputs that you need to design our Inverter.

2.Design steps : Then finally we will design the Inverter.

3.Output : Outputs of the inverter are the one that we actually use by the EDA tools.
![Screenshot (134)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/042bb1bf-4ea0-437b-ad39-01f2a33dc77f)
![Screenshot (139)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/61f60748-58df-4f5b-bd6e-ee5496690099)
![Screenshot (140)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/3d8b748e-c773-4afe-9f68-fcc2878e5de9)

 Design steps divideded into # parts:
 circuit design --->  In tis step we will implement the required functionality and prefer proper Pmos nad Nmos such that the library requirements are met.
 Layout design ---> In this step,after drawing cmos circuit, we place the transistors such that thet meet the euler's path.
 **eulers's path :** path which is only traced once.
 ![Screenshot (144)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/6c607fc7-0e84-46d6-a6d4-6b409a08fe9f)
![Screenshot (149)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/8af8f79e-b808-4f9a-a96f-b8e52e75b3d6)
![Screenshot (147)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/06502be6-4c76-4a77-85e6-a57771f57c6d)
![Screenshot (149)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/cd061976-0604-4975-abb7-1598edbd5d12)
Output stage also consists of the GDSII file, LEF and extracted spice netlist file that helps in determining the Time, noise and power characterstics of the circuit.
![Screenshot (150)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/e1c050e3-f798-4bfb-b1f1-eccc865a927a)
![Screenshot (154)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/bfee0033-94ad-4269-9deb-2ce0e0464962)
![Screenshot (157)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/28622c04-ea24-4e48-bffb-8f2d92c30a0b)
![Screenshot (158)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/bcf95f45-13b5-440a-a309-a78bd6477957)
![Screenshot (159)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/0f0645d8-a9f0-4986-a00c-acc60b9e2f55)
![Screenshot (163)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/b454710b-b295-4282-9f58-4445dee2de0b)
![Screenshot (161)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/0f52bc35-6b9e-493b-a9e2-d244ab69f9e9)
![Screenshot (162)](https://github.com/Sairamvanam/-NASSCOM-VSD-SoC-Design-Program/assets/163321291/33ee8a06-0e10-4e69-8104-82b7e3d1099c)
