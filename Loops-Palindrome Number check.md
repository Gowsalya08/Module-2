## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
def is_palindrome(number):
    original_number = number
    reversed_number = 0
    while number > 0:
        digit = number % 10
        reversed_number = reversed_number *10 +digit
        number = number //10
    return original_number == reversed_number
num = int(input())
if is_palindrome(num):
    print("The given number", num, "is a Palindrome")
else:
    print("The given number", num, "is not a palindrome")
## Output
<img width="1151" height="222" alt="image" src="https://github.com/user-attachments/assets/c1af769e-2261-46b2-a4b7-eef64138488c" />


## Result
Thus the Python program that checks whether a given number is a **palindrome** using loops was successfully completed
