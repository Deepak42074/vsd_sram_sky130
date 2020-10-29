# VSD_SRAM
This project focuses on design of 1024x32(4KB) SRAM memory with operating voltage of 1.8v 
and access time of less than 2.5ns using opensource sky130 pdk technology and compiled using 
opensource compiler openRAM.The circuits(custom cells) which are required as input to openRAM 
are designed and simluated using opensource tools.

## Installing and cloning of repository
### Installing Ngspice
1. Open terminal
2. Type below command to install Ngspice:
##### sudo apt-get install –y ngspice
3. Type below command to install git package:
##### sudo apt install git
### Cloning to repository:
##### git clone https://github.com/Deepak42074/VSD_SRAM.git
* Change directory to Prelayout directory :
##### cd VSD_SRAM/NgspiceNetlist/Prelayout/
* Cloning to Sky130 pdk: 
##### git clone https://foss-eda-tools.googlesource.com/skywater-pdk/libs/sky130_fd_pr
* Simulation of Basic CMOS inverter:
##### cd VSD_SRAM/NgspiceNetlist/Prelayout/
##### ngspice inv.spice


## SRAM Memory Architecture

![](https://github.com/Deepak42074/VSD_SRAM/blob/main/SramMemoryArchitecture/SRAM_memory_architecture.png)


# Prelayout Schematic and Simulaiton waveforms:

## 6T_SRAM cell 
The standard 1-bit 6T - SRAM cell consists of 6 transistors. It has pair of cross-coupled   	                
CMOS inverters and two NMOS access transistors (M5, M6). The NMOS transistors (M3, M4) and 
PMOS transistors(M1,M2) are driver and pull up transistors respectively.

![](https://github.com/Deepak42074/VSD_SRAM/blob/main/CircuitDiagrams/6T_sram_cell.png)

**Simulation Waveform**
** Type below command in Prealyout directory**
** ngspice 6T_sram_cell.spice**

![](https://github.com/Deepak42074/VSD_SRAM/blob/main/SimulationWaveforms/Prelayout/6T_sram_cell.png)









