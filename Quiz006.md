```.py

text = input("Write a word:")
sum = 0
for ascii in text:
    code = ord(ascii)
    if code<91: # upper case
        sum = sum + code
    if code> 96:
        sum = sum + code
print(f"The code for your {text} is {sum}")

text = input("Write a second word:")
sum = 0
for ascii in text:
    code = ord(ascii)
    if code<91: # upper case
        sum = sum + code
    if code> 96:
        sum = sum + code
print(f"The code for your {text} is {sum}")
```

<img width="1399" alt="Screen Shot 2022-09-19 at 18 36 34" src="https://user-images.githubusercontent.com/111941990/190990454-73d7f044-7106-4486-bb17-c8e264a0382a.png">
