```.py
number_lockers = 2400

#2
for locker in range(1, number_lockers+1, 1):
    print(f"Locker No {locker}")
    """
    index = 1
    while index < number_lockers + 1:
        print(f"[While]Locker No {locker}")
        index +=1
    """
    #3: Create the sequence
    # 1.(4n +1) 2. if statements 3. module operator +lists

    color_code = locker % 4
    if color_code == 0:
        color = "blue"
        if color_code == 1:
            color = "red"
        if color_code == 2:
            color = "white"
        if color_code == 3:
            color = "yellow"

    #MORE EFFICIENT
    colors = ["blue", "red", "white", "yellow"]
    color = colors[color_code]

    #4. print results
    #print(f"Locker No {number_lockers} is color {color.upper()}")
    #print(f"Locker No {locker}, {color}")
    print(f"Locker No {locker} is color {color.upper().center(50,'.')}")
```

