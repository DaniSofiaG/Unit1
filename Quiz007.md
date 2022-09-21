```.py

#gernerate 10 random passwords
print("Password Generator")
import random
num_passwords = 10
length = int(input("Enter password length: "))
characters = "0123456789abcdefghijklmnñopqrstuvwxyzABCDEFGHIJKLMNÑOPQRSTUVWXYZ"
characters_symbols = "0123456789abcdefghijklmnñopqrstuvwxyzABCDEFGHIJKLMNÑOPQRSTUVWXYZ##:/%!&¿?$*+;#_"

symbols_ask= input("Do you want symbols to be included? yes or no")

if symbols_ask == "no":
    for x in range(num_passwords):
        password = ""
        for x in range(length):
            password_characters = random.choice(characters)
            password = password + password_characters
        print(f"Here is a random password:", {password})

if symbols_ask == "yes":
        for x in range(num_passwords):
            password = ""
            for x in range(length):
                password_characters = random.choice(characters_symbols)
                password = password + password_characters
            print(f"\33[0;31m{password}")
```

<img width="1397" alt="Screen Shot 2022-09-19 at 19 42 15" src="https://user-images.githubusercontent.com/111941990/191000945-10b96aa2-efde-49df-9ba4-dd42a3b7c738.png">

<img width="511" alt="Screen Shot 2022-09-21 at 16 58 38" src="https://user-images.githubusercontent.com/111941990/191448794-c4e9614c-4951-4b99-9b7c-90c7ba8d36dc.png">

..
