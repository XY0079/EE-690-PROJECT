# EE-690-PROJECT
Cadence-Based Design and Verification of an 8-Input NAND Gate 


# README

## 8-Input NAND Gate Design and Simulation

This project presents the design and simulation of an **8-input NAND gate** in **Cadence Virtuoso**.
The work includes theoretical delay estimation using the **Elmore delay model**, transistor-level layout design, and transient simulation in **ADE L** to verify the logic function and observe input-to-output propagation delay. 

## Project Overview

In this assignment, an 8-input NAND gate was implemented and analyzed at both the theoretical and simulation levels.
The main goals of the project are:

* to estimate propagation delay using the Elmore delay method,
* to build the transistor-level layout in Virtuoso,
* to verify the correctness of the NAND logic function,
* to compare theoretical delay estimation with Cadence simulation results. 

## Delay Estimation

Based on the handwritten report, the Elmore delay estimation gives:

* **NMOS delay**: approximately **11.5 ps**
* **PMOS delay**: approximately **57.5 ps** 

These theoretical values are then compared with simulation results obtained in Cadence.
The report notes that the simulated delays are approximately:

* **falling delay**: about **35–45 ps**
* **rising delay**: about **30–40 ps** 

The difference between theoretical and simulated values is expected, since Cadence simulation captures more realistic circuit behavior and includes additional environmental and device-related factors. 

## Transistor Sizing

The 8-input NAND gate was designed using the following transistor dimensions:

* **PMOS**: W = **3 µm**, L = **600 nm**
* **NMOS**: W = **12 µm**, L = **600 nm** 

These dimensions were selected to construct the multi-input NAND structure and support functional verification in layout and simulation.

## Layout Design

The project includes a transistor-level layout created in **Cadence Virtuoso**.
The report first shows the layout concept of a **2-input NAND gate with CMOS inverter**, and then extends this idea to the complete **8-input NAND gate** structure. The schematic-style drawing in the report also illustrates the input nodes **A–H**, the power rails (**VDD** and **GND**), and the output node **Y**. 

The layout screenshot demonstrates the physical realization of the transistor network for the NAND gate. This step confirms that the circuit is not only theoretically designed but also physically implemented in a standard VLSI design environment. 

## Simulation

Transient simulation was performed in **Virtuoso ADE L**.
According to the report, the waveform results show that:

* the logic functions are correct,
* the signals corresponding to the tested nets behave as expected,
* there is a consistent and measurable delay between input and output. 

This is consistent with the expected behavior of a multi-stage CMOS logic gate and supports comparison with the Elmore delay estimate. The ADE L detail page also indicates that the transient analysis completed successfully. 

## Conclusion

This project demonstrates the full workflow of digital CMOS gate analysis:

* theoretical propagation delay estimation,
* transistor sizing,
* layout implementation in Cadence Virtuoso,
* transient simulation and functional verification. 

The simulation results confirm that the **8-input NAND gate** operates correctly and exhibits realistic propagation delays.
Although the Elmore delay model provides a useful first-order estimate, Cadence simulation gives more practical results because it reflects non-ideal effects and detailed circuit conditions. 

## Tools Used

* **Cadence Virtuoso**
* **ADE L**
* **Elmore Delay Estimation Method** 

