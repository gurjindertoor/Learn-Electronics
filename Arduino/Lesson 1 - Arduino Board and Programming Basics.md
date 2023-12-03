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

You've now learned: 1. Arduino board receives inputs/outputs 2. the different parts of an Arduino sketch/program 3. the basic data types used in the Arduino programming language 4. what functions are

Next you'll apply all of these skills and create your first program!
