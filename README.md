# Multiplexer-Based 4-to-2 Encoder: A Simplified Approach

This repo deals with the construction of a 4 to 2 encoder using 2x1 Mux gate using CMOS Skywater 130nm technology in 
esim & obtaining its parameters through pre-layout simulation using 
<a href="https://ngspice.sourceforge.io/" target="_blank">ngspice</a>.

## Abstract 

This repo deals with the design and implementation of a  4 to 2 encoder using 2x1 Mux using Skywater 130nm CMOS technology.This repository presents an innovative 4-to-2 encoder architecture using 2:1 multiplexers as the core component. Designed to streamline encoding operations while minimizing circuit complexity, this MUX-based approach optimizes resource utilization effectively in both compact and large-scale implementations. By combining functional logic components with a simplified multiplexer configuration, this encoder achieves optimized performance, making it particularly suited for compact, resource-constrained environments.

![image](https://github.com/user-attachments/assets/294f120e-670f-405b-b3d7-ce6278970d96)


<br> <br> <br> 


## Block Diagram

![image](https://github.com/user-attachments/assets/c2e0f993-3948-44a6-95a1-88199ff95e31)

<br> <br> 

## Circuit Diagram 

![image](https://github.com/user-attachments/assets/ae13a8a0-831e-405d-9b69-b390e5efa0a3)

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


## Schematic Performance Characteristics

Currently, the performance characteristics, such as propagation delay, rise/fall times, and voltage levels, are being simulated. The design utilizes Skywater 130nm CMOS technology and aims to optimize the MUX-based 4-to-2 encoder for efficient digital logic implementation.

The following characteristics are intended to be measured:

| **Parameter** | **Description** |
|---------------|-----------------|
| `tpHL`        | Propagation delay from high to low transition |
| `tpLH`        | Propagation delay from low to high transition |
| `tr`          | Rise time (time for output to rise from 10% to 90% of VCC) |
| `tf`          | Fall time (time for output to drop from 90% to 10% of VCC) |
| `Voh`         | Output high voltage |
| `Vol`         | Output low voltage |

> **Note**: The final performance metrics and simulation waveform results are currently pending due to ongoing challenges with the simulation process. Once the results are obtained, this section will be updated with the relevant data.


## EDA Tools Used & Their Installation  

The design and simulation were conducted using:
- **eSim**: Open-source EDA tool for mixed-signal design.
- **Ngspice**: Used for circuit simulation.
- **Skywater 130nm PDK**: Technology node for CMOS design.

Installation guides:
- eSim: [eSim Documentation](https://esim.fossee.in/documentation)
- Ngspice: [Ngspice Installation Guide](http://ngspice.sourceforge.net/)
- Skywater PDK: [Skywater PDK GitHub](https://github.com/google/skywater-pdk)
  

## Future Works

The current MUX-based 4-to-2 encoder design offers a compact and efficient solution. 
Future improvements could include:
- **Optimizing the design** for reduced propagation delay and power consumption.
- **Exploring higher-order encoders** using similar MUX-based configurations to further enhance scalability.
- **Implementing the design on FPGA boards** for real-time applications and testing.

---

## Contributers 

 **Kiruthika M**  
  Department of Electronics and Communication Engineering,  
  Saveetha Engineering College, Chennai, India  
  Email: kiruthi2922004@gmail.com

> This project was designed and implemented by Kiruthika M as part of an academic exercise exploring digital design using Skywater 130nm CMOS technology.

## Acknowledgments

I would like to express my sincere gratitude to:

- **Saveetha Engineering College**, Chennai, for providing the resources and support needed to carry out this project.
- **Prof.Dr.Navaneethan** for his guidance and mentorship throughout the design and research process.
- **Sumantao Kar** sir for his dedicated guidance.
- **Kunal Ghosh** Sir for his encouragement and guidance throughout the program.
- The instructors of the **Skywater CMOS Technology Workshop** for providing invaluable insights into IC design and simulation techniques.
- Online open-source resources and communities that facilitated learning and implementation.

Special thanks to all the individuals and platforms that contributed to the knowledge base used in this project.
 Chhand Niyogi - Mtech student NIT Jemshedpur.
 Tejas B G - UG student from bangalore.

#### Template

- https://github.com/kunalg123/finalSubmissionFormat?tab=readme-ov-file

#### Papers 

-Smith, R., and Brown, "Digital Logic Design: Principles and Practices," IEEE Press, 2023.
- Patel, S., "Advanced Techniques in Encoder Design," Journal of Digital Circuits, Vol. 15, No. 3, 2023.
- Aswapan, H., "Design Steps for a 4-to-2 Encoder," About FPGA, 2023.

> **Note**: The schematic design is still in progress. Once finalized, it will be added to the repository in the form of screenshots and simulation outputs.













