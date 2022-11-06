# Fibonacci 1
```py
times_executed = 0
def fib(n):
    global times_executed
    times_executed = times_executed + 1
    if n < 0:
        return False
    elif n == 0:
        return 1
    elif n > 0:
        return fib(n - 1) + fib(n - 2)
    else:
        return False
```

![pobierz (1)](https://user-images.githubusercontent.com/117569921/200168266-83a43a45-1c03-4a68-87bb-b516401d44b2.png)



# Fibonacci 2
```py
def fib2(n):
    i = 0
    a = 1
    b = 1
    fibs = []
    while(i <= n // 2):
        i = i + 1
        fibs.append(a)
        fibs.append(b)
        a = a + b
        b = a + b
    return fibs
```

![pobierz](https://user-images.githubusercontent.com/117569921/200168256-280e3249-1c65-4cf9-a4db-c774c6cd0deb.png)

