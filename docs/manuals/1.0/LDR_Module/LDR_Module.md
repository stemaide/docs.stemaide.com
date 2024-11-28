# Project 1: LIGHT INTENSITY CHECKER

| **Description** | This is a basic project that helps one to check the light intensity present at a particular environment. |
|------------------|----------------------------------------------------------------|
| **Use case**     |  Wanting to get a device that will measure or detect the brightness of an L.E.D or anything that bright such as day light and even night, you can use this approach to do that. |

## Components (Things You will need)

| ![LDR Module](../../assets/components/ldr.png) | ![Arduino Uno](../../assets/components/arduino.png) | ![Arduino USB Cable](../../assets/components/USB_Cable.png) | ![Breadboard](../../assets/components/breadboard.png) |![Breadboard](../../assets/components/jump_wire.png)|
|-------------------------|-------------------------|-------------------------|-------------------------|-------------------------|

## Building the circuit

Things Needed:
-	Arduino Uno = 1
-	Arduino USB cable = 1
-	Light dependent resistor   = 1
-	Red jumper wire = 1
-	Black jumper wire = 1
-	Green jumper wire = 1
-	White jumper wire = 1


## Mounting the component on the breadboard

**Step 1:** Take the light dependent resistor and the breadboard, insert the light dependent resistor into the horizontal connectors on the   breadboard

![LDR fixed on breadboard](../../assets/1.0/LDR_Module/Picture1.png).


## WIRING THE CIRCUIT

### Things Needed:

- Red male-male-to-male jumper wires = 1
- Blue male-to-male jumper wires = 1


**Step 2:** Take the red jumper wire. Connect one end of the wire to the “VCC” port on the resistor and the other end to the “5V” port on the Arduino UNO.

![LDR fixed on breadboard](../../assets/1.0/LDR_Module/Picture2.png)

**Step 3:** Take the black jumper wire. Connect one end of the wire to the “GND” hole on the Arduino UNO and the other end to the “GND” port on the resistor.

![LED fixed on breadboard](../../assets/1.0/LDR_Module/Picture3.png).

**Step 4:** Take the white jumper wire. Connect one end of the wire to the “DO” hole on the resistor and the other end to hole number 2 on the Arduino UNO.

![LED fixed on breadboard](../../assets/1.0/LDR_Module/Picture4.png).

**Step 5:** Take the green jumper wire. Connect one end of the wire to the “AO” port  on the Arduino UNO to the “AO” port on the resistor.

![LED fixed on breadboard](../../assets/1.0/LDR_Module/Picture5.png).

_make sure you connect the arduino usb use blue cable to the Arduino board_.

## PROGRAMMING

**Step 1:** Open your Arduino IDE. See how to set up here: [Getting Started](../../../../README.md#getting-started).

**Step 2:** Type ``` const int LDR_PIN = A0; ``` as shown below in the image.

_**NB:** Make sure you avoid errors when typing. Do not omit any character or symbol especially the bracket { }  and semicolons ;  and place them as you see in the image . The code that comes after the two ash backslashes “//” are called comments. They are not part of the code that will be run, they only explain the lines of code. You can avoid typing them._
![LDR_PIN decalration](../../assets/1.0/LDR_Module/code1.png).

**Step 3:** Type ``` const int DO_PIN = 2;``` as shown below in the image.

![DO_PIN decalration](../../assets/1.0/LDR_Module/code2.png).
_**NB:** The code below sets the pin names as an output pin. An output pin helps send signals from the microcontroller to other components in the circuit. The pinMode () function, helps determine and control the behavior of a specific pin on the board._

**Step 4:** Type ``` pinMode (DO_PIN, INPUT); ``` as shown below in the image.

![PinMode decalration](../../assets/1.0/LDR_Module/code3.png).

**Step 5:** Type ``` Serial.begin(9600); ;``` as shown below in the image.

![Serial decalration](../../assets/1.0/LDR_Module/code4.png).

**Step 6:** Type ``` int 1drValue = analogRead (LDR_PIN); ``` as shown below in the image.

![Analog decalration](../../assets/1.0/LDR_Module/code5.png).

**Step 7:** Type ``` int digitalValue = digitalRead (DO_PIN); ``` as shown below in the image.

![DigitalRead decalration](../../assets/1.0/LDR_Module/code6.png).

**Step 8:** Type ``` Serial.print(“Analog Value:”); ``` as shown below in the image.

![Serial.print decalration](../../assets/1.0/LDR_Module/code7.png).

**Step 9:** Type ``` Serial.printIn(ldrValue); ``` as shown below in the image.

![Serial.println decalration](../../assets/1.0/LDR_Module/code8.png).

**Step 10:** Type ``` Serial.print(“Digital Value:”); ``` as shown below in the image.

![Serial.print decalration](../../assets/1.0/LDR_Module/code9.png).

**Step 11:** Type ``` Serial.printIn(digitalValue); ``` as shown below in the image.

![Serial.println decalration](../../assets/1.0/LDR_Module/code10.png).


**Step 12:** Save your code. _See the [Getting Started](../../../../README.md#getting-started) section_

**Step 13:** Select the arduino board and port _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_.

**Step 14:** Upload your code.

## CONCLUSION
In summary, this LED project presents a basic yet significant step in understanding parallel LED control. By simultaneously lighting up two LEDs, learners gain insight into simple circuit connections and programming synchronization. This project serves as a starting point for more complex configurations while highlighting the fundamental principle of coordinated electronic actions, setting the stage for broader exploration in electronics and automation.



