# Your First Code
In this sheet, we're going to work through the Arduino basics and create a simple LED project.
If you have worked with C, C#, C++ or any other C-similar language, you will have no issues with this!

## Basic Code
### Semi-Colons
Every line of code must end in a semi-colon. This is one of the major differences to languages like python.
If your code isnt working, check your semi-colons.!
### Variables
Every variable you create must have a type assigned. 
Whereas in python you can create a variable with just a name, for example...
``` python
exampleVariable = 6
```
...you need to explicitly state what kind of variable you are creating. The 3 main variable types are:
- String (A piece of text)
``` C
String exampleText = "Hello World";
```
- int (A whole number)
``` C
int exampleNumber = 6;
```
- double (A number with decimal places)
``` C
double exampleNumber = 6.42;
```
- char (A single character)
``` C
char exampleText = 'C';
```

## Pin Mode
On Arduino boards, each pin is labelled with a pin number. These pins can be set to output a voltage (about 3.3v) or read in a voltage. For our work today, we will be using the pins to output voltage instead of reading in voltage.

To set our pins to output voltage, we first need to configure the pin as an Output pin instead of Input pin.
Write the following code in the setup section of your file:
``` C
pinMode([pin number], OUTPUT);

pinMode(2, OUTPUT);
pinMode(3, OUTPUT);
pinMode(4, OUTPUT);
```

Now that our pin is configured, we can start to send out 3.3v. We can control when our board outputs voltage by setting the pin to either LOW or HIGH.
- When the pin is set to low, no voltage is output
- When the pin is set to high, 3.3v is output

``` C
digitalWrite([pin number], HIGH); 
```

``` C
digitalWrite([pin number], LOW); 
```

### Onboard LED
Most Arduinos come with a pre-installed LED built into the board. 

- On Arduino Uno boards, this LED is on Pin 13.
- On ESP32 boards, this LED is on Pin 2.

You can turn this LED on/off by setting the corresponding LED pin to high or low. 

EG:
``` C
pinMode(13, OUTPUT);
digitalWrite(13, HIGH);
delay(1000);
digitalWrite(13, LOW);
```

## Delay
Adding delay to your code is critical if you want to actually see what's happening. Without any delays, the code will run too quick for you to comprehend/debug/understand.

Delay can be added at any point in your code. Simply write the line:
``` C
delay(1000);
```

Delay is measured in milliseconds. 
- A delay of 1000 (delay(1000)) is equal to 1 second
- A delay of 10000 (delay(10000)) is equal to 10 seconds
- A delay of 2500 (delay(2500)) is equal to 2.5 seconds

# Creating a Blinking Arduino
To test your skills so far, we're going to create some code to make the built-in LED blink on and off.

For this, use the pinMode command to set the LED pin to output. Remember,  if you are using an Arduino, the LED pin is pin 13; If you are using an ESP32, the LED pin is pin 2.
Place the pinMode code in the setup() section of your file.

In the loop() section, write the following code:
- Set the LED pin to high using digitalWrite() to turn on the LED
- Delay the code by 1 second
- Set the LED pin to low using digitalWrite() to turn off the LED

Upload the code and see what happens!
