## Project Description

# HW-Monitor-Desktop-Widget
Simple desktop widget to keep track of current hardware scenario

HW Monitor Desktop Widget is a lightweight desktop system monitoring tool built using Python. The application displays real-time hardware usage statistics such as CPU usage, RAM usage, Disk usage, and Battery status in a compact floating window on the desktop. The widget is designed to stay on top of all applications and provides quick system status monitoring without opening any heavy software.

The interface is minimal, semi-transparent, and draggable, making it convenient for users who want a small real-time system monitor on their screen.

## Objective

The main objective of this project is to create a simple desktop widget that continuously monitors essential system hardware statistics and displays them in a small, unobtrusive graphical interface.

This project demonstrates how Python can be used to build desktop utilities by combining system monitoring libraries with graphical user interface frameworks.

## Features

* Real-time monitoring of CPU usage
* RAM usage display
* Disk usage monitoring
* Battery percentage and charging status
* Small floating widget window
* Always-on-top display
* Semi-transparent dark themed interface
* Draggable widget (click and drag to move)
* Right-click menu to exit the application
* Automatic refresh every 2 seconds
* Color indication for high resource usage

## Technologies and Libraries Used

Python 3

Libraries:

* tkinter : Used to create the graphical user interface.
* psutil : Used to retrieve system hardware statistics such as CPU, memory, disk, and battery information.

## How the Program Works

1. The program creates a small GUI window using tkinter.
2. The window is customized to remove borders and remain on top of other applications.
3. Labels are used to display hardware information including CPU, RAM, Disk, and Battery status.
4. The psutil library fetches the current system statistics.
5. The statistics are updated every 2 seconds using the tkinter event loop.
6. Color indicators are used to highlight high resource usage (for example, CPU above 85% turns red).
7. The widget can be dragged across the screen by clicking and holding the left mouse button.
8. A right-click menu allows the user to close the widget.

## How to Run the Program

Step 1: Install Python (if not already installed)

Step 2: Install the required dependency

```
pip install psutil
```

Step 3: Save the Python file (for example: hw_monitor.py)

Step 4: Run the script

```
python hw_monitor.py
```

The monitoring widget will appear on the desktop.

## Controls

Left Mouse Click + Drag
Move the widget anywhere on the screen.

Right Mouse Click
Open the menu and select "Exit Monitor" to close the application.

## Displayed Metrics

CPU
Shows the current processor usage percentage.

RAM
Displays the percentage of system memory currently in use.

DSK
Displays the disk usage percentage of the main system drive.

BAT
Shows battery percentage and indicates whether the device is charging or running on battery.

## Possible Improvements / Future Work

* Add GPU monitoring support
* Display CPU temperature
* Add network usage monitoring
* Allow resizing of the widget
* Add customizable refresh intervals
* Provide theme customization options
* Convert the program into a system tray application
* Package the application as a standalone executable

## Conclusion

This project demonstrates how Python can be used to create a functional and visually minimal desktop monitoring tool. By combining tkinter for the interface and psutil for system data, the program provides a practical utility for real-time hardware monitoring.
