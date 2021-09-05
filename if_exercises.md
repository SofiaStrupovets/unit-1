# Solutions for if exercises in Snakify

## 1.Minimum of 2 numbers
![](minof2numbers.jpg)

```.py
a = int(input('Enter value 1 '))
b = int(input('Enter value 2 '))

if a>b:
    print (b)
else:
    print (a)

```

## 2.Sign function
![](sign.jpg)

```.py
a = int(input('Enter value '))

if a>0:
    print(1)
elif a<0:
    print(-1)
else:
    print(0)

```

## 3. Minimum of 3 numbers
![](minof3numbers.jpg)

```.py
a = int(input('Enter value 1 '))
b = int(input('Enter value 2 '))
c = int(input('Enter value 3 '))

if a>b:
    if b>c:# if a>b>c
        print(c)
    else: #if a>c>b
        print(b)
elif b>a:
    if a>c: #if b>a>c
        print(c)
    else: #if b>c>a
        print(a)
        
```

## 4.Equal numbers
![](equal.jpg)

```.py
a = int(input('Enter integer 1 '))
b = int(input('Enter integer 2 '))
c = int(input('Enter integer 3 '))

if a==b==c:
    print(3)
elif a==b!=c or a==c!=b or c==b!=a:
    print(2)
else:
    print(0)
    
```

## 5.Rook move
![](rook.jpg)

```.py
a = int(input('Enter original column '))
b = int(input('Enter original row '))
c = int(input('Enter final column '))
d = int(input('Enter final row'))

if a>c or a<c:
    if b==d:
        print('YES')
    else:
        print('NO')
elif b>d or b<d:
    if a==c:
        print('YES')
    else:
        print('NO')
else:
    print('NO')
        
```

## 6.Chess board
![](chess.jpg)

```.py
a = int(input('Enter column 1'))
b = int(input('Enter row 1'))
c = int(input('Enter column 2'))
d = int(input('Enter row  2'))

if (a+b)%2==(c+d)%2:
    print('YES')
else:
    print('NO')

```

## 7.King move
![](king.jpg)

```.py
a1 = int(input('Enter original column '))
b1 = int(input('Enter original row '))
a2 = int(input('Enter final column '))
b2 = int(input('Enter final row'))

if a1+1==a2 or a1-1==a2 or a1==a2:
    if b1+1==b2 or b1-1==b2 or b1==b2:
        print('YES')
    else:
        print('NO')
else:
    print('NO')
    
```

## 8.Bishop moves
![](bishop.jpg)

```.py
a1 = int(input('Enter original column '))
b1 = int(input('Enter original row '))
a2 = int(input('Enter final column '))
b2 = int(input('Enter final row'))

if (a1-a2)==(b1-b2) or (a1+b1)==(a2+b2):
    print ('YES')
else:
    print('NO')
    
```

## 9.Queen move
![](queen.jpg)

```.py
a1 = int(input('Enter original column '))
b1 = int(input('Enter original row '))
a2 = int(input('Enter final column '))
b2 = int(input('Enter final row'))

if a1==a2 or b1==b2:
    print('YES')
elif (a1-a2)==(b1-b2) or (a1+b1)==(a2+b2):
    print ('YES')
else:
    print('NO')
    
```

## 10.Knight move
![](knight.jpg)

```.py
a1 = int(input('Enter original column '))
b1 = int(input('Enter original row '))
a2 = int(input('Enter final column '))
b2 = int(input('Enter final row'))

if a1+2==a2 or a1-2==a2:
    if b1+1==b2 or b1-1==b2:
        print('YES')
    else:
        print('NO')
else:
    if b1+2==b2 or b1-2==b2:
        if a1+1==a2 or a1-1==a2:
            print('YES')
        else:
            print('NO')
    else:
        print('NO')
        
```

## 11.Chocolate bar
![](chocolate.jpg)

```.py
n = int(input())
m = int(input())
k = int(input())

if (n*m)>k:
    if (k%m==0) or (k%n==0)
        print('YES')
    else:
        print('NO')
else:
    print('NO')
```

## 12.Leap year
![](leap.jpg)

```.py
a = int(input('Enter year'))
if (a)%4==0 and (a)%100!=0:
    print('LEAP')
elif (a)%400==0:
    print('LEAP')
else:
    print('COMMON')
    
```
