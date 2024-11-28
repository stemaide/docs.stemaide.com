# Project 1: TRAFFIC LIGHT

| **Description** | This is an interesting aspect where you’ll learn to program the traffic light just as the one you see in the communities.   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Use case**    | You can create a traffic light to help prevent accidents, regulate traffic flow and also enhance safety in our environment. |

## Components (Things You will need)

| ![Traffic light module ](../../assets/components/trafficmodule.png) | ![Arduino Uno](../../assets/components/arduino.png) | ![Arduino USB Cable](../../assets/components/USB_Cable.png) | ![Breadboard](../../assets/components/breadboard.png) | ![Jumper Wires](../../assets/components/jump_wire.png) |
| ------------------------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------ |

## Building the circuit

Things Needed:

- Arduino Uno = 1
- Arduino USB cable = 1
- Traffic light module = 1
- green jumper wires = 1
- red jumper wires = 1
- yellow jumper wires = 1
- White jumper wire= 1

## Mounting the component on the breadboard

**Step 1:** Take the Traffic light and the breadboard, insert the Traffic light into the horizontal connectors on the breadboard.

![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/Trafic%20Light%20image%201.png).

## WIRING THE CIRCUIT

### Things Needed:

- Green jumper wires = 1
- Red jumper wires = 1
- Yellow jumper wires = 1
- White jumper wire= 1

**step 1:** Take the red jumper wire. This wire will connect the Arduino UNO and the red light (red pin) of the traffic light. This pin is labeled “R” on the traffic light.

**step 2:** Connect one end of the red jumper wire to the red pin’s hole and the other end to the Arduino UNO. Ensure you place the pin in the right hole.

**step 3:** Connect the other end of the red pin to hole number 5 on the Arduino UNO.

![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/Traffic%20Ligth%20image%202.png).

**step 4:** Connect one end of the yellow jumper wire to Y of traffic light on the breadboard. Ensure you put the pin in the right hole on the breadboard and connect the other end of the yellow jumper wire to pin number 6 on the Arduino UNO.  
![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%201.png).

**step 5:** Connect one end of the green jumper wire to G of traffic light on the breadboard. Ensure you put the pin in the right hole on the breadboard and connect the other end of the green jumper wire to pin number 7 on the Arduino UNO.  
![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%202.png).

**step 6:** Connect the one end of the white jumper wire to the GND of the Traffic light on the breadboard and the other end to GND on the Arduino UNO board.
![Trafic Light fixed on breadboard](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%203.png).

## PROGRAMMING

**Step 1:** Open your Arduino IDE. See how to set up here: [Getting Started](../../../../README.md#getting-started).

**Step 2:** Type the following codes before the void setup function.

```
const int red = 5;
const int yellow = 6;
const int green = 7;
```

![Pinmode decalration](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%204.png).

**Step 3:** Type the following codes in the void setup function as shown below;

```
 pinMode (red, OUTPUT);
pinMode (yellow, OUTPUT);
pinMode (green, OUTPUT);
```

![Trafic pinMode](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%205.png).

**Step 4:** Type the following codes in the void loop function as shown below;

```
 digitalWrite (green, HIGH);
delay (3000);
digitalWrite (green, LOW);
delay (3000);
```

![Truning On the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%206.png).

**Step 5:** Now let make the yellow blink by typing the following codes;

```
  digitalWrite (yellow, HIGH);
delay (1000);
digitalWrite (yellow, LOW);
delay (1000);
```

![Truning On the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/trafic%207.png).

**Step 6:** Now let make the Red also blink by typing the following codes;

```
 digitalWrite (red, HIGH);
delay (2000);
digitalWrite (red, LOW);
delay (2000);
```

![Truning On the Trafic ligth ](../../assets/1.0/Traffic%20Light%20Module/Traffic%20Light%20Red%20On/tarfic%208.png).

## Uploading the code

**Step 1:** Save your code. _See the [Getting Started](../../../../README.md#getting-started) section_

**Step 2:** Select the arduino board and port _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_.

**Step 3:** Upload your code. _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_

## CONCLUSION

In conclusion, the STEMAIDE traffic light project exemplifies the practical application of electronics and programming to enhance road safety and traffic efficiency. By simulating the familiar traffic signal system, this project provides valuable insights into coding logic, component integration, and real-world control systems. Through a basic yet impact project, learners gain hands-on experience in designing, coding, and implementing a fundamental automation solution with potential applications in various urban contexts.
