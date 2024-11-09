# Energy-Efficient 6T SRAM Cell Design for AI Applications

This project presents an energy-efficient 6T SRAM cell design at the 130nm node, optimized for AI applications through enhanced stability and reduced power dissipation. It supports sustainable computing in AI-driven tasks like GPU caching and edge processing.

## A Glance at the Energy-Efficient 6T SRAM Cell Design

The energy-efficient 6T SRAM cell design presented in this project focuses on achieving stability and low power consumption, essential for reliable operation in AI-driven applications. This design addresses challenges like process variability and power dissipation, making it suitable for integrating systems that demand sustainable performance, like GPU caches, edge AI accelerators, and inference engines. The project explores the principle of generation, implementation, issues, improvements, and future scope of this optimized SRAM design.

For more detailed information, please refer to the full project documentation:  
[Project Paper](./Documentation/VSDHACKATHON_Preethigrace.pdf)

## Block diagram of 6T SRAM CELL

<div align="center">
  <img src="https://github.com/Preethigrace-7/6TSRAM/blob/main/Images/BLOCK%20DIAGRAM.png" alt="Project Screenshot">
</div>

## Circuit diagram of 6T SRAM CELL

<div align="center">
  <img src="https://github.com/Preethigrace-7/6TSRAM/blob/main/Images/Schematic_page-0001.jpg" alt="Circuit Diagram">
</div>

## 6T SRAM Performance Parameters
| Parameter  | Description                                        | Min    | Type    | Max    | Unit   | Condition                                      |
|------------|----------------------------------------------------|--------|---------|--------|--------|------------------------------------------------|
| RL         | Load resistance at Vbgp terminal                  | 100    |         |        | Mohm   | VDD=3.3V, T=27C                                |
| CL         | Load capacitance at Vbgp terminal                 |        |         | 50     | pF     | VDD=2.7V - 3.6V, T=-40C - 125C, RL=100M        |
| Vbgp       | Output Reference voltage                          | 1.2013 | 1.2056  | 1.2070 | V      | T=-40 to 140C, VDD=3.3V                        |
| Vbgp       | Output Reference voltage                          | 1.1698 | 1.2056  | 1.2234 | V      | VDD=2.7V to VDD=3.6V, T=27C                    |
| TC_vbgp    | Temperature Coefficient of Vbgp                   |        | 26.2663 |        | ppm/C  | T=-40 to 125C, VDD=3.3V                        |
| VC_vbgp    | Voltage Coefficient of Vbgp                       |        | 5.9555  |        | %/V    | VDD=2.7V to 3.7, T=27C                         |
| Tstart     | Start up time                                     |        | 3.3     |        | us     | Vdd=3.3V, T=27C, CL=50pF                       |
| VDD        | Supply Voltage                                    | 3.2    | 3.3     | 3.6    | V      | T=-40C to 125C                                 |
| IDD        | Supply Current                                    |        | 22.4760 |        | uA     | EN=1                                          |
| IDD        | Supply Current                                    |        | 95.3950 |        | pA     | EN=0                                          |






