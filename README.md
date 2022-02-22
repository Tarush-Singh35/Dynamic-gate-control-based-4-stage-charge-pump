# Dynamic-gate-control-based-4-stage-charge-pump
The purpose of this Hackathon is to implement the proposed design in 28 nm PDK (Process Design Kit).
As a result of literature survey and Implemantation, this is a final Report Submission for successful completion of Dynamic-gate-control-based-4-stage-charge-pump and simulation, for [Cloud Based Analog IC Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/).

This repository presents the design of Dynamic-gate-control-based-4-stage-charge-pump implemented using Synopsis Custom Compiler on 28nm CMOS Technology.

# Table of Contents
 * [Introduction](#introduction)
 * [Working](#working)
 * [Designing](#designing)
 * [Tools Used](#Tools-Used)
 * [Pre-Layout Schematics and Simulations](#pre-Layout-Schematics-and-Simulations)
 * [Netlist](#netlist)
 * [Observations](#observations)
 * [Author](#author)
 * [Acknowledgements](#acknowledgements)
 * [References](#references)

# Introduction:

Reducing power consumption in modern VLSI circuits and systems has become significant research due to more demand of low power memory devices. To reduce power consumption, the power supply voltage tends to be scaled down. It also reduces noise margin and speed of operation, which is not favour in digital circuits. The performance of the low power memory device depends on physical mechanisms of oxide tunneling which need constant high voltage irrespective of the MOS technology and scaling. Furthermore, low power devices such as EEPROM and flash memories require higher voltage to perform write and erase operations. Consequently,to design on-chip memory circuits with low power supply voltage is very difficult and critical challenge for nonvolatile memory applications. However, this problem is solved by charge pump (CP) circuits. The CP circuit provides higher on-chip voltage with low power supply voltage. The CP circuit utilize charge transfer switches (CTS) for transferring charges and pumping capacitors as energy storage elements. CP circuits are used in nearly all EEPROM and flash memory devices.The CP circuit is also used in the power managementblocks of liquid-crystal-display (LCD) panels and quiescent touch sensor power supply circuits.

# Tools Used:

<b>• Synopsys Custom Compiler:</b></br>
&emsp;The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

<b>• Synopsys Primewave:</b></br>
&emsp;PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

<b>• Synopsys 28nm PDK:</b></br>
&emsp;The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Netlist:

Refer to the netlist of the circuit here: <a href='Dynamic_CP.cir'>Dynamic Charge Pump Circuit</a>

# Observations:
- The output voltage is 5V .The voltage gain has significantly improved as threshold voltage drop is removed and ON resistance of Charge Transfer Switch is reduced. Further, the substrate bias effect in the Charge Pump circuitis also removed.However operated in Strong inversion region has caused this circuit to have a trade-of between gain and speed hence the circuit can be used for high speed application but it has low noise margin as well as low SNR this can be seen in the transient analysis.

# Author:
• Tarush Singh, B.E(ECE), MCT Rajiv Gandhi Institute of Technology, Andheri, Versova-400053.

# Acknowledgements:
• <a href='https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/'>Cloud Based Analog IC Design Hackathon</a></br>
• <a href='https://www.synopsys.com/'>Synopsys India</a></br>
• <a href='https://www.vlsisystemdesign.com/'>VLSI System Design (VSD) Corp. Pvt. Ltd India</a></br>

# References:
- P. Karuppanan, K. Khan, and S. R. Ghosh, “Dynamic gate and substrate control charge pump circuits,” in Analog Integrated Circuits and Signal Processing, April 2015.
- H. Dadhich, V. Maurya, K. Verma, and S. Jaiswal, “Design and analysis of different type of charge pump using cmos technology,” in 2016 International Conference on Advances in Computing, Communications and Informatics (ICACCI), November 2016.
- M. E. Alaoui, F. Farah, K. E. Khadiri, H. Qjidaa, A. Aarab, and R. E. Alami, “Analysis and design of dickson charge pump for eeprom in 180nm cmos technology,” in 2018 International Conference on Intelligent Systems and Computer Vision (ISCV), My 2018
