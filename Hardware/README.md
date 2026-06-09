
## Hardware Part 🔧⚡

The hardware side of the DC Energy Meter is responsible for measuring the real DC voltage and current from the circuit.

The system uses an Arduino Nano as the main controller.  
The voltage is measured using a voltage divider circuit, while the current is measured using the INA219 current sensor.  
Then, the Arduino processes these readings to calculate power and energy consumption.

In simple words:  
the circuit measures, the Arduino calculates, and the display/output shows the result. 🔥

## Hardware Design Photos 📸

### Schematic Design

<img src="Screenshot%202026-06-09%20063438.png" alt="DC Energy Meter Hardware Setup" width="700">
### PCB ROUTING 
<img src="Screenshot%202026-06-09%20063449.png" alt="DC Energy Meter PCB Layout" width="700">

### Hardware Setup

<img src="Screenshot%202026-06-09%20063718.png" alt="DC Energy Meter Schematic Design" width="700">
## Hardware Components Used

- Arduino Nano  
  Used as the main controller to read sensor values and calculate voltage, current, power, and energy.

- INA219 Current Sensor  
  Used to measure DC current through the load using I2C communication with the Arduino.

- Voltage Divider Circuit  
  Used to reduce the input DC voltage to a safe level suitable for the Arduino analog pin.

- Resistors  
  Used in the voltage divider circuit and signal conditioning.

- Capacitor  
  Used for filtering and stabilizing the measured voltage signal.

- Zener Diode  
  Used as protection for the Arduino analog input.

- Battery / DC Source  
  Used as the input power source for testing the meter.

- Terminal Connectors  
  Used to connect the voltage input, current path, source, and external wiring.

- Power Pins / VCC and GND Connections  
  Used to supply power to the circuit modules.

## Hardware Role

- Measures DC voltage
- Measures DC current
- Sends current data through INA219 using I2C
- Reads voltage using the Arduino analog input
- Protects the Arduino input from high voltage
- Helps calculate power in watts
- Helps calculate consumed energy over time
- Supports real-time monitoring of DC loads
