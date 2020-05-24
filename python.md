## What are the method(s) an iterator object must implement?
- [ ] __iter__()
- [x] __iter__(), __next__()
- [ ] __iter__(), __super__()
- [ ] __iter__(), __super__(), __next__()

## How can you create an iterator object from a list?
- [x] By passing the given list to the iter() function
- [ ] By using a for loop
- [ ] By using a while loop
- [ ] You cannot create an iterable object from the list

## If a function contains at least one yield statement, it becomes ...
- [ ] An iterable
- [x] A generator function
- [ ] An anonymous function
- [ ] None of the above

## What is the output of the following piece of code?
```python
my_list = [1, 3, 6, 10]
a = (x**2 for x in my_list)
print(next(a), next(a))
```
- [ ] 1 3
- [x] 1 9
- [ ] 1 9 36 100
- [ ] 1

## What criteria must be met to create a Python closure?
- [ ] Program must have a function inside another function
- [ ] A nested function must refer to a value defined in the enclosing function
- [ ] An enclosing function must return a nested function
- [x] All of the above

## What is the output of the following piece of code?
```python
def Foo(n):
    def multiplier(x):
        return x * n
    return multiplier

a = Foo(5)
b = Foo(5)

print(a(b(2)))
```
- [ ] 25
- [ ] 100
- [ ] 10
- [x] 50

## What is the output of the following piece of code?
```python
def make_pretty(func):
    def inner():
        print("I got decorated")
        func()
    return inner

def ordinary():
    print("I am ordinary")

pretty = make_pretty(ordinary)
pretty()
```
- [ ] I got decorated
- [ ] I am ordinary
- [x] I got decorated /n I am ordinary
- [ ] I am ordinary /n I got decorated

## Which of the following statements is true?
- [ ] You cannot chain multiple decorators in Python
- [ ] Decorators don't work with functions that take parameters
- [ ] The @ symbol doesn't have any use while using decorators
- [x] None of the above

## What is the more pythonic way to use getters and setters?
- [ ] Decorators
- [ ] Generators
- [ ] Iterators
- [x] @property

## In Python, there is a built-in function property() that returns a property object. Which of the following methods does the property object has?
- [ ] getter(), setter()
- [x] getter(), setter(), delete()
- [ ] getter(), delete()
- [ ] setter(), delete()

## What are the most common functional programming methods that use lambda functions? (Select all that apply)
- [x] map()
- [x] filter()
- [ ] lookup()
- [x] reduce()

## Which type of concurrency is best for CPU-bound programs?
- [ ] Asyncio
- [ ] Threading
- [ ] Dictionaries
- [x] Multiprocessing

## You have an I/O-bound program that takes about 2 seconds to run and that only gets run once a week. Which concurrency library should you use?
- [ ] Threading
- [x] You should not use concurrency
- [ ] Multiprocessing
- [ ] Asyncio

## Which of the following are true for objects of Python's set type?
- [ ] May contain elements that are mutable
- [ ] Elements' order is significant
- [x] A given element can't appear more than once
- [x] Are mutable

## Which of the following functions are spelled correctly?
```python
def func1(name="Willy": str): -> str
    return "No hay problema {}".format(name)

def func2(name:str = "Willy") -> str:
    return "No hay problema {}".format(name)

def func3(name="Willy": str) -> str:
    return "No hay problema {}".format(name)

def func4(name:str = "Willy"): -> str
    return "No hay problema {}".format(name)
```
- [ ] func1
- [x] func2
- [ ] func3
- [ ] func4
- [ ] None of the above
