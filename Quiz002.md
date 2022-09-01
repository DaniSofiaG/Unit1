```.py

#Give 2 numbers, A and B, Outbut TRUE if one of them is 20 or if their sum is 20.

number_A = int(input("Enter number A"))
number_B = int(input("Enter number B"))
output = False

if number_A == 20:
    print("Number A is 20")

if number_B == 20:
    print("Number B is 20")
    output = True

if number_B + number_A == 20:
        print("Number B+A is 20")
        output = True

print(f"The solution is {output}")

#2 lists
list_A = []
list_B = []
output = False

n = input("List A: Enter 4 numbers using , to separate them: ")
n = input("List B: Enter 4 numbers using , to separate them: ")

if list_A == 20:
    output = True
    print("List A is 20")

if number_B == 20:
    print("List B is 20")
    output = True

if list_B + list_A == 20:
        print("list B+A is 20")
        output = True

print(f"The solution is {output}")

```



