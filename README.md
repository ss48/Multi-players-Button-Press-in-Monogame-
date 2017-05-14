# Multi-players-Button-Press-in-Monogame-


To get started
We create a new “MonoGame Windows Store project” call it Button Bash. 
We need to build a program that counts and displays the presses of a single button on the gamepad.
To keep track of the number of times the button has been pressed we define an integer to hold the value;
We need to find a way to tell the program to increase count when the button position changes from up to down and not by holding the button down.
We know that the Update method is called at regular intervals. If the Update method is called the first time and detects that B is up, and the second time it is called it detects B has been pressed. It means that the Update method must perform a test of “If the button was up last time and is down this time, the counter must be increased”. So it needs to test if the button state has changed since the last call.
Thus, we need to declare the state variable to hold this value. 
