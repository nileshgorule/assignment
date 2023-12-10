# Lists


```python

```


```python
#1.Create an empty list.

list = []
print("creating empty list",list)
```

    creating empty list []
    


```python
#2.Add an element to a list.

fruits = ["Apple","banana","cherry","blue berry"]
print(fruits)
fruits.append("rasberry")
print(fruits)


```

    ['Apple', 'banana', 'cherry', 'blue berry']
    ['Apple', 'banana', 'cherry', 'blue berry', 'rasberry']
    


```python
#3.Remove an element from a list.

fruits = ["Apple","banana","cherry","blue berry"]
print(fruits)
fruits.remove("banana")
print(fruits)
```

    ['Apple', 'banana', 'cherry', 'blue berry']
    ['Apple', 'cherry', 'blue berry']
    


```python
#4.Access an element at a specific index in a list.

fruits = ["Apple","banana","cherry","blue berry"]
print(fruits[3])


```

    blue berry
    


```python
#5.Find the length of a list.
fruits = ["Apple","banana","cherry","blue berry"]
print("length of the list :",len(fruits))


```

    length of the list : 4
    


```python
#6.Check if an element exists in a list.

fruits = ["Apple","banana","cherry","blue berry"]
i = "cherry"
if i in fruits:
    print(i,"is exist in",fruits)
else:
    print("not exist")

```

    cherry is exist in ['Apple', 'banana', 'cherry', 'blue berry']
    


```python
#7.Concatenate two lists.

fruit_list1 = ["Apple","banana","cherry","blue berry"]
fruit_list2 = ["pinepple","rasberry","mango","orange"]
fruit_list3 =fruit_list1+fruit_list2
print("fruit_list 1 =",fruit_list1)
print("fruit_list 2 =",fruit_list2)
print("concatenated list =",fruit_list3)
```

    fruit_list 1 = ['Apple', 'banana', 'cherry', 'blue berry']
    fruit_list 2 = ['pinepple', 'rasberry', 'mango', 'orange']
    concatenated list = ['Apple', 'banana', 'cherry', 'blue berry', 'pinepple', 'rasberry', 'mango', 'orange']
    


```python
#8.Find the maximum and minimum elements in a list.

num = [3,5,55,23,87,34]
print("Maximum value from the list is:",max(num))
print("Minimum value from the list is:",min(num))
```

    Maximum value from the list is: 87
    Minimum value from the list is: 3
    


```python
#9.Count the occurrences of a specific element in a list.

fruit_list = ["Apple","banana","cherry","blue berry","cherry"]
res = fruit_list.count("cherry")
print("cherry is present",res,"times in list",fruit_list)
```

    cherry is present 2 times in list ['Apple', 'banana', 'cherry', 'blue berry', 'cherry']
    


```python
#10.Reverse a list.

num = [3,5,55,23,87,34]
print("original list",num)
num.reverse()
print("reversed list",num)

```

    original list [3, 5, 55, 23, 87, 34]
    reversed list [34, 87, 23, 55, 5, 3]
    


```python
#11.Sort a list in ascending order.

num = [3,5,55,23,87,34]
print("original list",num)
num.sort()
print("sorted list",num)


```

    original list [3, 5, 55, 23, 87, 34]
    sorted list [3, 5, 23, 34, 55, 87]
    


```python
#12.Remove duplicates from a list.

num = [2,3,4,2,4,3,6,3,2]
res = []
for i in num:
    if i not in res:
        res.append(i)
        
print(" from list=",num,"\n","after removing duplicate =",res)
```

     from list= [2, 3, 4, 2, 4, 3, 6, 3, 2] 
     after removing duplicate = [2, 3, 4, 6]
    


```python
#13.Extract odd-indexed elements from a list.

num = [1,2,3,4,5,6,7,8,9]
newlist =[]
for i in num:
        if i%2!=0:
            newlist.append(i)
print(newlist)

```

    [1, 3, 5, 7, 9]
    


```python
#14 .Multiply all elements in a list by a specific factor.

num = [1,2,3,4,5]
newlist = [i**2 for i in num]
print(newlist)

```

    [1, 4, 9, 16, 25]
    


```python
#15.Create a new list containing only unique elements from an existing list.
num = [10,30,20,10,30,20,40,50,60,20]
res = []
for i in num:
    if i not in res:
        res.append(i)
print("printing unique values from list and presenting","\n","new list",res)



```

    printing unique values from list and presenting 
     new list [10, 30, 20, 40, 50, 60]
    

# tuples


```python
#16.Create a tuple with three elements.

a = (1,2,3)
print(a)
```

    (1, 2, 3)
    


```python
#17.Access an element from a tuple.
a = (1,2,3)
print(a[1])

```

    2
    


```python
#18.Check if an element exists in a tuple.
a = (1,2,3)
i = 2
if i in a:
    print(i,"is exist in tuple",a)
else:
    print("not exist")

```

    2 is exist in tuple (1, 2, 3)
    


```python
#19.Convert a tuple to a list.

my_tuple = (1,2,3)
print(my_tuple,"this is",type(my_tuple))
my_list=[i for i in my_tuple]
print(my_list,"this is",type(my_list))



```

    (1, 2, 3) this is <class 'tuple'>
    [1, 2, 3] this is <class 'list'>
    


```python
#20.Concatenate two tuples.
a =(1,2,3)
b =(4,5,6)
c = a+b
print(c)
```

    (1, 2, 3, 4, 5, 6)
    


```python
#21.Find the index of a specific element in a tuple.

a =(1,2,3,4,5,6,7,8)
index = a.index(6)
print("index value of 6 is",index)

```

    index value of 6 is 5
    


```python
#22.Unpack the elements of a tuple into separate variables.

fruits = ("Apple","orange","mango")
print(fruits)
(a,b,c) = fruits
print(" after upacking =",a,b,c)

```

    ('Apple', 'orange', 'mango')
     after upacking = Apple orange mango
    


```python
#23.Convert a list into a tuple.

a = ["Apple","Banana","Cherry"]
print(a)
b = tuple(a)
print(b)
```

    ['Apple', 'Banana', 'Cherry']
    ('Apple', 'Banana', 'Cherry')
    


```python
#24.Create a nested tuple.

a = (1,2,3,(4,5,6))
print("creating nested tuple:",a)

```

    creating nested tuple: (1, 2, 3, (4, 5, 6))
    


```python
#25.Swap the values of two variables using tuples.

a = (10,20,30)
b = (60,40,50)
print("Before swapping: a =", a, "b =", b)
a, b = b, a
print("After swapping: a =", a, "b =", b)

```

    Before swapping: a = (10, 20, 30) b = (60, 40, 50)
    After swapping: a = (60, 40, 50) b = (10, 20, 30)
    

# dictionary 


```python
#26 Create an empty dictionary.

dict = {}
print("printing empty dictionary-->",dict)
print(type(dict))
```

    printing empty dictionary--> {}
    <class 'dict'>
    


```python
#27.Add a key-value pair to a dictionary.

dict = {"a":1,"b":2,"c":3,"d":4}
print("adding key-value pairs in the dictionary:",dict)
```

    adding key-value pairs in the dictionary: {'a': 1, 'b': 2, 'c': 3, 'd': 4}
    


```python
#28.Access the value associated with a specific key.

dict = {"a":1,"b":2,"c":3,"d":4}
print(dict)
print([(i,dict[i]) for i in dict])
```

    {'a': 1, 'b': 2, 'c': 3, 'd': 4}
    [('a', 1), ('b', 2), ('c', 3), ('d', 4)]
    


```python
#29.	Check if a key exists in a dictionary.

dictionary = {"a":1,"b":2,"c":3,"d":4}
i = "c"
if i in dictionary:
    print(i,"key exist",dictionary)
else:
    print("not exist")


```

    c key exist {'a': 1, 'b': 2, 'c': 3, 'd': 4}
    


```python
#30.	Remove a key-value pair from a dictionary.

dict = {"aman":23,"ram":54,"raja":45,"neeta":30}
print("before removing key value pair from dictionary",dict)
res = dict.pop("raja")
print("after removing key value pair from dictionary",dict)

```

    before removing key value pair from dictionary {'aman': 23, 'ram': 54, 'raja': 45, 'neeta': 30}
    after removing key value pair from dictionary {'aman': 23, 'ram': 54, 'neeta': 30}
    


```python
#31.	Get all keys from a dictionary.

dict = {"aman":23,"ram":54,"raja":45,"neeta":30}
print(dict)
print(dict.keys())

```

    {'aman': 23, 'ram': 54, 'raja': 45, 'neeta': 30}
    dict_keys(['aman', 'ram', 'raja', 'neeta'])
    


```python
#32.	Get all values from a dictionary.

dict = {"aman":23,"ram":54,"raja":45,"neeta":30}
print(dict)
print(dict.values())

```

    {'aman': 23, 'ram': 54, 'raja': 45, 'neeta': 30}
    dict_values([23, 54, 45, 30])
    


```python
#33.	Iterate through the keys in a dictionary.


famous_food = {'Gujarat': 'dhokla',
               'Maharashtra': 'vadapav',
               'Rajasthan': 'daal bhati churma',
               'Bihar': 'chat masala'
}
 
print('List Of states:\n')
for state in famous_food :
    print(state)
```

    List Of states:
    
    Gujarat
    Maharashtra
    Rajasthan
    Bihar
    


```python
#34.	Iterate through the values in a dictionary.


famous_food = {'Gujarat': 'dhokla',
               'Maharashtra': 'vadapav',
               'Rajasthan': 'daal bhati churma',
               'Bihar': 'chat masala'
}
 
print('List Of famous_food:\n')
for food in famous_food.values():
    print(food)
```

    List Of famous_food:
    
    dhokla
    vadapav
    daal bhati churma
    chat masala
    


```python
#35.	Check if a value exists in a dictionary's values.

dictionary = {"a":1,"b":2,"c":3,"d":4}
dictionary_values = dictionary.values()
if 4 in dictionary_values:
    print(4,"value exist in",dictionary)
else:
    print("not exist")
    
    
dictionary = {"a":1,"b":2,"c":3,"d":4}
dictionary_values = dictionary.values()
if 5 in dictionary_values:
    print(5,"value exist in",dictionary)
else:
    print("not exist")
```

    4 value exist in {'a': 1, 'b': 2, 'c': 3, 'd': 4}
    not exist
    


```python
#36.	Merge two dictionaries.

dict1={"banana":40,"apple":20,"orange":50}
dict2={"a":2,"b":3,"c":5}
merge = dict1|dict2
print("merging two dictinaries:",merge)

```

    merging two dictinaries: {'banana': 40, 'apple': 20, 'orange': 50, 'a': 2, 'b': 3, 'c': 5}
    


```python
#37.	Clear all elements from a dictionary.

car = {"brand": "Ford","model": "Mustang","year": 1964}
car.clear()
print("dictioanary is clear",car)
```

    dictioanary is clear {}
    


```python
#38.	Get the length of a dictionary.

car = {"brand": "Ford","model": "Mustang","year": 1964}
print("length of the dictionary is:",len(car))
```

    length of the dictionary is: 3
    


```python
#39.	Create a dictionary with keys as numbers and values as their squares.

dictionary = {}
for i in range(1,11):
    dictionary[i]=i**2
print(dictionary)


```

    {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64, 9: 81, 10: 100}
    

# sets


```python
#40.	Create an empty set.
```


```python
my_set = set()
print(my_set)
print(type(my_set))
```

    set()
    <class 'set'>
    


```python
#41.	Add an element to a set.

my_set = set()
print(my_set)
my_set.add("orange")
my_set.add("apple")
print("after adding element:",my_set)



```

    set()
    after adding element: {'apple', 'orange'}
    


```python
#42.	Remove an element from a set.

my_set = {"samsung","hp","hcl"}
print("original set:",my_set)
my_set.remove("samsung")
print("after removing the element from set",my_set)

```

    original set: {'hcl', 'samsung', 'hp'}
    after removing the element from set {'hcl', 'hp'}
    


```python
#43.	Check if an element exists in a set.

my_set = {"samsung","hp","hcl","boat","mahindra","tata"}
print(my_set)
print("samsung present in set:","samsung" in my_set)
print("iphone present in set:","iphone" in my_set)

```

    {'mahindra', 'tata', 'hcl', 'samsung', 'boat', 'hp'}
    samsung present in set: True
    iphone present in set: False
    


```python
#44.	Find the intersection of two sets.

set1 = {"apple","banana","orange","pineapple"}
set2 = {"cherry","orange","mango","apple"}
print(set1.intersection(set2))
```

    {'orange', 'apple'}
    


```python
#45.	Find the union of two sets.

set1 = {1,3,4,20,10}
set2 = {1,2,3,4,5,}
print(set1.union(set2))
```

    {1, 2, 3, 4, 5, 10, 20}
    


```python
#46.	Find the difference between two sets.

set1 = {1,3,4,20,10}
set2 = {1,2,3,4,5,}
print(set1.difference(set2))
print(set2.difference(set1))

```

    {10, 20}
    {2, 5}
    


```python
#47.	Check if one set is a subset of another.

set1 = {1,2,3,10,20,30}
set2 = {1,2,3}
print(set1)
print(set2)
print("Check if set2 is a subset of set1:",set2.issubset(set1))

```

    {1, 2, 3, 20, 10, 30}
    {1, 2, 3}
    Check if set2 is a subset of set1: True
    


```python
#48.	Remove all elements from a set.
my_set = {1,2,3,10,20,30}
print("MY SET",my_set)
my_set.clear()
print("after removing  all element:",my_set)
```

    MY SET {1, 2, 3, 20, 10, 30}
    after removing  all element: set()
    


```python
#49.	Convert a list to a set.

a=[1,2,3,4,5,6]
print(a)
print(type(a))
b=set(a)
print(b)
print(type(b))
```

    [1, 2, 3, 4, 5, 6]
    <class 'list'>
    {1, 2, 3, 4, 5, 6}
    <class 'set'>
    


```python
#50.	Convert a set to a list.

a={1,2,3,4,5,6}
print(a)
print(type(a))
b=list(a)
print(b)
print(type(b))

```

    {1, 2, 3, 4, 5, 6}
    <class 'set'>
    [1, 2, 3, 4, 5, 6]
    <class 'list'>
    


```python
#51.	Find the common elements in multiple sets.

def common(set1, set2, set3):

    set1 = set(set1)
    set2 = set(set2)
    set3 = set(set3)
    return [fruits for fruits in set1 if fruits in set2 and fruits in set3]
#driver code
set1 = {"banana","apple","pineapple","cherry","mango"}
set2 = {"mango","apple","grapes","jackfruits"}
set3 = {"grapes","mango","chery"}
print(set1)
print(set2)
print(set3)
common = common(set1, set2, set3)
print("\ncommon element in multiple set",common)
```

    {'cherry', 'mango', 'apple', 'banana', 'pineapple'}
    {'mango', 'grapes', 'jackfruits', 'apple'}
    {'chery', 'grapes', 'mango'}
    
    common element in multiple set ['mango']
    


```python
#52.	Add multiple elements to a set in one go.

my_set = {"apple","mango","cherry"}
print("orginal set",my_set)
extra = {"jackfuit","coconut","grapes"}
my_set.update(extra)
print("adding multiple elements in one go:",my_set)
```

    orginal set {'cherry', 'mango', 'apple'}
    adding multiple elements in one go: {'cherry', 'mango', 'grapes', 'coconut', 'jackfuit', 'apple'}
    


```python
#53.	Remove a specific element from a set, raising an error if not present.

my_set = {"apple","mango","cherry"}
print("original set:",my_set)
my_set.remove("jackfruit")
print(my_set)
```

    original set: {'cherry', 'mango', 'apple'}
    after removing undefine element
    


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    Cell In[130], line 6
          4 print("original set:",my_set)
          5 print("after removing undefine element")
    ----> 6 my_set.remove("jackfruit")
          7 print(my_set)
    

    KeyError: 'jackfruit'



```python
#54.	Check if two sets are disjoint (have no common elements).
set1={1,2,3,4}
set2={5,6,7,8}
set3={9,10,11,12,13}
set4={1,2}
print(set1)
print(set2)
print(set3)
print(set4)
print("checking set1 and set2 are disjoint:",set1.isdisjoint(set2))
print("checking set1 and set4 are disjoint:",set1.isdisjoint(set4))
print("checking set3 and set4 are disjoint:",set3.isdisjoint(set4))

```

    {1, 2, 3, 4}
    {8, 5, 6, 7}
    {9, 10, 11, 12, 13}
    {1, 2}
    checking set1 and set2 are disjoint: True
    checking set1 and set4 are disjoint: False
    checking set3 and set4 are disjoint: True
    

# Mixed Concepts



```python
#55.Find the second-largest element in a list.

list1=[19,30,40,78,90,40,33,50]
print(list1)
list2 = list(set(list1))
list2.sort()
print("second largest element is:",list2[-2])
```

    [19, 30, 40, 78, 90, 40, 33, 50]
    second largest element is: 78
    


```python
#56.	Merge two lists and remove duplicates.
fruit_list1 = ["Apple","banana","cherry","blue berry","orange"]
fruit_list2 = ["pinepple","rasberry","cherry","orange"]
print(fruit_list1)
print(fruit_list2)
fruit_list3 = fruit_list1 + fruit_list2
print("merged list:",fruit_list3)
duplicate = list(set(fruit_list3))
print("removing duplicate from merged list:", duplicate)


```

    ['Apple', 'banana', 'cherry', 'blue berry', 'orange']
    ['pinepple', 'rasberry', 'cherry', 'orange']
    merged list: ['Apple', 'banana', 'cherry', 'blue berry', 'orange', 'pinepple', 'rasberry', 'cherry', 'orange']
    removing duplicate from merged list: ['orange', 'rasberry', 'banana', 'pinepple', 'cherry', 'blue berry', 'Apple']
    


```python
#57.	Count the frequency of each element in a list using a dictionary.

def frequency(list1):
    counted = {}
    for items in list1:
        counted[items] = list1.count(items)
    print(counted)

#driver code
list1 = [10,2,3,4,500,6,"a","d"]
frequency(list1)

```

    {10: 1, 2: 1, 3: 1, 4: 1, 500: 1, 6: 1, 'a': 1, 'd': 1}
    


```python
#58.	Remove the last element from a list and add it to the beginning of another list.

list1 = ["table","chair","stool"]
new_list = ["chai","coffe","milk"]
print(list1)
list1.remove("stool")
print("after removing last element from list:",list1)
print("adding beginning of another list:")
new_list.insert(0,"stool")
print(new_list)

```

    ['table', 'chair', 'stool']
    after removing last element from list: ['table', 'chair']
    adding beginning of another list:
    ['stool', 'chai', 'coffe', 'milk']
    


```python
#59.	Convert a list of tuples into a dictionary.

def Convert(tup, dic):
    dic = dict(tup)
    return dic
     
# Driver Code 
tups = [("akash", 10), ("gaurav", 12), ("anand", 14),  ("suraj", 20), ("akhil", 25), ("ashish", 30)]
print(tups)
dictionary = {}
print (Convert(tups, dictionary))
```

    [('akash', 10), ('gaurav', 12), ('anand', 14), ('suraj', 20), ('akhil', 25), ('ashish', 30)]
    {'akash': 10, 'gaurav': 12, 'anand': 14, 'suraj': 20, 'akhil': 25, 'ashish': 30}
    


```python
#60.	Create a list of unique elements from a list of lists.

def unique(ls):
    res = set(x for l in ls for x in l)
    return list(res)

#driver code
lists = [[1,2,3,5], [20,30,50,40], [0,5,42,1], [30,72,2,1], [1,22,1,22]]
print("Original list:")
print(lists)
print("Unique values of the list of lists:")
print(unique(lists))

```

    Original list:
    [[1, 2, 3, 5], [20, 30, 50, 40], [0, 5, 42, 1], [30, 72, 2, 1], [1, 22, 1, 22]]
    Unique values of the list of lists:
    [0, 1, 2, 3, 5, 40, 72, 42, 50, 20, 22, 30]
    


```python
#61.	Find the intersection of two dictionaries (common keys).

dict1 = {"neil":1,"nithin":3,"nilesh":4,"navya":3,"nav":5}
dict2 = {"neil":1,"nilesh":4,"nithin":3}
print("dictionary1",dict1)
print("dictionary2",dict2)
dict3 = {x:dict1[x]for x in dict1 if x in dict2}
print("intersection of two list",dict3)

```

    dictionary1 {'neil': 1, 'nithin': 3, 'nilesh': 4, 'navya': 3, 'nav': 5}
    dictionary2 {'neil': 1, 'nilesh': 4, 'nithin': 3}
    intersection of two list {'neil': 1, 'nithin': 3, 'nilesh': 4}
    


```python
#62.	Find the symmetric difference between two sets (elements in either set, but not in both).

set_A = {1, 2, 3, 4, 5}
set_B = {6, 7, 3, 9, 4}
print(set_A)
print(set_B)
print("symmetric difference between two sets",set_A.symmetric_difference(set_B))

```

    {1, 2, 3, 4, 5}
    {3, 4, 6, 7, 9}
    symmetric difference between two sets {1, 2, 5, 6, 7, 9}
    


```python
#63.	Sort a list of dictionaries based on a specific key.

my_dict = {"avinash": 2, "animal": 1, "sarfarosh": 3,"zoom":4}
sorted_dict = dict(sorted(my_dict.items()))

print(sorted_dict)

```

    {'animal': 1, 'avinash': 2, 'sarfarosh': 3, 'zoom': 4}
    


```python
#64.	Check if two dictionaries have the same keys but different values.


dic1 = {"raj":4,"ramesh":5,"ram":6}
dic2 = {"raj":4,"ramesh":2,"ram":4}

if(dic1 == dic2):
    print("dict1 and dic2 are same")
else:
    print("dict1 and dic2 are not same")

```

    dict1 and dic2 are not same
    
