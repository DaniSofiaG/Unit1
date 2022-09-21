```.py

number = int(input("Enter an integer"))


for i in range(1, number + 1):
    if number % i == 0 and i < number:
        output = True
        comma = ","
        print(i, comma, end=" ")
print(output)
```


<img width="1398" alt="Screen Shot 2022-09-15 at 16 12 57" src="https://user-images.githubusercontent.com/111941990/190339221-465df164-30c1-4c64-96d1-3c4e37c6d3f1.png">


<img width="501" alt="Screen Shot 2022-09-21 at 16 16 43" src="https://user-images.githubusercontent.com/111941990/191439777-8cb35410-f167-4acd-a640-7dcf4e463e6e.png">
