```.py
def cypher(message, shift):
	result = ""

	for i in range(len(message)):
		char = message[i]

		# ASCCI alphabet 97-122
		if (char.isalpha()):
			result += chr(ord(char) + shift)
	return result


# Test 1 SL
message = "hello world"
shift = 13
print("Shift by how much: " + str(shift))
print("Enter your message: " + message)
print("This is your cypher:" + cypher(message, shift))

print("°"*50)
# Test 1 HL
print("HL Code")
message = "hello world"
shift = int(input("Enter your shift:"))
print("Shift by how much: " + str(shift))
print("Enter your message: " + message)
print("This is your cypher:" + cypher(message, shift))
```

<img width="1416" alt="Screen Shot 2022-10-08 at 14 46 02" src="https://user-images.githubusercontent.com/111941990/194691207-74bb362c-5f1c-4312-b073-21da40cfd6e6.png">
<img width="408" alt="Screen Shot 2022-10-08 at 15 48 09" src="https://user-images.githubusercontent.com/111941990/194694089-aab1d7d5-b47b-47c2-8d18-a059cab6fac4.png">


