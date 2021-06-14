---
title: Lists, Tuples, Sets, Dictionaries
layout: post
author: Lists, Tuples, Sets, Dictionaries
author: coder-lg
excerpt_seperator: "<!--more-->"
---

* TOC
{:toc}

# Lists, Tuples, Sets, Dictionaries


### Listing


```python
list_01=['Jupyter',2,3,4,5,'conda']
print(list_01)
print(list_01[0])
print(list_01[1])
print(list_01[2])
print(list_01[3])
print(list_01[4])
print(list_01[5])
print(len(list_01))
list_01.pop(1)
print(list_01)
list_01.append('to the back')
print(list_01)
```

    ['Jupyter', 2, 3, 4, 5, 'conda']
    Jupyter
    2
    3
    4
    5
    conda
    6
    ['Jupyter', 3, 4, 5, 'conda']
    ['Jupyter', 3, 4, 5, 'conda', 'to the back']


### Making a new list by using the same old list name with [1]


```python
list_01[1]=[1,2,3,4,5,6,7,8]
print(list_01)
print(list_01[1])
print(list_01[1][5])
```

    ['Jupyter', [1, 2, 3, 4, 5, 6, 7, 8], 4, 5, 'conda', 'to the back']
    [1, 2, 3, 4, 5, 6, 7, 8]
    6


### Duplicating and renaming a number/name in a list


```python
list2=list_01
print(list2)
list2[4]='condareddy'
print(list_01)
list2[4]='conda'
print(list_01)
```

    ['Jupyter', [1, 2, 3, 4, 5, 6], 4, 5, 'conda', 'to the back']
    ['Jupyter', [1, 2, 3, 4, 5, 6], 4, 5, 'condareddy', 'to the back']
    ['Jupyter', [1, 2, 3, 4, 5, 6], 4, 5, 'conda', 'to the back']


### Print


```python
print(list_01)
```

    ['Jupyter', [1, 2, 3, 4, 5, 6], 4, 5, 'conda', 'to the back']


### Copying and renaming a component in a list


```python
list3=list_01.copy()
print(list3)
list3[1]='EZ'
print(list3)
```

    ['Jupyter', [1, 2, 3, 4, 5, 6], 4, 5, 'conda', 'to the back']
    ['Jupyter', 'EZ', 4, 5, 'conda', 'to the back']


### Tuples


```python
dummies_tuple=(1212,4332,3523.5,24432)
print(dummies_tuple)
print(dummies_tuple[1])
print(len(dummies_tuple))
dummy = list(dummies_tuple)
dummy[0]=12
print(dummy)
dummies_tuple = tuple(dummy)
print(dummies_tuple)
```

    (1212, 4332, 3523.5, 24432)
    4332
    4
    [12, 4332, 3523.5, 24432]
    (12, 4332, 3523.5, 24432)


### Sets


```python
new_set={1213,12434,'water','genius'}
print(new_set)
print('water' in new_set)
print('dummy' in new_set)
new_set.add(72)
print(new_set)
new_set.remove('water')
print(new_set)
```

    {12434, 'water', 1213, 'genius'}
    True
    False
    {'water', 72, 12434, 'genius', 1213}
    {72, 12434, 'genius', 1213}


### Dictionaries


```python
simple_dict={
        "brand": "Apple",
        "product": "iPhone",
        "model": "12"
}
print(simple_dict)
print('I bought an',simple_dict['product'],simple_dict['model'],'from the',simple_dict['brand'],'store')
```

    {'brand': 'Apple', 'product': 'iPhone', 'model': '12'}
    I bought an iPhone 12 from the Apple store


### Renaming a component in a dictionary


```python
simple_dict["model"]="12 Pro Max"
print('I bought an',simple_dict['product'],simple_dict['model'],'from the',simple_dict['brand'],'store')
```

    I bought an iPhone 12 Pro Max from the Apple store


### Adding a component in a dictionary


```python
simple_dict["color"]="red"
print('I bought an',simple_dict['color'],simple_dict['product'],simple_dict['model'],'from the',simple_dict['brand'],'store')
```

    I bought an red iPhone 12 Pro Max from the Apple store


### Creating and taking specific components
#ie: 0,a,b,c,d,e,f
```
print(simple_list[a:c])
```
Components from a to c will be printed

#### getting from integers:
```python
simple_list=[1,2,3,4,5,6,7,8,9,10]
print(simple_list)
print(simple_list[2:5])
print(simple_list[1:6])
print(simple_list[-3:-1])
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    [3, 4, 5]
    [2, 3, 4, 5, 6]
    [8, 9]
