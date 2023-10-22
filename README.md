# Emerging-Sys-Arch
Artifact 1: "pwmled2.c" was designed to control the PWM signals for two LEDs on a TI board. The problem it solved was creating a program to change the duty cycles of two LEDs in a repeating pattern, achieving different brightness levels for these LEDs. It was essentially a hardware control application.

Artifact 2: "uart2echo.c" was developed to echo characters received over UART and control an LED on a Launchpad Board based on user input. This application addressed the need to interact with a user through a UART interface and control an LED accordingly, making it a combination of hardware and user interaction.

What I did particularly well:
1. Clear Code Structure: Your code in Artifact 1 is well-structured and organized. It begins with necessary includes, followed by a structured main function that clearly outlines the program's flow.
2. Error Handling: You've included error handling in the code. For instance, you check if PWM handles are successfully opened and handle cases where they are not.
3. Structured State Machine: You've implemented a structured state machine using an enum (State) to handle different states (e.g., IDLE, LED_ON, LED_OFF). This makes the code easy to follow and maintain.
4. Initialization Check: You check if the UART and GPIO initialization is successful and handle the situation if it fails, ensuring that the program won't continue with uninitialized hardware.

Where I could improve:
1. Error Handling: Both artifacts could benefit from more robust error handling. For example, when initializing or configuring hardware, it's essential to handle potential errors gracefully. If, for some reason, the hardware initialization fails, you might want to provide better feedback or take corrective actions.
2. Comments for Algorithmic Logic: When you have complex logic in your code, such as the duty cycle changing algorithm in Artifact 1, consider adding comments to explain the purpose and logic behind it. This can help others (and yourself) understand the code's behavior.

Tools and resources added to the support network:
I improved my understanding of embedded systems by working with TI's Code Composer Studio and their provided drivers. In future projects, I can leverage this experience and the knowledge gained from working with hardware-specific code.

Transferable skills:
1. Hardware Interaction: Experience with embedded systems and hardware control will be transferable to other projects involving IoT, robotics, or any application that interfaces with physical devices.
2. Code Analysis: The ability to understand and analyze existing code is valuable in software development, especially when dealing with complex systems.
3. Troubleshooting: I developed problem-solving skills, particularly in debugging hardware-related issues, which will be useful in similar projects.

Maintainability, readability, and adaptability:
1. Code Comments: Both artifacts include comments that explain the purpose of code sections and variables, making it easier for others to understand and modify the code.
2. Modularity: Code in both artifacts is divided into functions and structured in a way that allows for future modifications or additions.
3. Parameterization: Key parameters, such as the PWM period in Artifact 1 and UART baud rate in Artifact 2, are defined as variables, making it easy to adapt the code for different hardware or requirements.
4. Error Handling: Both artifacts include error handling to ensure robustness and stability in the face of unexpected issues.
