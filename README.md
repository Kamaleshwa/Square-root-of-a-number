# Find the square root of a number

## AIM:
To write a program to find the square root of a number.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define a function.
2. Assign number_iters = 100 in the function to perform 100 iteratios.
3. Set i = 0.
4. Calculate  number = 0.5 * (number + a / number) for 100 iterations.
5. Return number

## Program:
#Program to find the square root for the given number(newton's method) using function.
#Developed by: kamaleshwar.kv
#RegisterNumber: 212223240063 
def square_root(number):
    # Initial guess for the square root
    guess = number / 2
    # Set a tolerance level for convergence
    tolerance = 0.000001

    while True:
        # Calculate the new guess using Newton's method
        new_guess = 0.5 * (guess + number / guess)
        
        # Check if the absolute difference between the new guess and the old guess is within tolerance
        if abs(new_guess - guess) < tolerance:
            break
        
        # Update the guess for the next iteration
        guess = new_guess

    return new_guess


number = float(input())
if number < 0:
    print("Square root is not defined for negative numbers.")
else:
    print("Square root of the number:" , square_root(number))

## Output:
![image](https://github.com/Kamaleshwa/Square-root-of-a-number/assets/144980199/9f176858-814b-4d4f-8650-98775bea5278)




## Result:
Thus the program to find the square root for the given number(newton's method) using function is written and verified using python programming.
