# Connecting Load Cells

For the proper functioning of the weighing system in the iDryer, it is essential to correctly connect the load cell wires to the HX711 module. Follow the instructions below.

## Wiring Structure

The system uses only four-wire load cells. Typically, the color scheme is as follows:

* **Red**: Excitation + (E+)
* **Black**: Excitation - (E-)
* **Green**: Signal + (A+)
* **White**: Signal - (A-)

## Wiring Diagram to HX711 Module

| Load Cell Wire | HX711 Module Pin |
| :------------- | :--------------- |
| Red (E+)       | E+               |
| Black (E-)     | E-               |
| Green (A+)     | A+               |
| White (A-)     | A-               |

## Wire Verification Method Using a Multimeter

If wire colors are uncertain, use a multimeter to determine the correct connections:

**Set the multimeter to resistance mode (Ohms)**.

**Identify wire pairs with close resistance values**:

* Measure resistance between all possible wire pairs.
* Identify two pairs with resistance around 350-450 Ohms (for most standard load cells).

**Identifying the circuits**:

* One pair will be the excitation wires (Excitation+, Excitation-).
* The other pair will be the signal outputs (Signal+, Signal-).
* Typically, black and red wires are ground and power, respectively.

**How to determine which wire is A+ and which is A-**:

* Set the multimeter to measure DC millivolts (mV DC).
* Apply 5V power to the excitation wire pair (e.g., from the controller board's DC-DC converter).
* Connect multimeter probes to the signal wire pair.
* If the voltage is positive, the wire connected to the red probe is A+; if negative, swap the probes.
  Additionally:
* Press the load cell.
* If voltage increases when pressing, the wire connected to the red probe is A+.
* If voltage decreases (goes negative), swap the probes.

## Connection Procedure

* **Identify the function of each wire** using the method described above.
* **Prepare the wires**: strip 3-5 mm of insulation from the ends.
* **Solder the wires to the HX711 board** according to the wiring table.
* **Observe correct load cell numbering according to board labeling**.
* **Inspect soldering quality**: ensure no shorts between adjacent pins.

## Important Notes

* Only four-wire load cells are used in the device.
* Incorrect wiring can cause improper scale operation or damage to modules.
* After connection, perform weight calibration via the device menu. Enter calibration mode and follow the on-screen instructions.
* When the EEPROM is rewritten, scale calibration must be repeated.
