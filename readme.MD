# Arduino Safe Project

This project implements a simple safe system using an Arduino board, a keypad, an LCD display, and a servo motor for locking and unlocking.

## Components:
1. **Arduino Board**: The brain of the system that controls the overall functionality.
2. **Keypad**: Used for entering the secret code to unlock the safe.
3. **LCD Display**: Provides feedback and instructions to the user.
4. **Servo Motor**: Actuates the locking mechanism to lock and unlock the safe.

## Functionality:
- **Locking Mechanism:** The servo motor is used to physically lock and unlock the safe. It is controlled by the Arduino board.
- **Secret Code:** The user must enter a predefined secret code using the keypad to unlock the safe.
- **User Interface:** The LCD display provides visual feedback to the user, guiding them through the process of entering the secret code and indicating whether the safe is locked or unlocked.
- **EEPROM Storage:** The secret code is stored in the Arduino's EEPROM memory, ensuring that it persists even when the power is turned off.

## Operation:
1. Upon startup, the system displays a welcome message on the LCD screen.
2. If the safe is locked, the user is prompted to enter the secret code using the keypad.
3. If the entered code matches the stored secret code, the safe is unlocked, and the servo motor actuates to unlock the safe.
4. If the entered code is incorrect, the system displays an "Access Denied" message.
5. If the safe is unlocked, the user has the option to set a new secret code by pressing a designated key on the keypad.
6. After setting a new code, or if a new code is not required, the safe automatically locks itself after a brief delay.

## Usage:
- Connect the components according to the specified pin configurations in the code.
- Upload the code to the Arduino board.
- Ensure that the servo motor is properly calibrated to lock and unlock the safe.
- Follow the prompts on the LCD display to lock and unlock the safe using the keypad and secret code.

![Image Description]("C:\Users\ASUS\Desktop\iot task\Screenshot 2024-02-26 204753.png")


## Note:
- This project provides a basic implementation of a safe system for educational purposes. Additional security measures and features can be added based on specific requirements and considerations.
