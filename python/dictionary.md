# Python Dictionaries

## View

This is what a python dictionary looks like.


```python
my_dict = {
    "a": "aa",
    "b": "bb"
}
```

## Read a dictionary

To read a python dictionary, use the following methods:

```python
my_dict = {
    "a": "aa",
    "b": "bb"
}
my_dict["a"]
# output: 'aa'
my_dict.b
# output: 'bb'
my_dict.get("a")
# output: 'aa'
my_dict.get("c")
# output:
my_dict.keys()
# output: dict_keys(['a', 'b'])
my_dict.values()
# output: dict_values(['aa', 'bb'])
my_dict.items()
# outpur: dict_items([('a', 'aa'), ('b', 'bb')])
if "a" in my_dict:
    print("Yes")
# output: Yes
```

## Add and update python dictionary

To add or update python dictionaries, use the following methods.

```python
my_dict.update({"c": "cc"})
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
```

## Remove items from python dictionary


To remove python dictionaries, use the following methods.

```python
my_dict.pop('c')
my_dict
# output: {'a': 'aa', 'b': 'bb'}

my_dict.update({"c": "cc"})
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
my_dict.pop('c')
my_dict
# output: {'a': 'aa', 'b': 'bb'}

del my_dict["c"]
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
my_dict.pop('c')
my_dict
# output: {'a': 'aa', 'b': 'bb'}

my_dict.clear()
my_dict
# output: {}
```

## Loop a python dictionary

To loop through a python dictionaries, use the following methods.

```python
for x in my_dict:
    print(x)
# output: a
#         b

for x in my_dict:
    print(my_dict[x])
# output: aa
#         bb

for x in thisdict.values():
    print(x)
# output: aa
#         bb

for x in thisdict.keys():
    print(x)
# output: a
#         b

for x, y in my_dict.items():
    print(x, y)
# output a aa
#        b bb
```

## Copy a python dictionary

To copy a python dictionaries, use the following methods.

```python
my_dict
# output: {'a': 'aa', 'b': 'bb'}
mirror_dict = my_dict
mirror_dict["c"] = "cc"
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
mirror_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
coppied_dict = my_dict.copy()
coppied_dict["d"] = "dd"
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
coppied_dict
# output: {'a': 'aa', 'b': 'bb', 'd': 'dd'}
coppied_dict_1 = dict(my_dict)
coppied_dict_1["d"] = "dd"
my_dict
# output: {'a': 'aa', 'b': 'bb', 'c': 'cc'}
coppied_dict_1
# output: {'a': 'aa', 'b': 'bb', 'd': 'dd'}
```
