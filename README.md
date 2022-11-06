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

![stretched-2560-1440-742529](https://user-images.githubusercontent.com/117569921/200168216-0ab3d2f5-821c-458c-918d-38da1ae96cdc.png)


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

![stretched-2560-1440-742529](https://user-images.githubusercontent.com/117569921/200167993-249acaf2-79ee-4f97-806c-602a351b5a64.png)
