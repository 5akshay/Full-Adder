# Full-Adder Using gate diffusion Input
# Design 10T Full Adder using Modified Gate Diffusion Input Technique.
This repository presents the Design of Full Adder ckt using 28nm CMOS Technology and tool used is Synopsis Custom Compiler.
# Table Of Content
- [Abstract](https://github.com/5akshay/Full-Adder/blob/main/README.md#Abstract)
- [Circuit Details](https://github.com/5akshay/Full-Adder/blob/main/README.md#Working)
- [Tool Used](https://github.com/5akshay/Full-Adder/blob/main/README.md#Tool-Used)
- [Full Adder Ckt using GDI technique](https://github.com/5akshay/Full-Adder/blob/main/README.md#CMOS-Inverter-Gate)
- [Buffer Ckt](https://github.com/5akshay/Full-Adder/blob/main/README.md#CMOS-XOR-Gate)
- [Simulated Waveform](https://github.com/5akshay/Full-Adder/blob/main/README.md#Simulated-Waveform)
- [Schematic Netlist](https://github.com/5akshay/Full-Adder/blob/main/README.md#Schematic-Netlist)
- [References](https://github.com/5akshay/Full-Adder/blob/main/README.md#References)
- [Acknowledgements](https://github.com/5akshay/Full-Adder/blob/main/README.md#Acknowledgements)

# Abstract
Full adder circuit may be a important element within the style of application of integrated circuits in VLSI. the look and analysis of Full Adder cell exploitation the modified Gate Diffusion Input (MGDI) technique on optimizing the facility, delay and Power Delay Product (PDP). this system (MGDI) permits reducing power, delay and space of digital circuits, whereas maintaining low complexness of logic style. Through investigation is disbursed for the effectiveness exploitation combination of various low power full adder circuit style techniques. the most objective of those full adders is providing high-speed and low power consumption conjointly provides sensible voltage swing.

# Circuit Details
One of the significant differences between GDI & CMOS based structure is that, instead of connecting VDD & Ground to the source of PMOS & NMOS respectively, input signals are given in GDI cell. The basic GDI cell was suggested by Morgenshtein. It has three input terminals: G (gate input by PMOS & NMOS shorted), P (source input of PMOS), and N (source input of NMOS). GDI based full adder architecture depicted in Fig can be divided into two parts. In the first stage, XOR & XNOR function are generated. The XOR gate (M1, M2, M3, M4), uses less number of transistors as compared to conventional design of XOR gate using CMOS logic, which results in improving the overall performance. In Fig M1, M3, M5, M7, M10 are PMOS transistors and M2, M4, M6, M8, M9 are NMOS transistors. Both the bulks of PMOS & NMOS are connected to source.
- Truth Table
![full-adder2](https://user-images.githubusercontent.com/100597348/156207340-b12ec67a-5bf5-42ea-a889-c8459f067a64.png)

- The truth table can be verified with the help of following calculations
- Sum = x' y' z+x' yz+xy' z'+xyz.
- Carry = xy+xz+yz

# Tool Used
- Synopsys Custom Compiler: The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart
of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

- Synopsys Primewave: PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

- Synopsys 28nm PDK: The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Full Adder Ckt using GDI technique
<img width="666" alt="fulladder" src="https://user-images.githubusercontent.com/100597348/156211958-04fee82b-2232-4fd2-a1a7-e7840e2c35b1.png">


# Buffer Ckt
<img width="464" alt="buffer" src="https://user-images.githubusercontent.com/100597348/156212008-3aa7d35d-2545-4edf-9c11-48c7da34305b.png">

# Simulated Waveform
<img width="957" alt="waveform" src="https://user-images.githubusercontent.com/100597348/156212071-31521bd3-f9cc-4132-a1c9-ffc1f1cb8c69.png">


# Schematic Netlist
- The netlist is present here : [Netlist](https://github.com/5akshay/Full-Adder/blob/main/netlist.txt)


# Acknowledgements
- [Kunal Ghosh , Co-Founder , VSD Corp. Pvt. Lim.](https://github.com/kunalg123)
- [Synopsys India](https://www.synopsys.com/)
- [Indian Institute Of Technology , Hyderabad ](https://iith.ac.in/)
- Chinmay Panda , IIT Hyderabad
- Sameer Durgoji , NIT Karnataka

# References
- [1] K. Mangla and S. Saxena, "Analysis of Different CMOS Full Adder Circuits," International Journal of Engineering and Technical Research (IJETR), vol. 3, no. 5, pp. 241-245, May 2015.
- [2] Zarin Tabassum, Meem Shahrin, Aniqa Ibnat, Tawfiq Amin, “Comparative Analysis and Simulation of Different CMOS Full Adders Using Cadence in 90 nm Technology” 2018 3rd International Conference for Convergence in Technology (I2CT)
- [3] https://www.javatpoint.com/full-adder-in-digital-electronics

# Author
Akshay Rahangdale, MTech VLSI Design, Vellore Institute Of Technology, Vellore

