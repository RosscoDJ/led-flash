# led-flash
Hardware LED flasher for microcontrollers.

This project is a hardware add-on for microcontrollers that provides a flashing LED. It saves clock cycles and frees up resources such as timers to be used for more important tasks. All is controlled using only one output pin on the microcontroller.

The project utilises a single supply opamp set up as an oscillator to drive the LED, with Vin connected to an output pin of the MCU. Therefore, when the pin is set ```HIGH```, the led will flash.

C2 should be placed as close to the LM358 power pin (pin 8) as possible. 
R4 can be varied in value for a different flashing rate.
U1B can be set up as a duplicate of the circuit for a second flasher circuit from a different MCU pin.

Upcoming changes:
- Provide LED-on or LED-off when not flashing
