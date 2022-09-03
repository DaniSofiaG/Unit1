# Sum of three numbers
```.py
#Write a program that takes three numbers and prints their sum. Every number is given on a separate line.
#This program reads two numbers and prints their sum:
#Can you change it so it can add three numbers?
a = int(input(3))
b = int(input(2))
c = int(input(5))

print(a + b + c)
```
<img width="615" alt="Screen Shot 2022-09-03 at 8 38 35" src="https://user-images.githubusercontent.com/111941990/188246725-579a9880-b17e-4ebd-9ed9-b486b2f5a867.png">


# Hi John
```.py
#Write a program that greets the person by printing the word "Hi" and the name of the person. See the examples below.
name = input()
print('Hi', name)
```
<img width="616" alt="Screen Shot 2022-09-03 at 8 35 50" src="https://user-images.githubusercontent.com/111941990/188246946-9f814928-dfba-4221-8aa1-f150118c02f1.png">

# Square
```.py
#Write a program that takes a number and print its square.
number = int(input())
print(number**2)
```
<img width="629" alt="Screen Shot 2022-09-03 at 8 36 23" src="https://user-images.githubusercontent.com/111941990/188247080-93739ba5-2506-4b35-aa21-668b4e8a7129.png">

# Area of right-angled triangle
```.py
#Write a program that reads the length of the base and the height of a right-angled triangle and prints the area. Every number is given on a separate line.
b = int(input())
h = int(input())

print(b*h/2)
```
<img width="618" alt="Screen Shot 2022-09-03 at 8 36 37" src="https://user-images.githubusercontent.com/111941990/188247207-fa24e263-c9e7-442f-aadc-2a457a0f15a8.png">

# Hello, Harry!
```.py
#Write a program that greets the user by printing the word "Hello", a comma, the name of the user and an exclamation mark after it. See the examples below.
Warning. Your program's output should strictly match the desired one, character by character. There shouldn't be any space between the name and the exclamation mark. You can use + operator to concatenate two strings. See the lesson for details.
name = input()

print('Hello, ' + name + '!')
```
<img width="608" alt="Screen Shot 2022-09-03 at 8 36 52" src="https://user-images.githubusercontent.com/111941990/188247309-a9fc0c13-3098-4471-b7c5-64ce76d55f31.png">

# Apple sharing
```.py
#N students take K apples and distribute them among each other evenly. The remaining (the undivisible) part remains in the basket. How many apples will each single student get? How many apples will remain in the basket?
The program reads the numbers N and K. It should print the two answers for the questions above.
n = int(input())
k = int(input())

print(k // n)
print(k % n)
```
<img width="609" alt="Screen Shot 2022-09-03 at 8 37 05" src="https://user-images.githubusercontent.com/111941990/188247431-7bf76242-7110-48ae-bc70-36e150d366eb.png">

# Previous and next
```.py
#Write a program that reads an integer number and prints its previous and next numbers. See the examples below for the exact format your answers should take. There shouldn't be a space before the period.
Remember that you can convert the numbers to strings using the function str.
a = int(input())

print('The next number for the number ' + str(a) + ' is ' + str(a+1) + '.')
print('The previous number for the number ' + str(a) + ' is ' + str(a-1) + '.') 
```
<img width="621" alt="Screen Shot 2022-09-03 at 8 37 19" src="https://user-images.githubusercontent.com/111941990/188247509-950b8df9-7572-47d0-a81a-ffb131d7cb1a.png">

# Two timestamps
```.py
#A timestamp is three numbers: a number of hours, minutes and seconds. Given two timestamps, calculate how many seconds is between them. The moment of the first timestamp occurred before the moment of the second timestamp.
a_hours = int(input())
a_minutes = int(input())
a_seconds = int(input())


b_hours = int(input())
b_minutes = int(input())
b_seconds = int(input())

print((b_hours*60)*60 + b_minutes*60 + b_seconds - ((a_hours*60)*60 + a_minutes*60 + a_seconds))
```
<img width="612" alt="Screen Shot 2022-09-03 at 8 37 33" src="https://user-images.githubusercontent.com/111941990/188247569-7d1dd652-9efe-4e70-b83c-f872fb45a1bf.png">

# School desks
```.py
#A school decided to replace the desks in three classrooms. Each desk sits two students. Given the number of students in each class, print the smallest possible number of desks that can be purchased.
The program should read three integers: the number of students in each of the three classes, a, b and c respectively. In the first test there are three groups. The first group has 20 students and thus needs 10 desks. The second group has 21 students, so they can get by with no fewer than 11 desks. 11 desks is also enough for the third group of 22 students. So we need 32 desks in total.
a = int(input()) 
b = int(input())
c = int(input())

print(a//2 + b//2 + c//2 + a%2 + b%2 + c%2)
```
<img width="599" alt="Screen Shot 2022-09-03 at 8 37 47" src="https://user-images.githubusercontent.com/111941990/188247619-6f23a52d-4a27-48fc-9193-860e1c332c07.png">

