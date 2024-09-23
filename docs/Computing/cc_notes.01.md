# Bugs in code

compiler(code) -> machine code

(\x.x)y -> y

```config
y=23
```

```py
# file.py
def y():
    return read_config("y")

def multiply_by3(x: int) -> int:
    """mutiply by 3"""""
    return y()*3

def funk():
    return random_choose(2, "3")

def add_2(x: int) -> int:
    return x + 2

#############

from file import func

funk(3) # 6
funk()
func(3) # 12

add_2(multiply_by3(3))
add_2(random_choose())
```


```
f(x), state -> y

```


1. config files
2. version
3. dependencies

```
a: deps@3.12
    - lib@4.2
b: pack@3.02 
    - lib@3.9

install y@2.9
```
