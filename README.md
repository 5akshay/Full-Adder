# Full-Adder
Using gate diffusion Input
# Design 10T Full Adder using Modified Gate Diffusion Input Technique.
This repository presents the Design of Full Adder ckt using 28nm CMOS Technology and tool used is Synopsis Custom Compiler.
# Table Of Content
- [Abstract](https://github.com/5akshay/Full-Adder/blob/main/README.md#Abstract)
- [Circuit Details](https://github.com/5akshay/Full-Adder/blob/main/README.md#Working)
- [Tool Used](https://github.com/5akshay/Full-Adder/blob/main/README.md#Tool-Used)
- [Full Adder Ckt using GDI technique](https://github.com/5akshay/Full-Adder/blob/main/README.md#CMOS-Inverter-Gate)
- [Buffer Ckt](https://github.com/5akshay/Full-Adder/blob/main/README.md#CMOS-XOR-Gate)
- [Parity Generator Testbench Design](https://github.com/5akshay/Full-Adder/blob/main/README.md#Parity-Generator-Testbench-Design)
- [Simulated Waveform]https://github.com/5akshay/Full-Adder/blob/main/README.md#Simulated-Waveform)
- [Schematic Netlist](https://github.com/5akshay/Full-Adder/blob/main/README.md#Schematic-Netlist)
- [References](https://github.com/5akshay/Full-Adder/blob/main/README.md#References)
- [Acknowledgements](https://github.com/5akshay/Full-Adder/blob/main/README.md#Acknowledgements)

# Abstract
Full adder circuit may be a important element within the style of application of integrated circuits in VLSI. the look and analysis of Full Adder cell exploitation the modified Gate Diffusion Input (MGDI) technique on optimizing the facility, delay and Power Delay Product (PDP). this system (MGDI) permits reducing power, delay and space of digital circuits, whereas maintaining low complexness of logic style. Through investigation is disbursed for the effectiveness exploitation combination of various low power full adder circuit style techniques. the most objective of those full adders is providing high-speed and low power consumption conjointly provides sensible voltage swing.

# Circuit Details
One of the significant differences between GDI & CMOS based structure is that, instead of connecting VDD & Ground to the source of PMOS & NMOS respectively, input signals are given in GDI cell. The basic GDI cell was suggested by Morgenshtein. It has three input terminals: G (gate input by PMOS & NMOS shorted), P (source input of PMOS), and N (source input of NMOS). GDI based full adder architecture depicted in Fig can be divided into two parts. In the first stage, XOR & XNOR function are generated. The XOR gate (M1, M2, M3, M4), uses less number of transistors as compared to conventional design of XOR gate using CMOS logic, which results in improving the overall performance. In Fig M1, M3, M5, M7, M10 are PMOS transistors and M2, M4, M6, M8, M9 are NMOS transistors. Both the bulks of PMOS & NMOS are connected to source.
- Truth Table
![IMG20220218174656__01](https://user-images.githubusercontent.com/100522966/156021375-95a4c002-123b-486d-bb41-f6431148d66b.jpg)

- The truth table can be verified with the help of following calculations


![image](https://user-images.githubusercontent.com/100522966/156019591-67a3fc94-c704-463d-94dc-8878aa3cd674.png)

Coming to the CMOS Design , I designed xor gate with the help 
of 2 transistors and for each xor gate there is need of one 
complementary input which is designed with the help of inverters. 
For 4 bit Parity generator there is need of 3 xor circuits and for 
complete xor operation it takes 4 transistors, so total number of 
transistors to design this circuit is 12. 


# Tool Used
- Synopsys Custom Compiler: The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart
of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

- Synopsys Primewave: PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

- Synopsys 28nm PDK: The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Full Adder Ckt using GDI technique
![Inverter](https://user-images.githubusercontent.com/100522966/155893158-d4e660bd-86b3-4030-a142-3747dd995419.JPG)

# Buffer Ckt
![Xor](https://user-images.githubusercontent.com/100522966/155893190-c46562ef-97d0-49e3-8f29-ba2f571bc662.JPG)



# Parity Generator Testbench Design
![Parity_gene_tb](https://user-images.githubusercontent.com/100522966/156007922-3579f5fd-f365-487b-8016-445c631a3551.JPG)

# Simulated Waveform
![Parity_gene_wave](https://user-images.githubusercontent.com/100522966/156008074-c6031885-7147-4c40-846a-244d4950f7dd.JPG)

# Schematic Netlist
The netlist is present here : [Netlist](https://github.com/AniJoshi12/Party-Generator/edit/main/Netlist)

# Acknowledgements
- [Kunal Ghosh , Co-Founder , VSD Corp. Pvt. Lim.](https://github.com/kunalg123)
- [Synopsys India](https://www.synopsys.com/)
- [Indian Institute Of Technology , Hyderabad ](https://iith.ac.in/)
- Chinmay Panda , IIT Hyderabad
- Sameer Durgoji , NIT Karnataka

# References
[1] K. Mangla and S. Saxena, "Analysis of Different CMOS Full Adder Circuits," International Journal of Engineering and Technical Research (IJETR), vol. 3, no. 5, pp. 241-245, May 2015.
[2] Zarin Tabassum, Meem Shahrin, Aniqa Ibnat, Tawfiq Amin, “Comparative Analysis and Simulation of Different CMOS Full Adders Using Cadence in 90 nm Technology” 2018 3rd International Conference for Convergence in Technology (I2CT)

[3] https://www.electronicshub.org/parity-generator-and-parity-check/

[4] https://old.amu.ac.in/emp/studym/100006525.pdf

# Author
Akshay Rahangdale , MTech VLSI Design , Vellore Institute Of Technology , Vellore

