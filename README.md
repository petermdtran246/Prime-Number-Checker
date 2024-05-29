# Prime Number Checker
This Python program checks if a given number is a prime number.

### Algorithm
The algorithm follows these steps:

1. Function Definition: The code defines a function prime_checker that takes a single integer argument number. This function determines whether the input number is prime.

2. Prime Flag Initialization: Inside the function, a variable is_prime is initialized to True. This flag will be used to track whether the current number is a candidate for being prime throughout the loop.

3. Loop for Divisibility Check: A for loop iterates through potential divisors of the number. The loop starts at 2 (since 1 divides every number) and continues up to number - 1 (excluding the number itself and 0 for efficiency).

  -  Inside the loop, the code checks if the current divisor i divides evenly into the number using the modulo operator (%). If it does (number % i == 0), it means the number is divisible by another number besides 1 and itself, disqualifying it from being prime.
  -  If the number is divisible, the is_prime flag is set to False. Since we've found a divisor (other than 1 and itself), we can exit the loop early using a break statement (optional for efficiency).

4. Prime Number Determination:

After the loop completes (either by iterating through all divisors or finding a divisor), the value of the is_prime flag determines the output:
  -  If is_prime is still True, it means no divisors were found in the loop, and the number is prime.
  -  If is_prime is False, it means a divisor was found, and the number is not prime.

5. Output: Based on the is_prime flag, the function prints a message indicating whether the input number is prime or not.

6. User Input and Function Call:

  -  Outside the function, the program prompts the user to enter a number.
  -  The user's input is converted to an integer using int(input()).
  -  The prime_checker function is called, passing the user's input number as a keyword argument (number=n).

