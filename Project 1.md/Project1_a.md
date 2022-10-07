# Crypto Wallet

![200w](https://user-images.githubusercontent.com/111941990/191906556-dc599fb6-4c12-4790-885e-e96b16a3bfd4.gif)


# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

An examle of the data store is date, despcription, category and ammount
| Date | Description | Category | Amount |
|------|-------------|----------|--------|--------
|Sep 23 2022 | bought a house | Expenses | 10 BTC |
|Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |
## Proposed Solution

Design statement:
I will design and make an electronic ledger for a client who is a local trader, looking for a way to organize and keep track of her transactions. The ——– will about ———— and is constructed using the software pycharm. It will take  ———- to make and will be evaluated according to the criteria ———.

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
# Log-in and Register system Flow chart 3
```.py
#Log-in screen for Sato
from my_lib import register, end_code, colors, bold_white, validate_int_input, transactions, initial_balance, current_balance
from Password import login

welcome_msg = "Welcome to your crypto wallet".center(50, "=")
prompt_msg = "Log-in if you have an account or register to create a new one [1-2]"

print(f"{colors[2]}{welcome_msg}{end_code}")
print("Log-in if you have an account or register to create a new one".center(50))

account= """
1. log-in
2. register
"""
print(account)
option = validate_int_input(prompt_msg)
while option>2 or option < 1:
    option = validate_int_input(f"{colors[1]}Invalid option.{prompt_msg}{end_code}")

#1: log-in and registration
with open("db.csv", "r") as file:
    Passwordtwo= file.readlines()

if option ==1:
    print(f"{bold_white}1.Log-in{end_code}")
    user= input("Enter you username:")
    password= input("Enter your password:")
    existing_user= login(user, password)
    if existing_user:
        print("Welcome back!")
    else:
        print(f"{colors[1]}Invalid username or password. You'll be sent to the welcome page, please try again!{end_code}")
        exit()
    index = 0

if option ==2:
    print(f"{bold_white}2.Register{end_code}")
    user= input("New Username:")
    password = input("New password:")
    new_user= register(user, password)
    print("Welcome!")
    index = 0
```

![Project_ log-in and register system flowchart](https://user-images.githubusercontent.com/111941990/194450705-f3b3dd76-4ac0-4b81-b994-f044984c4e62.png)

# Initaial Balance Flow chart 2
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
![2nd flowchart](https://user-images.githubusercontent.com/111941990/194595598-4cb6301b-e401-4c7d-8379-2bbed89380cb.jpg)


# Record Transactions Flow chart 1
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

![3rd Flow chart](https://user-images.githubusercontent.com/111941990/194599362-5e8e4f82-4e5d-4c78-b0d4-e584e8fd97c2.jpg)














## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                                         | To have a clear idea of the hardware and software requirements for the proposed solution                        | 10min         | Sep 24                 | B         |

