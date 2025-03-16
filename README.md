# Linear Voltage Stabilizer

## Description
This project is a linear voltage stabilizer with a series adjustment element, designed to provide a stable and adjustable output voltage between 7V and 10.5V. It ensures output voltage stability regardless of input voltage variations, temperature changes, or load current fluctuations.

## Technical Specifications
* **Output Voltage:** Adjustable between 7V and 10.5V
* **Input Voltage:** Between 14V and 15.75V
* **Maximum Current:** 0.4A (overload protection included)
* **Output Load:** 1050Ω
* **Thermal Drift:** < 2mV/°C
* **Minimum Gain of the Error Amplifier:** 200
* **Operating Temperature Range:** 0°C - 70°C

## Circuit Structure
The circuit consists of the following functional blocks:
1. **Voltage Reference** – Provided by a Zener diode for stability.
2. **Error Amplifier** – Compares the reference voltage with the output voltage and generates an error signal.
3. **Series Adjustment Element** – A Darlington configuration that adjusts the current through the load.
4. **Negative Feedback Network** – Allows fine adjustment of the output voltage.
5. **Protection Circuit** – Monitors and limits the current to prevent overload.

## PCB Concept and Design in OrCAD

### 1. Component Placement on the Board
* Components are arranged to minimize the length of critical traces and improve circuit stability.
* Power components are separated from control components to avoid excessive thermal dissipation and unwanted interference.

### 2. Transistor Placement and Thermal Efficiency
* Transistors are positioned to allow optimal heat dissipation, preventing overheating.
* The layout minimizes the use of mounting holes, favoring a more compact and manufacturable design.

### 3. Routing and Trace Optimization
* Power traces are short and wide to minimize losses and ensure good conductivity.
* Strict routing rules are applied to avoid large ground loops and optimize circuit functionality.

### 4. Manufacturing Layers
* The PCB is designed with two layers, balancing complexity and production costs.
* The top layer contains the main components and critical traces.
* The bottom layer is used to prevent trace overlap.
* Vias are strategically placed to ensure efficient and robust connections.

### 5. Manufacturing and Testing Considerations
* The design is optimized for easy industrial manufacturing, including guide edges.
* Clear component labeling facilitates both automatic and manual assembly.

## Simulations and Tests
* **Output voltage variation** depending on input voltage
* **Thermal drift testing** to verify circuit stability
* **Overload protection testing**
* **Open-loop gain testing**

## File Structure
* **documentation.pdf** – Detailed project documentation
* **OrCAD/** – Schematics and PCB layout files designed in OrCAD
