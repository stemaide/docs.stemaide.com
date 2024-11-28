# Project 1: Trafic Light Green Blink Only

| **Description** | This is where you will learn how to make the green LED blink.                                                                                                                                                |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Use case**    | This could be a system that would make the green LED on the traffic light blink to create more awareness or signal that it’s time to move since sometimes, drivers have their attention off when in traffic. |

## Components (Things You will need)

| ![Traffic light module ](../../assets/components/trafficmodule.png) | ![Arduino Uno](../../assets/components/arduino.png) | ![Arduino USB Cable](../../assets/components/USB_Cable.png) | ![Breadboard](../../assets/components/breadboard.png) | ![Jumper Wires](../../assets/components/jump_wire.png) |
| ------------------------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------ |

## Building the circuit

Things Needed:

- Arduino Uno = 1
- Arduino USB cable = 1
- Traffic light module = 1
- green jumper wires = 1
- White jumper wire= 1

## Mounting the component on the breadboard

**Step 1:** Take the Traffic light and the breadboard, insert the Traffic light into the horizontal connectors on the breadboard.

![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/Trafic%20Light%20image%201.png).

## WIRING THE CIRCUIT

### Things Needed:

- green male-male-to-male jumper wires = 1
- White jumper wire = 1

**step 1:** Take the green jumper wire. This wire will connect the Arduino UNO the green light (green pin) of the traffic light. This pin is labeled “G” on the traffic light.

**step 2:** Connect one end of the green jumper wire to R pin of traffic light on the breadboard. Ensure you put the pin in the right hole.

**step 3:** Connect the other end of the green jumper wire to pin number 5 on the Arduino UNO.

![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green1.png).

**step 4:** Take the white jumper wire and connect one end to the GND pin of the traffic light.

**step 5:** Connect the other end of the white jumper wire to GND on the Arduino UNO.

![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green2.png).

## PROGRAMMING

**Step 1:** Open your Arduino IDE. See how to set up here: [Getting Started](../../../../README.md#getting-started).

**Step 2:** Type `   const int green = 7;` before the void setup function.

![Pinmode decalration](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%201.png).

**Step 3:** Type the following codes in the void setup function as shown below;

```
pinMode (green, OUTPUT);
```

![Trafic pinMode](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%202.png).

**Step 4:** Type the following codes in the void loop function as shown below;

```
digitalWrite (green, HIGH);
```

![Truning On the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%203.png).

The digitalWrite () function controls the state of the pin. The pin can either be HIGH or LOW. The HIGH state turns on the LED. As a result, the code below turns on the LED.

**Step 5:** Now, let's introduce a delay by typing `delay(400);` exactly as shown in the image below.
![Truning OFF the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%205.png).

**Step 6:** : Type `digitalWrite (green, LOW);` exactly as shown in the image below.
![Truning OFF the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%206.png).

**Step 7:** Now, let's finish up with a delay by typing `delay(400);` exactly as shown in the image below.
![Truning OFF the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/green%20code%207.png).

## Uploading the code

**Step 1:** Save your code. _See the [Getting Started](../../../../README.md#getting-started) section_

**Step 2:** Select the arduino board and port _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_.

**Step 3:** Upload your code. _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_

## OBSERVATION

When the circuit is functioning, observe the green LED of the tgrafic ligth blinking as expected. This indicates that the LED is receiving the signal correctly from the Arduino and is operating as intended.

## CONCLUSION

In brief, the project centered on creating a blinking green light within a simulated traffic light system provides an instructive introduction to controlled visual signaling. By programming the green LED to blink, participants gain insights into timing control, code logic, and the role of dynamic visual cues. This endeavor serves as a cornerstone in electronics exploration, showcasing the concept of rhythmic signaling and fostering curiosity about practical applications, such as traffic flow management and automation.
