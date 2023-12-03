## Lesson 2: Creating your first program/project!

The 'Blink' program is typically the first program/project that new users of Arduino create. The Arduino board has a built-in light emitting diode (LED) on pin 13.

In Arduino, a pin is often controlled by assigning it to a variable. Keep this in mind as you create this project.

This section will cover the necessary information for you to create the program by giving you enough information to do it yourself without giving you the answer outward, but if you get stuck there will be a list of instructions at the end of the section. However, feel free to ask for help or practice your research skills if you run into any problems.

### Built-in functions required for this program/project

Below are 3 functions required for the 'Blink' program.

Notice that if the function has more than one word there isn't a space separating the two but instead the second word (and if the function had a subsequent third, fourth, etc. word) is capitalized. This is known as camelCase and is used to describe variable names and functions alike, so be sure to use camelCase when you define variables or functions, etc.

Next, the function after its name has a set of parenthesis, inside the parenthesis you'll provide arguments, these are the specific details that are provided to the function. Think of the arguments as an input that is used by the function and the output is based on the information provided by the input. Before providing the argument, a placeholder typically exists in the form of what's called a parameter. The pinMode(); function has 2 parameters therefore requires 2 arguments, the digitalWrite(); function also has 2 parameters therefore requiring 2 arguments, and the delay(); function only has 1 parameter therefore requiring 1 argument. If a function requires more than 1 argument, you separate the argument by a comma. (More on that below).

Built-in functions can be found here:

```
pinMode();
digitalWrite();
delay();
```

1. pinMode(); is a function that configures a specific pin to behave either as an input or an output. It has 2 parameters/arguments - the first is the pin and the second is the mode. The mode will be in all caps and either INPUT, OUTPUT, or INPUT_PULLUP.
   1. INPUT - sets the pin as an input which makes it possible to read data from a sensor
   2. OUTPUT - sets the pin as an output, allows you to provide power to components like LEDS
   3. INPUT_PULLUP - similar to INPUT but also enables an internal pull-up resistor which is useful for buttons or switches

An example:

```
    pinMode(1, INPUT_PULLUP)
```

_Hint_ The above is an example where 2 arguments are provided, you'll need to use the example to figure out how to write the code for the built-in LED at pin 13 and select the appropriate mode.

2. digitalWrite(); is a function used to write a HIGH or LOW value to a digital pin. If the pin has been configured as an OUTPUT with pinMode(); you can control a component. HIGH will give power to the value while LOW will not.

An example:

```
    digitalWrite(1, HIGH);
```

3. delay(); is a function that pauses the program for a specified number of milliseconds, during the delay, no other code runs.

An example:

```
    delay(5000);
```

The above delay function pauses for 5 seconds.

### Putting it all together

Now, you have all the information required to create your own program. Your task is to write a program that uses the built-in LED at pin 13 to turn on, pause for one second, turn off, pause for one second.

You'll need to:

1. Define an integar variable assigned to a numeric value where the numeric value is the pin for the built-in LED
2. Use the 3 functions provided above - you'll use one of the three in the setup function:

```
    void setup() {
        //one of the three variables will go here
    }
```

3. Use the other 2 functions provided in the loop function:

```
    void loop() {
        //use the other two variables here
    }
```

### Sending Code to the Arduino Board

1. Verify the Code - Find the Check Mark icon at the top left corner and click on it, this is the "Verify" button - it verifies that the code you wrote is error free which if it isn't it'll tell you in red in the below panel of the IDE

2. Upload the Code - Next to the Verify button is the button to upload the program to the Arduino board, if the code was verified and didn't have errors, once you click this button the Arduino IDE will send the code to the Arduino board

That's it! By following these steps, you can write, verify, and upload your blink program to the Arduino board using the Arduino IDE. If you encounter any issues, double-check your code, board, and port selections. (You should have selected the port in Lesson 0).

### Next steps

If the built-in LED on the Arduino board is turning on then pausing for one second, then turning off, and pausing for another second on-repeat, then you've done it! You completed the project and can now experiment by changing the delay values!

### Summary

You've created your first program/project! You learned how to: 1. define variables in the Arduino IDE 2. learned of function parameters/arguments 3. used built-in functions that Arduino provides 4. how to verify and upload your code from the Arduino IDE to the Arduino board
