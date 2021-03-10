# Collector 

This directory can be used to start a venv with the required python packages to run the GUI + motor control for the collector.

## How to run

1. Start venv
```
source bin/activate
```

2. Start GUI
```
python3 collector.py
```

## Important information 

- This setup was tested on a Raspberry Pi 4 running Raspberry Pi OS
- Using keyboard listener to gather barcode scanner data sometimes results in a runtime error, because the keyboard listener fails to stop freezing the application. Maybe use second thread for keyboard listener that can be stopped from the outside. 
- The stepper motor GPIO python package in `?` was modified to decrease step-size.
