### NAME: RANJANI K

### REG NO.: 212224230220

# Experiment-4
## ARMSTRONG NUMBER 
# Aim: Write a python program to check the number is Armstrong number or not and inspect for failures. 

# Algorithm
1.	Start the program.
2. Read an integer input number.
3. Initialize the variables current_digit, sum = 0, and num = number.
4. Repeat Steps 5 to 7 until num > 0
5. current_digit = (num % 10).
6. sum = sum + (current_digit * current_digit * current_digit). 7. Stop the program.
7. num = num / 10.
8. Check if sum == number. If true, print "It is an Armstrong Number." Otherwise, print "It is not an Armstrong Number."
9. Stop the program. 

# Program
```
def is_armstrong(n):
    if not isinstance(n, int):
        raise TypeError("Input must be an integer.")
    if n < 0:
        return False
    digits = str(n)
    power = len(digits)
    total = sum(int(d)**power for d in digits)
    return total == n


try:
    num = int(input("Enter a number: "))
    if is_armstrong(num):
        print(f"{num} is an Armstrong number.")
    else:
        print(f"{num} is not an Armstrong number.")

except ValueError:
    print("Input Error: Please enter a valid integer.")
except Exception as e:
    print("Unexpected Error:", e)
```
# Output
<img width="742" height="60" alt="image" src="https://github.com/user-attachments/assets/91f79a8f-6d2a-49be-802b-2ecb1b813493" />
<img width="745" height="76" alt="Screenshot 2025-08-30 104231" src="https://github.com/user-attachments/assets/65ef018e-c528-40e6-9c7b-0726733223ef" />

# Result
Thus, the python program to check the number is Armstrong number or not implemented and the output is verified successfully.
