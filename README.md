# calculator
def add(a, b):
    return a+b


def substract(a, b):
    return a-b


def multiply(a, b):
    return a*b


def divide(a, b):
    if b == 0:
        return "can not divide by zero"
    else:
        return a/b


while True:
    print("\n simple CLI calculator ")
    print("1. addition")
    print("2. substraction")
    print("3. multiplication")
    print("4. division")
    print("5. exit")
    choice = input("enter your choicefrom(1-5):")
    if choice == '5':
        print("see you next time")
        break
    num1 = float(input("enter first number:"))
    num2 = float(input("enter second number:"))
    if choice == '1':
        print("result:", add(num1, num2))
    elif choice == '2':
        print("result:", substract(num1, num2))
    elif choice == '3':
        print("result:", multiply(num1, num2))
    elif choice == '4':
        print("result", divide(num1, num2))
    else:
        print("invalid choice,try again!")

