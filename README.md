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

| **Parameter**              | **Description**                                               | **Min**  | **Type** | **Max**  | **Unit** | **Condition**                                                        |
|----------------------------|---------------------------------------------------------------|---------|----------|---------|----------|----------------------------------------------------------------------|
| **Technology**              | 130 nm CMOS Process                                           |         |          |         |          |                                                                      |
| **RL**                      | Load resistance at output terminal                            | 100     |          |         | MΩ       | VDD = 3.3V, T = 27°C                                                 |
| **CL**                      | Load capacitance at output terminal                           |         |          | 50      | pF       | VDD = 2.7V - 3.6V, T = -40°C - 125°C, RL = 100MΩ                       |
| **Vdd**                     | Supply voltage                                                | 3.2     | 3.3      | 3.6     | V        | T = -40°C to 125°C                                                    |
| **Vout**                    | Output reference voltage (V)                                  | 1.0     | 1.2      | 1.4     | V        | VDD = 3.3V, T = 27°C                                                  |
| **Tc_vout**                 | Temperature coefficient of output voltage                     |         | 20       |         | ppm/°C   | T = -40°C to 125°C, VDD = 3.3V                                        |
| **Vc_vout**                 | Voltage coefficient of output voltage                         |         | 5        |         | %/V      | VDD = 2.7V to 3.6V, T = 27°C                                          |
| **Tstart**                  | Start-up time                                                 |         | 3.0      |         | μs       | VDD = 3.3V, T = 27°C, RL = 100MΩ, CL = 50pF                            |
| **IDD (EN=1)**              | Supply current when enabled                                   | 20      |          | 30      | μA       | VDD = 3.3V, T = 27°C                                                  |
| **IDD (EN=0)**              | Supply current when disabled                                  | 0.1     |          | 1       | μA       | VDD = 3.3V, T = 27°C                                                  |



