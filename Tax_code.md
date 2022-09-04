```.py 

#Create a program tthat organizes from largest to smallest three heights in cms entered by th euser.
#Create a program that calculates the tax for a salary entered by the user following the table below

print("Insert salary")
salary = int(input())

if not (salary < 10.000):
    tax_5 = salary * 5 / 100
    print(tax_5)

elif not (salary > 50.000):
        tax_10 = salary * 10 / 100
        print(tax_10)

elif not (salary>100.000):
        tax_15 = salary * 15 / 100
        print(tax_15)

elif not (salary>100.001):
        tax_25 = salary * 25 / 100
        print(tax_25)
  ```

<img width="1440" alt="Screen Shot 2022-09-04 at 23 06 23" src="https://user-images.githubusercontent.com/111941990/188317836-5ed63ec4-b479-4ed0-aced-a518104cd5c7.png">
