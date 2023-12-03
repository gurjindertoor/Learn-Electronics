# Learn-Electronics

The purpose of this repository is to teach new users of the Houston Robotics Group the basics of electronics. This will be a repository that's continually updated to provide more lessons/concepts.

The user can currently learn:

1. How to up an Arduino board - downloading the Arduino IDE, creating sketches, connecting an Arduino board to a computer
2. The basics of programming in the Arduino IDE - basic data types, functions, and parts of the Arduino program/sketch
3. Create a first project - 'Blink'

## Lesson 0: Setting up an Arduino board

## 1. What is Arduino?

Arduino is a popular open-source electronics platform based on easy-to-use hardware and software. An Arduino board is a microcontroller, which is a small, programmable computer dedicated to running one specific task at a time.

## 2. How to Download the Arduino IDE

### What is an Integrated Development Environment (IDE)?

An IDE is a software application where you can write, edit, and test your programs/code all in one place, it's packed with a lot of helpful tools such as a text-editor and error-checker.

### Arduino IDE

The Arduino IDE is the main software used to program an Arduino. You'll be able to send your code to the Arduino board via the Arduino IDE. To download it:

1. Visit the official Arduino website: arduino.cc
2. Navigate to the Software section.
3. Download the version compatible with your operating system (Windows, macOS, or Linux).

## 3. Programming Language Used by Arduino

Arduino uses a programming language based on C/C++. It's simplified and has many built-in functions to easily control the hardware.

If you don't have any programming experience or have never programmed in C/C++, don't worry! You'll get a quick crash course that'll set you up to start creating your own projects further into the tutorial!

## 4. Setting Up an Arduino Script

Once the Arduino IDE is downloaded, in order to set up an Arduino script, do the following:

1. Open the Arduino IDE.
2. Start a new sketch (a sketch is an Arduino program).
3. Write or paste your code into the IDE.

## 5. Connecting Arduino to Your Computer and the IDE

1. Connect the Arduino board to your computer using a USB cable.
2. Open the Arduino IDE.
3. Go to Tools > Board and select your Arduino model.
4. Go to Tools > Port and select the port that your Arduino is connected to.

### 6. Research Skills and Troubleshooting

Remember, a lot of working with electronics and software involves research and problem-solving skills. If you're stuck:

1. Ask clear, specific questions.
2. Use search engines to find solutions.
3. Visit forums and communities like Stack Overflow or the Arduino forums.
4. Experiment and learn from trial and error.

### Summary

Voila! You've now:

1. downloaded the Arduino IDE
2. created your first sketch
3. connected and set up the Arduino board to recieve code

## Lesson 1: Arduino Board/Software Basics

At its heart, an Arduino board is a microcontroller, which is essentially a small, programmable computer dedicated to running one specific task at a time. It reads inputs - like signals from buttons, sensors, or data from other devices - and processes these inputs using a set of predefined instructions (your code). Then, it performs actions or generates outputs based on this processing, such as turning on an LED, activating motors, or sending data to a computer. This makes Arduino ideal for a wide range of interactive projects, from simple LED displays to complex robotic systems.

### Inputs, further explained

Think of inputs as the information or signals that the Arduino gets from the outside world. It's like how we use our senses to understand what's happening around us. Here are examples of what it listens to: 1. Sensors: These are like the Arduino's senses. They can pick up on things like how warm or cold it is (temperature), whether it's bright or dark (light), if something is pressing against them (pressure), or if something is moving nearby (motion). 2. Buttons and Switches: These are like simple commands. When you press a button or flip a switch, it tells the Arduino to start or stop doing something. 3. Communication from Other Devices: The Arduino can also get info from other gadgets like computers, smartphones, or even other Arduino boards. It's like receiving a text message telling it what to do.

### Outputs, further explained

Outputs are all about how the Arduino responds to what it hears. It's like how we talk or act in response to what we hear or see. Here are the ways it can react: 1. Activating an LED: This is like the Arduino saying, "Got it!" with a light signal. Turning an LED on or off is a simple way for it to show a response. 2. Driving Motors: This is when the Arduino gets active. It can make things move, like spinning a motor to drive a wheel or move an arm. 3. Sending Data: Sometimes, the Arduino's response is to send a message back. It can send data to other devices or even post something online.

### Input/Output Summary

An Arduino board works by taking in information (inputs) and reacting to it (outputs). Think of it like listening and then responding: the board listens to what's happening around it through sensors or commands, and then responds by doing something, like lighting up an LED or moving a motor.

## 2. Different Parts of an Arduino Script

When you start a new sketch, you'll see a few pieces of code. An Arduino script typically includes:

1. Setup: A function that runs once at the start. Used for initializing settings.
2. Loop: A function that runs continuously. This is where most of your code will go.
3. Comments: Lines starting with //, used to describe what the code does.
4. Functions: Blocks of code that perform specific tasks.

## 3. Basic Data Types, Functions, Software

### Basic Data Types in Arduino

1. int - Represents integer values. It's used for numbers without a decimal point. For example, int count = 10;
2. float - For floating-point numbers, or numbers with a decimal. Useful for more precise measurements like float temperature = 36.5;
3. char - Stands for 'character' and is used to store single characters like letters or symbols. For instance, char letter = 'A';
4. String - Used for storing a sequence of characters or text. For example, String name = "Arduino";
5. boolean - Represents true or false values, often used in conditional statements. For example, boolean isOn = true;
6. byte - Represents true or false values, often used in conditional statements. For example, boolean isOn = true;

### Functions

Functions are blocks of code that perform a specific task. They're like mini-programs within your main program. Arduino provides built-in functions within the IDE that you're able to use, these are pieces of code that provide a specific task already created and defined by Arduino that provide a lot of functionality. You'll create your own functions as you gain experience.

### Semi-colon

Every block of code in the Arduino IDE needs to end with a semi-colon (;), otherwise the code will run into errors. The purpose of the semi-colon is to tell the Arduino compiler where one instruction ends and another begins, without it, the compiler gets confused trying to read multiple instructions as one and this leads to errors.

### Summary:

You've now learned:

1. Arduino board receives inputs/outputs
2. the different parts of an Arduino sketch/program
3. the basic data types used in the Arduino programming language
4. what functions are

Next you'll apply all of these skills and create your first program!

## Lesson 2: Creating your first program/project!

The 'Blink' program is typically the first program/project that new users of Arduino create. The Arduino board has a built-in light emitting diode (LED) on pin 13.

In Arduino, a pin is often controlled by assigning it to a variable. Keep this in mind as you create this project.

![Arduino-Board-LED](https://github.com/gurjindertoor/Learn-Electronics/assets/78512847/0aeefc69-11e0-47b6-ac9f-0ed5a2ac13c2)

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

You've created your first program/project! You learned how to:

1. define variables in the Arduino IDE
2. learned of function parameters/arguments
3. used built-in functions that Arduino provides
4. how to verify and upload your code from the Arduino IDE to the Arduino board
