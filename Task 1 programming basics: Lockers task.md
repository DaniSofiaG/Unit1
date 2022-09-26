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
<img width="1436" alt="Screen Shot 2022-09-14 at 14 29 22" src="https://user-images.githubusercontent.com/111941990/190067558-12041010-9648-4280-948f-ecdce9c5696d.png">

<img width="712" alt="Screen Shot 2022-09-19 at 20 18 19" src="https://user-images.githubusercontent.com/111941990/191006445-de41e464-26ca-432a-9e5a-9a1d81606fc7.png">

<img width="705" alt="Screen Shot 2022-09-26 at 9 36 54" src="https://user-images.githubusercontent.com/111941990/192173447-de8e665a-d685-4420-80ed-8238a1a97258.png">

<img width="698" alt="Screen Shot 2022-09-19 at 20 18 26" src="https://user-images.githubusercontent.com/111941990/191006481-082a035f-8e7f-4f98-9f90-251268205535.png">



