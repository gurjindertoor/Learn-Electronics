## 1. Setup and Loop Functions

In every Arduino sketch, you have two main functions: setup() and loop(). setup() is called once when the sketch starts and is used for initializations. loop() is called repeatedly and contains the main code that runs continuously.

To "call" a function in programming, including in Arduino sketches, means to tell the program to execute the set of instructions defined within that function. When you call a function, you're essentially instructing the program to jump to that function, carry out the tasks defined in it, and then return to the point where it was called to continue executing the remaining code.

### Example:

```
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); // Initialize the LED pin as an output
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH); // Turn the LED on
  delay(1000);                     // Wait for a second
  digitalWrite(LED_BUILTIN, LOW);  // Turn the LED off
  delay(1000);                     // Wait for a second
}

```
