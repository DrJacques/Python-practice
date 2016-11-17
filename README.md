# Python-practice
# is_int
# An integer is just a number without a decimal part (for instance, -17, 0, and 42 are all integers, but 98.6 is not).

# For the purpose of this lesson, we'll also say that a number with a decimal part that is all 0s is also an integer, such as 7.0.

# This means that, for this lesson, you can't just test the input to see if it's of type int.

# If the difference between a number and that same number rounded down is greater than zero, what does that say about that particular number?

# Instructions
# Define a function is_int that takes a number x as an input.
# Have it return True if the number is an integer (as defined above) and False otherwise.
# For example:

# is_int(7.0)   # True
# is_int(7.5)   # False
# is_int(-1)    # True 
#Below is my code

def is_int(x):
    if abs(x-round(x))>0:
        return False
    else:
        return True
#Write a function called digit_sum that takes a positive integer n as input and returns the sum of all that number's digits.

#For example: digit_sum(1234) should return 10 which is 1 + 2 + 3 + 4.

#(Assume that the number you are given will always be positive.)

#Check the hint if you need help!
#Below is my code

def digit_sum(n):
    n = str(n)
    sum=0
    for i in n:
        i = int(i)
        sum=sum+i
    return sum
