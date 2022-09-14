# Python functions

## A simple python function

```python
def my_function():
    print("hello")

# output: hello
```

## A function with some args

```python
def my_arg_function(firstname: str, lastname: str):
    print(f'My fullname is {firstname} {lastname}')

my_arg_function("John", "Doe")
# output: My fullname is John Doe
```

## A return function

```python
def my_arg_function(firstname: str, lastname: str):
    return firstname + " " + lastname

fullname = my_arg_function("John", "Doe")
print(f'My fullname is {fullname}')
# output: My fullname is John Doe
```

## A function with unknown no of args

```python
def my_unknown_args_function(*args):
    print(args)
my_unknown_args_function(1, 2, 3, 4, 5, "Hello")
# output: (1, 2, 3, 4, 5, "Hello")
```

## A empty function

An empty function must have a ```pass``` keyword

```python
def my_empty_function():
    pass
```

## A function with arbitary keyword arguments

Arbitary keywords are the keywords that are passed by declaring while passing arguments.

```python
def my_function(**names):
    print("His full name is " + " " + names["firstname"] + " " + names["lastname"])
my_function(firstname = "John", lastname = "Doe")
```
