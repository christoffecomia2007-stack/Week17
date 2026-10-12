# Simulated Device Monitoring and Alert System
 
**Student Name:** (Kale Christoffe C. Comia)
**Student Number:** (2601334)
**Section:** (1CPE-A)
 
## Project Description
This program monitors simulated device temperature readings using Python. It classifies each temperature reading as NORMAL, WARNING, or CRITICAL based on predefined temperature limits.
 The program also calculates the total, average, minimum, and maximum temperatures and displays the percentage of readings in each category. It determines the overall monitoring status and validates user input to prevent invalid readings and menu choices.
 
## Features
- View all stored temperature readings
- Add a new reading (whole numbers from 0 to 100 only)
- Classify every reading
- Generate a numerical summary and overall status
- Reject invalid menu choices and invalid readings
 
## Requirements
- Python 3 (no external packages)
 
## How to Run
1. Open a terminal inside the Week17 folder.
2. Type: python device_monitor.py
   (On macOS or Linux, type: python3 device_monitor.py)
 
## Sample Output

SIMULATED DEVICE MONITORING SYSTEM
----------------------------------
[1] View Readings
[2] Add Reading
[3] Classify Readings
[4] Generate Summary
[5] Exit
Enter choice: 4

MONITORING SUMMARY
------------------
Number of readings : 5
Total of readings : 160
Average temperature : 32.00 °C
Minimum temperature : 28 °C
Maximum temperature : 37 °C

NORMAL : 2 (40.00%)
WARNING : 2 (40.00%)
CRITICAL : 1 (20.00%)
 
## Test Cases
I performed 10 tests. passed and failed. Full details are in test_cases.md.
 
## Known Limitations
-Temperature readings are lost when the program closes because they are stored only in a Python list.
-The program uses simulated temperature readings and does not connect to actual devices or sensors.
-The warning and critical temperature limits are predefined and cannot be changed by the user.
 
## Reflection
The hardest part of this project was creating the functions to classify temperature readings and calculate the monitoring summary accurately. I learned how to use loops, conditional statements, functions, and input validation to process temperature data. I also made sure that invalid menu choices and readings outside the allowed range are rejected by the program. One improvement I would make is to save the readings to a file so that the data will not be lost when the program closes. In the future, I would also like to connect the system to real temperature sensors and add more advanced alerts.
