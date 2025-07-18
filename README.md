# 🧪 Auto Potion Macro for Online MMORPG Game

A Python-based automation framework that detects real-time screen metrics and triggers keyboard inputs based on thresholds.


## ⚙️ Overview

This project demonstrates real-time screen analysis and automation using Python. It captures specific on-screen regions (like health/mana bars or progress meters), interprets pixel data to determine status, and automatically responds via simulated key presses.

Originally designed for a game environment, this tool showcases concepts applicable to:

- Process monitoring
- Automated testing (GUI-based software)
- Digital health monitoring (e.g., color-coded dashboards)
- Assistive technologies


## 🧠 Key Features

- Detects pixel-based thresholds from defined screen regions using OpenCV, NumPy, and Pillow
- Real-time automation with keyboard input via PyAutoGUI and pydirectinput
- Configurable triggers (e.g., if on-screen bar drops below X%)
- Modular GUI to toggle automation scripts and visualize their states
- Hotkey control and background operation support


## 🖥️ Use Cases

- Automated UI interaction in testing or simulation environments
- Monitoring visual indicators (e.g., progress bars, system dashboards) and responding automatically
- Game bot prototyping for AI behavior studies (non-commercial/personal use)
- Vision-based automation where API hooks are not available


##🔧 Tech Stack

- Python 3.10+
- Libraries: OpenCV, PyAutoGUI, Pillow, NumPy, keyboard, pydirectinput
- GUI: Built with native tkinter
- Packaging: pyinstaller for executable generation


## 🔧 Requirements
- Windows OS
- Python 3.10+
- Modules: `pyautogui`, `cv2`, `numpy`, `pydirectinput`, `keyboard`, `pillow`


## 🔧 Installation

- Clone this repo
- cd python-automation
- Open cmd using Administrator mode 


## Virtual Environment (Recommended)

- python -m venv venv
- venv\Scripts\activate


## Install dependencies via pip:

`
git clone https://github.com/dkim179/python-automation.git
cd python-automation
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
`


## Important!!
Adjust HP/MP region if needed
The script uses hard-coded regions:


## ⚠️ Before You Start

Adjust HP/MP region if needed
The script uses hard-coded regions:

hp_bar_region = (80, 8, 164, 6)
mp_bar_region = (80, 22, 164, 6)

Modify them if your UI layout differs.


## **How It Works!!!**

1. Captures screenshots of target screen areas
2. Applies color masking and HSV filtering to detect bar levels
3.Calculates color fill percentage using pixel analysis
4. If thresholds (e.g., HP < 87%) are met, triggers hotkeys to simulate a response
5. Repeats in a loop, enabling fully automated decision-making


## 🧩 Build as Executable (Optional)

pip install pyinstaller
pyinstaller --onefile --windowed --uac-admin GUI.py


----------------------------------------------------------------------------------------------------


## 🎮 Auto Heal Macro GUI Usage

### 1. Install pyinstaller

- cd python-automation
- venv\Scripts\activate
- pip install pyinstaller
- pyinstaller --onefile --windowed --uac-admin GUI.py

- This will generate a /build, /dist, GUI.spec
- ***GUI.exe is located in /dist folder/***

---

### 1.1. Location of GUI Executable

- Create a **New Folder** in your "Desktop"
- Copy and Paste "GUI.exe, practice.py, main.py"
- `GUI.exe`, `main.py`, and `practice.py` **must be located in the same folder**.

---

### 2. Key Features of the GUI

- Start/stop macros for **(main.py)** and **(practice.py)** with button clicks  
- Displays each macro's status (Running / Stopped)  
- Automatically stops all running macros when the program closes

---

### 3. How to Run

1. Run the GUI within a Python 3 environment, or  
2. Double-click the built `GUI.exe` file to launch it.

---

### 4. Administrator Privileges

- Administrator privileges are required to run the macros.  

---

### 5. Hotkeys

- F1: Start macro  
- F2: Pause macro

---

### 6. Notes

- You can directly modify the code to adjust thresholds, delays, and other settings.

---

If you have any questions or issues, please open a ticket on the [Issues](https://github.com/dkim179/python-automation/issues) tab!


## ⚠️ Disclaimer
This tool is for personal and educational use only.
Use at your own discretion. Some games may consider automated input as a violation of terms of service, so please check the game's policy before using this tool in competitive or online environments.
