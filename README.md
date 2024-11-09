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

## Tools Used and Steps to Reproduce All Waveforms(Tools allowed are xschem/eSim/ngspice)

This project utilizes **eSim** and **Ngspice** for circuit simulation and waveform analysis. Below are the installation instructions and steps to run simulations on both Ubuntu and Windows OS.

### Tool Installation

#### eSim Installation on Ubuntu

1. **Download eSim Installer**: Download the latest eSim installer from [eSim Downloads](http://esim.fossee.in/downloads) and save it to a local directory.
   
2. **Unpack the Installer**:
   - Open the terminal, navigate to the download directory, and use the following command to unpack the installer:

     ```bash
     unzip eSim-2.4.zip
     ```

3. **Install eSim and Dependencies**:
   - After unpacking, run the following commands in the terminal to install eSim:

     ```bash
     cd eSim-2.4
     chmod +x install-eSim.sh
     ./install-eSim.sh --install
     ```

4. **Launch eSim**:
   - To start eSim, type in the terminal:

     ```bash
     esim
     ```

   - Alternatively, you can double-click the eSim icon created on your Desktop.

#### Ngspice Installation on Ubuntu

1. Open your terminal and enter the following command to install Ngspice:

   ```bash
   sudo apt-get install -y ngspice
   ```

## eSim Installation on Windows

1. **Download eSim Installer**: Download `eSim-2.4 installer.exe` from [eSim Downloads](https://esim.fossee.in/downloads).
2. **Disable Antivirus**: Disable any active antivirus temporarily to avoid interference during installation.
3. **Adjust Path for MinGW or MSYS**:
   - If MinGW or MSYS is already installed, remove them from the `PATH` environment variable to prevent conflicts with eSim.
4. **Run the Installer**:
   - Double-click the `.exe` file to start the installation. Click **Yes** if prompted by a permission window to proceed.
5. **Default Installation Path**:
   - eSim will install by default in the `C` drive under a folder named `FOSSEE`. Ensure the installation path does not contain spaces or reside in "Program Files".
6. **Launch eSim**:
   - An eSim icon will be created on the Desktop upon installation. Double-click the icon to start eSim.
