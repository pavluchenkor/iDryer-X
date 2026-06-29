# Damper Assembly and Testing

## Fitting

Before installing the servo motor into the damper housing, it is important to assemble the damper without the servo and test the smooth movement of the damper flap. The flap should move freely without sticking in any position. If necessary, make minor mechanical adjustments (e.g., remove burrs, fit seating areas, or polish the shaft).

## Mounting on the Shaft

Once smooth movement is confirmed, the flap can be placed onto the servo shaft. Securing it with a self-tapping screw is optional and may be counterproductive in some cases.

## Pre-Assembly Testing

It is recommended to connect the servo to the control board and test its operation on the bench before installing it into the housing. Ensure the flap moves freely when control signals are applied. If any sticking occurs, fix it before proceeding.

Initial flap positioning should be done while the servo is powered. Use the test mode in the menu to adjust the flap's position so that, when closed, it aligns parallel to the long side of the servo body.

<div class="grid cards" markdown>
- ![Setup servo iDreyer](../../img/air-damper/servo001.png)
- ![Setup servo iDreyer](../../img/air-damper/servo002.png)
- ![Setup servo iDreyer](../../img/air-damper/servo003.png)
- ![Setup servo iDreyer](../../img/air-damper/servo004.png)
</div>

## Final Assembly

Install the damper and servo assembly into the base component. Secure it using the retaining ring. There is no need to screw the servo or the ring to the base part, as final assembly will clamp the housing with screws, providing adequate fixation.

Install the temperature and humidity sensor. If using insulation material, cut a rectangle of the appropriate size and insert it as shown in the photo.

<div class="grid cards" markdown>
- ![Setup servo iDreyer](../../img/air-damper/servo005.png)
- ![Setup servo iDreyer](../../img/air-damper/servo006.png)
- ![Setup servo iDreyer](../../img/air-damper/servo007.png)
- ![Setup servo iDreyer](../../img/air-damper/servo008.png)
- ![Setup servo iDreyer](../../img/air-damper/servo009.png)
- ![Setup servo iDreyer](../../img/air-damper/servo010.png)
</div>

## Testing

After assembling the main unit, observe how the system behaves when the motor is powered. If the flap sticks, it may cause a significant voltage drop, potentially rebooting the microcontroller. If unexpected reboots occur during operation, check the flap mechanism for mechanical jamming.

It is strongly advised to test the damper assembly before final housing installation. This may require prior control board assembly and firmware flashing. Alternatively, a separate servo tester can be used. If no control board is available, the damper can be installed into the case and tested later after the electronics are assembled.
