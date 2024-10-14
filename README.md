# fawzeiaNasr
git https://github.com/Mosabyousif/GithubFirstDay.git
git chekout -b caculator-feature
touch calculator.py
# calculator.py
def add(x, y):
    return x+ y
def subtract(x, y):
    return x- y
def multiply (x, y):
    return x* y
def divide(x, y):
     if y != 0:
        return x/ y
     else:
          return "can not divide by 0!"
def calculator():
     print("select operation: ")
     print("1. Add")
     print("2. subtract")
     print("3. multiply")
     print("4. divide")

     choice = input("enter choice(1/2/3/4): ")
     num1 = float(input("Enter frist number:"))
     num2 = float(input("Enter second number:")) 
     if choice == '1':
        print(f"{num1} + {num2} = {add(num1, num2)}")
    elif choice == '2':
        print(f"{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == '3':
        print(f"{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == '4':
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    else:
        print("Invalid input")

if __name__ == "__main__":
    calculator()
git add calculator.py
git commit -m "add calculator program"
git push origin calculator-feature


    
