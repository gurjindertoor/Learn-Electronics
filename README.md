# Learn-Electronics

The purpose of this repository is to teach new users of the Houston Robotics Group that have limited experience in electronics the basics of electronics.

## Lesson 0: Set-up of Arduino board

## 1. What is Arduino?

Arduino is a popular open-source electronics platform based on easy-to-use hardware and software. An Arduino board is a microcontroller, which essentially is a small, programmable computer dedicated to running one specific task at a time.

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

Voila! You've now downloaded the Arduino IDE, created your first sketch, and connected and set up the Arduino to recieve code.

## Lesson 1: Arduino Board/Software Basics

At its heart, an Arduino board is a microcontroller, which is essentially a small, programmable computer dedicated to running one specific task at a time. It reads inputs - like signals from buttons, sensors, or data from other devices - and processes these inputs using a set of predefined instructions (your code). Then, it performs actions or generates outputs based on this processing, such as turning on an LED, activating motors, or sending data to a computer. This makes Arduino ideal for a wide range of interactive projects, from simple LED displays to complex robotic systems.

### Inputs, further explained

Think of inputs as the information or signals that the Arduino gets from the outside world. It's like how we use our senses to understand what's happening around us. Here are examples of what it listens to:

_Sensors_: These are like the Arduino's senses. They can pick up on things like how warm or cold it is (temperature), whether it's bright or dark (light), if something is pressing against them (pressure), or if something is moving nearby (motion).

_Buttons and Switches_: These are like simple commands. When you press a button or flip a switch, it tells the Arduino to start or stop doing something.

_Communication from Other Devices_: The Arduino can also get info from other gadgets like computers, smartphones, or even other Arduino boards. It's like receiving a text message telling it what to do.

### Outputs, further explained

Outputs are all about how the Arduino responds to what it hears. It's like how we talk or act in response to what we hear or see. Here are the ways it can react:

_Activating an LED_: This is like the Arduino saying, "Got it!" with a light signal. Turning an LED on or off is a simple way for it to show a response.

_Driving Motors_: This is when the Arduino gets active. It can make things move, like spinning a motor to drive a wheel or move an arm.

_Sending Data_: Sometimes, the Arduino's response is to send a message back. It can send data to other devices or even post something online.

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

You've now learned that the Arduino board receives inputs and outputs, the different parts of an Arduino sketch/program, the basic data types used in the Arduino programming language, and what functions are. Next you'll apply all of these skills and create your first program!

## Lesson 2: Creating your first program/project!

The 'Blink' program is typically the first program/project that new users of Arduino create. The Arduino board has a built-in light emitting diode (LED) on pin 13.

In Arduino, a pin is often controlled by assigning it to a variable. Keep this in mind as you create this project.

This section will cover the necessary information for you to create the program by giving you enough information to do it yourself without giving you the answer outward, but if you get stuck there will be a list of instructions at the end of the section. However, feel free to ask for help or practice your research skills if you run into any problems.

### Built-in functions required for this program/project

```
pinMode();
```

```
digitalWrite();
```

```
delay();
```
