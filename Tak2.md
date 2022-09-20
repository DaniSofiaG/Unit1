```.py

#EV_calculator.py
from my_lib import validate_int_input, end_code, colors, bold_white

welcome_msg = "Welcome to the EV Calculator".center(50, "=")
prompt_msg = "Please enter and option [1-4]"

print(f"{colors[2]}{welcome_msg}{end_code}")
print("options".center(50))

menu= """1. Average time kWh
2. Total kWh
3. Total charge time 
4. how all data
"""
print(menu)
option = validate_int_input(prompt_msg)
while option>4 or option < 1:
    option = validate_int_input(f"{colors[1]}Invalid option.{prompt_msg}{end_code}")

#option 4: show all data
with open("changing:log csv.py", "r") as file:
    ev_logs = file.readlines()

if option ==4:
    print(f"{bold_white}4.Showing all data{end_code}")
    index = 0
    for log in ev_logs:
        if index>0:
            print(f"No.{index}: {log}", end="") #strip removers the / at the end of the line
        index +=1
    print(ev_logs)

#option 2: Calculate total energy
if option == 2:
    index = 0
    total_energy = 0
    for log in ev_logs:
        if index > 0:
            values = log.split(",")
            date = values[0]
            energy = values[1]
            time = values[2]
            total_energy += float(energy[0:5])
        index += 1
    print(f"{colors[2]}The total energy charged is {total_energy}kWh")
    ```

