```.py
def calendar(output=str):
    m = 2
    y = 2022

    month = {1: 'January', 2: 'February', 3: 'March',t
             4: 'April', 5: 'May', 6: 'June', 7: 'July',
             8: 'August', 9: 'September', 10: 'October',
             11: 'November', 12: 'December'}

    days_1 = f"       1  2  3  4  5"
    days_2 = f"6  7  8  9  10 11 12"
    days_3 = f"13 14 15 16 17 18 19"
    days_4 = f"20 21 22 23 24 25 26"
    days_5 = f"27 28"

    print(month[m], y)
    print('Su', 'Mo', 'Tu', 'We', 'Th', 'Fr', 'Sa')

    days = f"{days_1}\n {days_2}\n {days_3}\n {days_4}\n {days_5}"
    print(days)
    
    return output
```


<img width="1128" alt="Screen Shot 2022-10-09 at 13 12 44" src="https://user-images.githubusercontent.com/111941990/194737734-f7d0c92c-fe84-4c76-9b32-a9b1d9b40c79.png">
