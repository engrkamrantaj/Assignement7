# Assignement # 7 Number Exploration Tool

The code is explained in these steps

### Enter Name of Particiapant and adding three of his fav Numbers


name = input("Enter your name = ")
*n1 = int(input("Enter your first fav number = "))
*n2 = int(input("Enter your second fav number = "))
*n3 = int(input("Enter your third fav number = "))

2.Personalized message with uses name and creating a list to add the numbers

print(f"\nHello {name} lets explore your fav numbers :")
numbers = []
numbers.append(n1)
numbers.append(n2)
numbers.append(n3)

print(numbers)

3. Checking if the number is even or odd

for x in numbers:
    if x % 2 == 0:
        print(f"The number {x} is even")
    else:
        print(f"The number {x} is odd")

for x in numbers:
    sqr = (x, x*x)
    print(f"The number {x} and its square : {sqr}")

n = n1+n2+n3
print(f"Amazing! The sum of your favorite numbers is: {n}")

if n == 2:
    print(f"Wow {n} is a prime number")

elif n <= 0:
    print("Invalid input negative number")
else:
    for a in range(2, n):
        if n % a == 0:
            print(f"Wow {n} is not a prime number")
            break
    else:  # This else will only work when the loop breaks
        print(f"Wow {n} is a prime number")
