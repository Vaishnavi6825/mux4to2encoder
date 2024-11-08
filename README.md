# Multiplexer-Based 4-to-2 Encoder: A Simplified Approach

This repo deals with the construction of a 4 to 2 encoder using 2x1 Mux gate using CMOS Skywater 130nm technology in 
<a href="https://xschem.sourceforge.io/stefan/index.html" target="_blank">xschem</a> & obtaining its parameters through pre-layout simulation using 
<a href="https://ngspice.sourceforge.io/" target="_blank">ngspice</a>.

## Abstract 

This repo deals with the design and implementation of a  4 to 2 encoder using 2x1 Mux using Skywater 130nm CMOS technology.This repository presents an innovative 4-to-2 encoder architecture using 2:1 multiplexers as the core component. Designed to streamline encoding operations while minimizing circuit complexity, this MUX-based approach optimizes resource utilization effectively in both compact and large-scale implementations. By combining functional logic components with a simplified multiplexer configuration, this encoder achieves optimized performance, making it particularly suited for compact, resource-constrained environments.

![image](https://github.com/user-attachments/assets/294f120e-670f-405b-b3d7-ce6278970d96)



<br> <br> <br> 


## Block Diagram

![image](https://github.com/user-attachments/assets/c2e0f993-3948-44a6-95a1-88199ff95e31)

<br> <br> 

## Circuit Diagram 



<br> <br>


### Transient Analysis Results for 4-to-2 Encoder Design

| **Parameter**   | **Description**                                                                                   | **Value**    | **Unit** | **Comments**                                         |
|-----------------|---------------------------------------------------------------------------------------------------|--------------|-----------|------------------------------------------------------|
| `tpHL`          | **Propagation Delay (High to Low)**: Time taken for output to switch from high (5V) to low (0V)   | -61.65       | ps        | Average value across simulations                     |
| `tpLH`          | **Propagation Delay (Low to High)**: Time taken for output to switch from low (0V) to high (5V)   | 224.37       | ps        | Average value across simulations                     |
| `tr`            | **Rise Time**: Time for output to rise from 10% (0.5V) to 90% (4.5V) of final high value          | 305.95       | ps        | Represents how quickly output reaches high level     |
| `tf`            | **Fall Time**: Time for output to drop from 90% (4.5V) to 10% (0.5V) of high level                | 235.97       | ps        | Represents how quickly output reaches low level      |
| `Voh`           | **Output High Voltage**: Maximum voltage at high level                                            | 5.000        | V         | Stable at 5V (VCC)                                   |
| `Vol`           | **Output Low Voltage**: Minimum voltage at low level                                              | 0.000        | V         | Stable at 0V                                         |
| `Cin`           | **Input Capacitance**: Capacitance at each input                                                  | -            | -         | Not measured in transient analysis                   |
| `Vth`           | **Threshold Voltage**: Minimum gate voltage required for conduction                               | 0.7          | V         | Based on Skywater 130nm technology                   |
| `VCC`           | **Supply Voltage**                                                                               | 5.000        | V         | Operating voltage range: -40°C to 125°C              |
| `Simulation Time` | Total time simulated for transient analysis                                                     | 100          | ns        | Captured multiple input transitions                  |

> **Note**: The transient analysis was performed using Ngspice on the Skywater 130nm technology node with a supply voltage of 5V. The inputs were pulsed to simulate real-world transitions and measure the dynamic behavior of the MUX-based encoder design.


<br> <br>
<br>

# Schematic Performance Characteristics



## EDA Tools Used & Their Installation  


## Future Works

## Contributers 

## Acknowledgments

## Contact Information

#### Template

- https://github.com/kunalg123/finalSubmissionFormat?tab=readme-ov-file

#### Papers 












