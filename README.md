from math import *
password_value = ('Mathsolver')
input_password = ''
password_attempt = 1
is_password_lock = False

while is_password_lock == False and password_attempt < 4:
        if password_attempt <= 3:
            input_password = input('Enter Password:')

        if input_password == password_value:
            is_password_lock = True
        else:
            password_attempt = password_attempt + 1
            if password_attempt < 4:
                print("Incorrect password, try again")

if is_password_lock != True:
    print("Please ask insert name for the correct password and rerun the calculator")
    exit(-1)

instructionString = 'Enter the letter for the command\n Add(A), Subtract(S), Multiply(M), Division(D),\n Square root(R), Power(P), Highest(H), Lowest(L), Absolute value(V)'

print(instructionString)
EnteredCommand = input('Enter a command (Q to quit):')

if EnteredCommand.upper()== ('Q'):
        print('Thank you for using (insert Name)\'s calculator')
if EnteredCommand.upper()== ('q'):
        print('Thank you for using (insert Name)\'s calculator')

while (EnteredCommand.upper() != 'Q') :

    if EnteredCommand.upper() == "A":
        print("Addition")
        num1 = input('enter a number:')
        num2 = input('enter another number:')
        resultCommand = float(num1) + float(num2)

    if EnteredCommand.upper() == "S":
        print('Subtraction'.upper())
        num1 = input('enter a number:')
        num2 = input('enter another number:')
        resultCommand = float(num1) - float(num2)

    if EnteredCommand.upper()== "M":
        print('Multiplication'.upper())
        num1 = input('enter a number:')
        num2 = input('enter another number:')
        resultCommand = float(num1) * float(num2)

    if EnteredCommand.upper()== "D":
        print('division'.upper())
        num1 = input('enter a number:')
        num2 = input('enter another number:')
        resultCommand = float(num1) / float(num2)

    if EnteredCommand.upper()== "R":
        print('square root'.upper())
        num1 = input('enter a number:')
        resultCommand = (sqrt(float(num1)))

    if EnteredCommand.upper()== "V":
        num1 = float(input('enter a number:'))
        resultCommand = float(abs(num1))

    if EnteredCommand.upper()== "P":
        print('power'.upper())
        num1 = float(input('enter a number:'))
        num2 = float(input('enter another number:'))
        resultCommand = (pow(num1, num2))

    if EnteredCommand.upper()== "L":
        print('lowest number'.upper())
        num1 = float(input('enter a number:'))
        num2 = float(input('enter another number:'))
        resultCommand = (min(num1, num2))

    if EnteredCommand.upper()== "H":
        print('highest number'.upper())
        num1 = float(input('enter a number:'))
        num2 = float(input('enter another number:'))
        resultCommand = (max(num1, num2))

    print('The answer is')
    print(resultCommand)
    print('')
    print(instructionString)
    EnteredCommand.upper = input('Enter a command (Q to quit):')
    if EnteredCommand.upper()== ('Q'):
        print('Thank you for using Lincoln\'s calculator')


