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
![OIP](https://user-images.githubusercontent.com/117569921/200165775-5e0ed8b3-fa27-42f2-9559-4cef266a69cd.jpg)
