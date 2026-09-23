# SWITCH-CONTROL--PWM

## AIM 
Analyse switch-controlled PWM operation by varying LED brightness through 0%, 25%, 50%, 75%, and 100% for successive switch presses. Reverse the sequence after reaching maximum brightness to simulate wiper-speed control. 


## Apparatus Required

| S. No. | Apparatus / Software | Specification |
|:---:|---|---|
| 1 | Microcontroller Development Board | **NXP S32K144 Development Board** |
| 2 | IDE | **S32 Design Studio** |
| 3 | Programming Language | **Embedded C** |
| 4 | SDK | **S32K144 SDK** |
| 5 | LED | On-board LED / External LED |
| 6 | Programmer / Debugger | On-board Debugger / OpenSDA |
| 7 | USB Cable | For programming and power supply |

---
## Procedure
1. Connect the S32K144 Development Board to the computer using a USB cable.
2. Open S32 Design Studio.
3. Create a new project for the S32K144 microcontroller.
4. Select and configure the appropriate S32K144 SDK for the project.
5. Identify the GPIO pin connected to the LED on the S32K144 development board.
6. Configure the selected GPIO pin/Drivers as a Digital Output/input.
7. Initialize the required GPIO peripheral using the GPIO initialization functions provided by the S32K144 SDK.
8. Write the Embedded C program to control the LED using the GPIO Toggle-Pin API.
9. Insert a one-second delay between successive GPIO toggle operations.
10. The program should continuously execute the following sequence.
11. Build the project in S32 Design Studio.
12. Verify that the project is compiled successfully without errors.
13. Connect the debugger/programmer to the S32K144 Development Board.
14. Download the generated program to the S32K144 microcontroller.
15. Run the program on the S32K144 board.

---
## OUTPUT


<img width="525" height="354" alt="image" src="https://github.com/user-attachments/assets/94bb31da-0093-48ea-8d11-9125f3ef2288" />

## Result

The switch-controlled PWM operation was successfully implemented. The LED brightness was varied through **0%, 25%, 50%, 75%, and 100%** for successive switch presses. After reaching maximum brightness, the PWM duty cycle was decreased in the reverse sequence to **75%, 50%, 25%, and 0%**, successfully simulating **wiper-speed control**.
