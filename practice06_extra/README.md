# Практическое занятие 6

## Содержание

- [Задача 1](#задача-1)
- [Задача 2](#задача-2)
- [Задача 3](#задача-3)
- [Задача 4](#задача-4)
- [Задача 5](#задача-5)
- [Задача 6](#задача-6)

### Задача 1

Напишите функцию deriv для приближенного вычисления производной в заданной
точке.

#### Решение

```bigquery
def deriv(func):
    x = sy.Symbol('x')

    def take(x):
        return sy.diff(func(x), x)

    def substitution(dig):
        return take(x).subs(x, dig)

    return substitution
```

#### Демо

```bigquery
>>> deriv(lambda x: x ** 3)(5)
75.00014999664018
```

### Задача 2

Создайте вариант именованного кортежа с помощью ФВП.

#### Решение



#### Демо