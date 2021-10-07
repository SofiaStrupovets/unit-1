Given a number as a String N. Multiply all of its digits, and repeat the same with the product obtained till the product consists of only one digit. 
Output the number of steps taken to do so.

```.py

def get_digits(num, digits=[]):
    while num > 0:
        digits.append(num % 10)
        return get_digits(num // 10, digits)
    if num == 0:
        return digits


def multiply_all(digits, multiplier=1):
    while len(digits) > 0:
        multiplier = multiplier * digits.pop(0)
        return multiply_all(digits, multiplier)
    if len(digits) == 0:
        return multiplier


def persistence(num, count=0):
    while num >= 10:
        num = multiply_all(get_digits(num))
        count += 1
        return persistence(num, count)
    if num < 10:
        return count
        
print(persistence(39))

```

I will be honest, I spent ages on this task and still was not able to figure out how to it, so I found this solution.
What I did, was the program that made step1(multiplied digits first time), and tried to use one more cycle to make it multiplying digits until one digit is left.
But that is the program which I ended up with. It broke all the time when I tried to add next steps and I have no idea how to improce it:

```.py
def Product(n):
    product = 1
    while n!=0:
        product = product * (n % 10)
        n = n // 10
    
    return product
print (Product(39))
```
