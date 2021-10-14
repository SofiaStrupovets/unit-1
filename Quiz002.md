Given three integer values, A, B, and C, output the largest difference between any of the numbers.

```.py

def difference(a,b,c):
    if a>b>c:
        print(a-c)
    if a>c>b:
        print(a-b)
    if b>a>c:
        print(b-c)
    if b>c>a:
        print(b-a)
    if c>b>a:
        print(c-a)
    if c>a>b:
        print(c-b)
        
print (difference(3,2,4))

```
