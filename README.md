# 📷 Python Screenshot Tool

##  Overview

This project is a lightweight and user-friendly **Python-based screenshot tool** with a graphical interface. Built using **Tkinter** and **PyAutoGUI**, this tool allows you to capture the entire screen with a single click and save the screenshot with a custom filename and location.

---

##  Features

* Simple GUI built using **Tkinter**
* Captures the **entire screen** using **PyAutoGUI**
* Prompts user to **choose save location and filename**
* Saves image as `.png` with `_screenshot` suffix
* Minimal and easy to use

---

##  How It Works

### 1. **Imports Libraries**

```python
import pyautogui
import tkinter as tk
from tkinter import filedialog
```

* `pyautogui` – used for screen capture
* `tkinter` – used for GUI and file dialog

### 2. **Create GUI Window**

* A Tkinter window appears with a canvas (for potential enhancements)
* A button labeled **"Take Screenshot"** is displayed

### 3. **Define Screenshot Function**

```python
def take_screenshot():
    screenshot = pyautogui.screenshot()
    file_path = filedialog.asksaveasfilename(defaultextension=".png", filetypes=[("PNG files", "*.png")])
    if file_path:
        screenshot.save(file_path.replace('.png', '') + "_screenshot.png")
```

* Captures the screen
* Opens a file dialog to select save path and name
* Appends `_screenshot.png` to the saved file

### 4. **Run the Application**

* The program initializes the GUI loop and waits for the user to click the screenshot button.

---

##  Usage Instructions

1. Run the Python script.
2. Click **Take Screenshot**.
3. Choose where to save the image and enter a filename.
4. Screenshot will be saved as `yourfilename_screenshot.png`.

---

##  Requirements

* Python 3.x
* `pyautogui`
* `tkinter` (usually comes with Python)

Install dependencies:

```bash
pip install pyautogui
```

---

##  Future Enhancements

* Add region selection for partial screenshots
* Add image preview
* Keyboard shortcut integration
* Screenshot history view

---

## ⚠️ Disclaimer

This tool is intended for personal or educational use. Make sure you have permission to capture content on the screen.

---

Happy Capturing! 
