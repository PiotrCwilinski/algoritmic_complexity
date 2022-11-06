# Fibonacci 1 (Rekurencyjny)
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



# Fibonacci 2 (Iteracyjny)
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


![pobierz (3)](https://user-images.githubusercontent.com/117569921/200168964-7fec88a5-72c8-40f1-9da7-80ca487dedb3.png)



# Porównanie Fibonacci 1 i Fibonacci 2

Wykres przedstawia zależność czasu od liczby Fibonacciego.
Kolor pomarańczowy przedstawia funkcję przy użyciu Fibonacciego 1.
Kolor niebieski przedstawia funkcję przy użyciu Fibonacciego 2
Jak widać na wykresie Fibonacci 2 jest znacznie lepiej zoptymalizowanym kodem.

![pobierz (2)](https://user-images.githubusercontent.com/117569921/200168319-ad1cc62b-24f4-4e27-b00a-3158bf84e545.png)


# Piesek dla uwagi
Piesek używający Fibonacciego 1


![image](https://user-images.githubusercontent.com/117569921/200168638-f777b2ad-4a50-4dd6-8b12-c17277439674.png)


Piesek używający Fibonacciego 2


![image](https://user-images.githubusercontent.com/117569921/200168789-138300d6-49c8-4716-a4eb-67352b65b367.png)
