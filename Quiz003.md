```.py

#Use str
print("Insert protein:")
protein = input()

if protein =="A":
    print("T")

elif protein =="G":
        print("C")

elif protein =="T":
        print("A")

elif protein =="C":
        print("G")

#HL
protein_list = [input()]
for i in range(len(protein_list)):
    if protein_list[i] == 'A':
        protein_list[i] = 'T'

    if protein_list[i] == 'G':
        protein_list[i] = 'C'

    if protein_list[i] == 'C':
        protein_list[i] = 'A'

    if protein_list[i] == 'T':
        protein_list[i] = 'A'

    print(f" proteins:{protein_list}")

```

<img width="1398" alt="Screen Shot 2022-09-15 at 19 23 07" src="https://user-images.githubusercontent.com/111941990/190380273-6946e4e6-8632-42c4-8548-3add77fd68c0.png">

<img width="362" alt="Screen Shot 2022-09-15 at 20 26 39" src="https://user-images.githubusercontent.com/111941990/190392324-f82e0877-a3af-4160-b2c3-87e21e8f6354.png">




