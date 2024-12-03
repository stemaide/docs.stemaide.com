# Project 1:Push Button with Buzzer

| **Description** | This project introduces a simple circuit using a push button and a buzzer. The push button acts as a trigger to activate the buzzer, which can be used for applications like a quiz contest bell or notification systems. |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Use case**    | Imagine you want to program a bell for a quiz contest.                                                                                                                                                                    |

## Components (Things You will need)

| ![BUZZER ](../../assets/components/buzzer_ima.webp) | ![Arduino Uno](../../assets/components/arduino.png) | ![Arduino USB Cable](../../assets/components/USB_Cable.png) | ![Breadboard](../../assets/components/breadboard.png) | ![Jumper Wires](../../assets/components/jump_wire.png) | ![Push Button](../../assets/components/Push_Button.png) |
| --------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------- |

## Building the circuit

Things Needed:

- Arduino Uno = 1
- Arduino USB cable = 1
- Buzzer = 1
- Red jumper wires = 2
- White jumper wire= 1
- Green jumper wire= 1

## Mounting the component on the breadboard

**Step 1:** Push Button:Insert two pins into row g and two pins into row d on the breadboard
![inseting push button](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push1.png).

**step 2:** Buzzer: Insert the buzzer into row J on the breadboard. Ensure the longer pin (positive) is correctly aligned.
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push2.png).

**Note:**Take note of where each of the pins are placed on the bread board

## WIRING THE CIRCUIT

### Things Needed:

- Red jumper wires = 2
- White jumper wire= 1
- Green jumper wire= 1

**step 1:** Red Wire: Connect one end to the pin on row d and the other end to Digital Pin 2 on the Arduino Uno.
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push3.png).

**step 2:** White Wire: Connect one end to the other pin on row d and the other end to GND on the Arduino Uno  
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push4.png).

**step 3:** Red Wire: Connect the positive pin of the buzzer to Digital Pin 3 on the Arduino Uno.  
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push5.png)

**step 4:** Green Wire: Connect the negative pin of the buzzer to GND on the Arduino Uno  
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push6.png)

**step 5:** Connect the one end of the white jumper wire to the GND of the Traffic light on the breadboard and the other end to GND on the Arduino UNO board.
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push7.png)

## PROGRAMMING

**Step 1:** Open your Arduino IDE. See how to set up here: [Getting Started](../../../../README.md#getting-started).

**Step 2:** Type the following codes before the void setup function.

```
const int ButtonPin= 2;
```

![Pinmode decalration](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code1.png).

**Step 3:** type`int B = 3;`as shown in the picture below.

![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%202.png).

**Step 4:** Type `int buttonState= 0;` as shown in the picture below.
![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%203.png).

**Step 5:** After the void setup ()within the curly brackets type the following codes.

```
pinMode (ButtonPin, INTPUT_PULLUP);
pinMode (B, OUTPUT);
```

![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%205.png).

**Step 6:** : After the (void loop ()) within the curly brackets type

```
buttonState = digitalRead(ButtonPin);
```

![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%206.png).

**Step 7:** :Now let type

```
 if (buttonState == LOW) {
digitalWrite (B, HIGH);
delay (500);
digitalWrite (B, LOW);
}
```

![inseting the buzzer](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%207.png).

**Step 8:** After all you are expercted to see this code.

![After all code](../../assets/2.0/2.2.Push%20Button%20+%20Buzzer/push%20code%208.png).

## Uploading the code

**Step 1:** Save your code. _See the [Getting Started](../../../../README.md#getting-started) section_

**Step 2:** Select the arduino board and port _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_.

**Step 3:** Upload your code. _See the [Getting Started](../../../../README.md#getting-started) section:Selecting Arduino Board Type and Uploading your code_

## CONCLUSION

If any issues arise during the upload, recheck the wiring and code for errors. Upon successful testing, this project demonstrates how to use a push button to control a buzzer, laying the foundation for interactive systems.
