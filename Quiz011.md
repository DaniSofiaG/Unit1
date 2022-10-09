```.py
def calendar(output=str):
 
    days_1 = f"       1  2  3  4  5"
    days_2 = f"6  7  8  9  10 11 12"
    days_3 = f"13 14 15 16 17 18 19"
    days_4 = f"20 21 22 23 24 25 26"
    days_5 = f"27 28"

    when= "February 2022"
    week_days=(“Su” “Mo”, “Tu”, “We”, “Th”, “Fr”, “Sa”)
    output = f"{when}\n{week_days}\n {days_1}\n {days_2}\n {days_3}\n {days_4}\n {days_5}"
    print(output)
    return output
```


<img width="1128" alt="Screen Shot 2022-10-09 at 13 12 44" src="https://user-images.githubusercontent.com/111941990/194737734-f7d0c92c-fe84-4c76-9b32-a9b1d9b40c79.png">
