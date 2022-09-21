```.py
#Sl
room= int(input("Insert a number room:"))

if room < 100:
    floor = room // 10
    room_f = (room //10)+1
    print(f"{room}-Room {floor}F{room_f}")

    if room % 10 == 0:
        floor = room // 10
        room_f = (room //10)
        print(f"{room}-Room {floor}F{room_f}")

#Hl
print("Room fromt with define input:")
hl= 100
floor = hl // 10
room_f = (hl //10)
print(f"{hl}-Room {floor}F{room_f}")
```


<img width="1399" alt="Screen Shot 2022-09-19 at 21 42 53" src="https://user-images.githubusercontent.com/111941990/191020810-9f9b6efd-e706-4a9e-be57-f0b733e616dc.png">
