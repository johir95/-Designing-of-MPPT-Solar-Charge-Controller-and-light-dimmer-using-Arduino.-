# Designing-of-MPPT-Solar-Charge-Controller-and-light-dimmer-using-Arduino.-

&nbsp;
&nbsp;

<h2>About:</h2>
The primary objective of this project is to design a sophisticated solar charge controller with Maximum Power Point Tracking (MPPT) capabilities light dimmer that can efficiently manage the charging of batteries from solar panels. In addition, the project aims to integrate a light-dimming functionality that adjusts the intensity of a connected lighting system based on ambient light conditions. The solution will enable remote monitoring, control, and optimization of both solar charging and lighting intensity through the Arduino platform.
This project outlines the creation of an Arduino-based solar charge controller featuring Maximum Power Point Tracking (MPPT) capabilities and an integrated light dimmer. The system optimizes solar panel output through continuous MPPT adjustments while dynamically adapting lighting intensity based on ambient light levels. This innovative solution aims to enhance solar energy utilization and lighting efficiency while offering convenience and adaptability. 


&nbsp;
&nbsp;

<h2>Circuit Components:</h2>

-  Arduino Nano 
-  Inductor 
-  Capacitor 
-  Resistor 
-  Current Sensor ACS712 
-  Voltage Sensor 
-  Transistor IRFZ44N 
-  Diode IN5809, MBR2045CT 
-  Push Button Switch 
-  Solar Panel 
-  16×2 LCD Display 
-  Boost Converter MC34063 
-  Opto-Coupler 
-  Trim pots 
-  MOSFET IRF3710 
-  Pin terminal block 
-  Jumper Wires 

&nbsp;
&nbsp;

<h2>Circuit Diagram:</h2>

<img align="centre" alt="Chip Design" width="500" height="300" src="https://github.com/johir95/-Designing-of-MPPT-Solar-Charge-Controller-and-light-dimmer-using-Arduino.-/blob/main/Circuit%20diagram.PNG">

&nbsp;
&nbsp;


<h2>Components Description:</h2>

-  **MPPT:** The Maximum Power Point Tracker (MPPT) circuit is based around a synchronous buck converter circuit. It steps the higher solar panel voltage down to the charging voltage of the battery.  
-  **Voltage Sensor:** It is used to measure electrical voltage in a circuit.  
-  **Current Sensor:** It is used to measure electrical current in a circuit.  
-  **Buck Converter:** A type of DC-DC that is capable of stepping down a higher input voltage to a lower output voltage.  
-  **Opto-Coupler:** It provides electrical isolation between two parts of an electronic circuit while allowing the transfer of signals or control information through an optical interface.  
-  **Arduino:** It is the processing unit of the circuit.  
-  **LCD Display:** Used for the display of information.  

&nbsp;
&nbsp;


<h2>Basic Circuit Operation:</h2>

For a Solar panel and battery, we need to design a Buck Converter. The Buck converter in our case is designed using the Inductor, Capacitor, and MOSFETS. The Solar Panel voltage is fed as an input voltage. The buck converter is made up of the synchronous MOSFET. There are two voltage divider circuits (R1, R2, and R7, R8) to measure the solar panel and battery voltages respectively. The output from the dividers feeds the voltage signal to Analog Pin A0 & A2 of Arduino. The diodes D1 & D5 are TVS diodes used for overvoltage protection from the solar panel and load side. The MOSFET Q2 is used to control the load. The current sensor ACS712 senses the current from the solar panel and feeds it to the Arduino analog pin A1. The 3 LEDs are connected to the digital pins of the microcontroller and serve as an output interface to display the charging state.


&nbsp;
&nbsp;



<h2>Output:</h2>

<h3>OFF Condition:</h3>

<img align="centre" alt="Chip Design" width="400" src="https://github.com/johir95/-Designing-of-MPPT-Solar-Charge-Controller-and-light-dimmer-using-Arduino.-/blob/main/Output%201.jpg">

&nbsp;
<h3>ON Condition:</h3>
<img align="centre" alt="Chip Design" width="400" src="https://github.com/johir95/-Designing-of-MPPT-Solar-Charge-Controller-and-light-dimmer-using-Arduino.-/blob/main/Output%202.jpg">
