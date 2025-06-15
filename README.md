# pymavlink_sitl_tutorial

This repository is a step-by-step tutorial for using ArduPilot SITL with pymavlink in Python.

## Overview

This project shows how to:
- Install and run SITL
- Connect using pymavlink
- Send basic commands (arm, takeoff, land)
- Read telemetry (GPS, battery, attitude)
- Upload simple missions via Python

## Project Structure

pymavlink_sitl_tutorial/
├── setup/                # SITL and MAVProxy install script
├── sitl/                 # SITL launch script
├── tutorials/            # Python examples (connect, fly, etc.)
├── utils/                # Reusable pymavlink functions
├── docs/                 # Setup guides
├── requirements.txt      # Python dependencies
└── README.md             # This file

## Requirements

- Python 3.8+
- WSL2 or Linux
- Internet access

## Installation

git clone https://github.com/mohammedaissi/pymavlink_sitl_tutorial.git
cd pymavlink_sitl_tutorial
pip install -r requirements.txt

cd setup
./sitl_install.sh

## Run SITL

cd ../sitl
./start_sitl.sh

## Run First Script

python tutorials/01_connect.py

## Tutorials

01_connect.py           # Connect to SITL  
02_arm_takeoff.py       # Arm and take off  
03_telemetry.py         # Read GPS and attitude  
04_set_mode.py          # Change flight mode  
05_mission_upload.py    # Upload waypoint mission  
06_land_disarm.py       # Land and disarm

## References

ArduPilot SITL: https://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html  
pymavlink: https://github.com/ArduPilot/pymavlink  
MAVProxy: https://ardupilot.org/mavproxy/

## Author

Mohammed Aissi  
GitHub: https://github.com/mohammedaissi  
LinkedIn: https://www.linkedin.com/in/mohammedaissi

## License

MIT License
