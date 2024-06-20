# python_screenshot_maker
This Python code creates a simple screenshot tool with a user-friendly interface:

1. Imports libraries: It uses "pyautogui" to capture screenshots and "tkinter" to build a graphical interface.

2. Creates a window: A window appears with a designated area (canvas) for potential future use.

3. Defines "Take Screenshot" function: Clicking the button with this label triggers the function:
   - Captures the entire screen using "pyautogui".
   - Prompts you to choose a location and filename to save the screenshot.
   - Saves the screenshot as a PNG image with "_screenshot.png" added to the filename.

4. Runs the program: This keeps the window open and waits for you to click the button.

In essence, it's a user-friendly way to capture screenshots on your computer and save them with a custom name!
