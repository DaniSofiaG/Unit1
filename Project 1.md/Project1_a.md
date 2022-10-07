# Crypto Wallet

![200w](https://user-images.githubusercontent.com/111941990/191906556-dc599fb6-4c12-4790-885e-e96b16a3bfd4.gif)


# Criteria A: Planning

## Problem definition

### Definition of the problem
#### Who is the client?
Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies
#### Why is the product being developed?	
She has started to buy and sell electronic currencies, however at the moment she is tracking all his transactions using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics.



Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |

## Proposed Solution

### Rationale for proposed solution
#### What is the product?
A crypto wallet, a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. This product is an effective solution because unlike other tools such as spreadsheets or material methods like accounting books, it will allow Ms. Sato to access and input her information quickly, securely and in a single place specially designed for her needs. I decided to use the software python because it is a very clear and direct program, which makes the development of a tool like a crypto wallet a lot more user and developer friendly. It's commonly used, thus the information that there is on how to manipulate strings and create functions is very extensive and accessible. Another reason why I decided to use this software is because it is the software with which I feel the most comfortable using, thus increasing the quality of the product for the client. This decision was made fully in consideration of the client’s satisfaction and needs. I structured my code in a way where the user was able to easily understand how to use it when running it. All options have instructions and colored titles to categorize the action the program is running. If there is something to select the program will run purple, as well as if there is title or messages. If the user gives an invalid input and/or selects an option which is not accessible to them, the program will run red. The functions of the program will run in different colors and will match their heading through the use of the same color in different tones or the color nearest to them in the rainbow.  I've added comments throughout the code to identify the different functions and wrote the program in chronological order in order to facilitate the identification of different code sections and/or functions.

### Design statement:
I will be able to design and make an electronic ledger for a client, Ms Sato, who is a local trader, looking for a way to organize and keep track of her transactions. This will run four main functions and will count with obth a log-in and resitration system equpped to set up and personalize her account. This rprogram is specifically made for the cryptocurrency biance coin, but can easily be modified to be use with any cryptocurrency and data, and is constructed using the software pycharm. It will take proper planning and designt to make and will be evaluated according to the criteria A, B and C and the success criteria I have designed in criteria B during the planning of my project

** add a description of your coin and citation **
| Group 1   |              |   | Group  2  |           |
|-----------|--------------|---|-----------|-----------|
| Developer | Digital Coin |   | Developer | Coin      |
| Alex      | Bitcoin      |   | Alek      | Solana    |
| Bernard   | Ethereum     |   | Mai       | Dogecoin  |
| Yutaro    | Dogecoin     |   | Daniela   | BInance   |
| Verlon    | Apecoin      |   | Kris      | Bitcoin   |
| Oswell    | Tether       |   | Paula     | Lumens    |
| Thumula   | Tron         |   | ZAven     | Ethereum  |
| Ainee     | Mana         |   | Jonathan  | Maker     |
| Lison     | Solana       |   | Kai       | Avalanche |
| Sabu      | Binance      |   | Daiichiro | Flow      |
| Emmy      | Polkadot     |   | Masamu    | Cardano   |
| Maria     | Cardano      |   | Yasmina   | Zcash     |
| Zelan     | Cosmos       |   | Jana      | LiteCoin  |
| Manahil   | BinanceUSD   |   | Lyn       | Iota      |
| Krish     | UsdCoin      |   | Meisa     | Polkadot  |
|           |              |   | Mayte     | Cosmos    |
|           |              |   | Pop       | Ripple    |
Justify the tools/structure of your solution

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger displays the basic description of the cryptocurrency selected.
3. The electronic ledger allows users to enter, withdraw and record transactions.
4. The electronic ledger has a system to create and record accounts, so that the client Ms Sato can make her personal account. 
5. The electronic ledger creates a personal file after a new client registers
6. The electronic ledger can reflect the client's current and initial balance


# Criteria B: Design

## System Diagram
![IMG_7301](https://user-images.githubusercontent.com/111941990/194451168-2451c6ef-ef40-44e6-ba95-aa313ba086ae.png)


## Flow Diagrams
### Register and Log-in system Flow chart 3
![Project_ log-in and register system flowchart](https://user-images.githubusercontent.com/111941990/194450705-f3b3dd76-4ac0-4b81-b994-f044984c4e62.png)

### Initaial Balance Flow chart 2
![2nd flowchart](https://user-images.githubusercontent.com/111941990/194595598-4cb6301b-e401-4c7d-8379-2bbed89380cb.jpg)


### Record Transactions Flow chart 1
![3rd Flow chart](https://user-images.githubusercontent.com/111941990/194599362-5e8e4f82-4e5d-4c78-b0d4-e584e8fd97c2.jpg)



## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                                         | To have a clear idea of the hardware and software requirements for the proposed solution                        | 10min         | Sep 24                 | B         |


# Criteria C: Development

## Register and Log-in System
My client Ms Sato, requires a system to create a personal acctount and to protect the data that she inputs into that account. To make this possible I created a register system and worked on the log-in system during class. The register system allows the user to create a personal account with a username and password of their choice, which is appended to a a file that then can be used to continue to the log-in system. Additional to that the registering system creates a file titled with the username created during the registration process, this file is personal and unique to the user. Th elog-in system is a great way to use the data storaged in the file when trying to access the program another time without registering a new account.
```.py
from project_library import colors, end_code, validate_int_input, register, login, initial_balance, transactions, withdraw

#Login and Register

welcome_msg = "Welcome to your crypto wallet".center(50, "=")
prompt_msg = (f"{colors[5]}Log-in if you have an account or register to create a new one [1-2]{end_code}")

print(f"{colors[6]}{welcome_msg}{end_code}")

account= """
1. log-in
2. register
"""
print(f"{colors[5]}{account}{end_code}")
account = validate_int_input(prompt_msg)
while not account in [1,2]:
    account = validate_int_input(f"{colors[1]}Invalid option.{prompt_msg}{end_code}")

with open("db.csv", "r") as file:

    #1.Login
    if account == 1:
        print(f"{colors[4]}1.Log-in{end_code}")
        user= input(f"{colors[6]}Enter your username:")
        password = input(f"{colors[6]}Enter your password:")
        if user:
            print(f"{colors[5]}Welcome back!{end_code}")
        else:
            print(f"{colors[1]}Invalid username or password. Refresh to try again!")
            exit()
        index = 0

    #2.Register
    if account == 2:
        print(f"{colors[3]}2.Register{end_code}")
        user = input(f"{colors[2]}New username:")
        password = input(f"{colors[2]}New password:")
        new_user = register(user, password)
        print(f"{colors[5]}Welcome!{end_code}")
        index = 0
        create_file = open(f"{user}", "x")
```

## Initaial Balance Flow chart 2
My client Ms Sato, requires a system that allows her to input her initial balance of Binance, in order to tract her future transactions and overall valance in a more organized and factual way. To make this possible I created a request for the user to input their initial balance into a file. This program runs right after and only if the user register for the first time, this way I avoided creating unecessary data that I would later have to delete from the file. The instructions for the format in which Ms Sato must input her initial balance is really crlear due to the use fo color and direct instructions. The file in which the balance is added is formated like a spread shit so that keepink track with the users balance is visually easier to use.
```.py
#Initial value
if account == 2:
    steps_msg = "We are happy to have you. Lets start to set up your account".center(50)
    print(f"{colors[6]}{steps_msg}{end_code}")
    print(f"{colors[4]} Set up initial BNB balance balance: (ex. 56776 BNB){end_code}")
    with open(f"{user}"r"") as file:
        balance = input()
        new_balance = initial_balance(balance)
        print(f"{colors[6]}Thank you! Now you can start using your binance crypto wallet :D{end_code}")
        index = 0
```

## Record Transactions Flow chart 1
My client Ms Sato, requires a system that where she can record the transactions she makes with ther bianance cryptocurrency, in an organized and clear matter. To make this possible I created a function that allow Ms Sato to append her transactions to a file in the form of a spreadseet that is devided by category, amount, date and a short description of the transaction. This program runs after the home menu if the user inputs 2. tFor this section of the code to function, I had to create a function in side my project_library which is a separate python file inside the same project. I imported the function so that I could use it in my program with the inputs inputs from Ms Sato.
```.py
#2. Record transaction
if functions == 2:
    print(f"{colors[5]}1. Record transaction{end_code}")
    category= input(f"{colors[6]}Select the category of the transaction: |food|Expenses|Transportation|Healthcare|Education|Personal| ->")
    ammount= input(f"Insert the ammount of the transaction: (ex. 26473 BNB) -> ")
    date= input(f"Insert the date the transaction was made: (YYYY/MM/DD) -> ")
    description = input(f"Write a short description of the transaction: ->{end_code}")
    new_transaction= transactions(category, ammount, date, description)
    index = 0
```
