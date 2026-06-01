# 1. Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim:

To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm:

1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program:

```
import math

class cse:
    def mech(self, r):
        c = math.pi * r**2
        print(f"Area of circle: {c:.2f}")

r = int(input("Enter radius: "))
ci = cse() 
ci.mech(r)
```

## Output:

<img width="648" height="326" alt="image" src="https://github.com/user-attachments/assets/f2445a2d-ad45-4d4d-9526-398c4ec50532" />

## Result:
Thus, the program that calculates the area of a circle based on the radius provided by the user is executed successfully.




# 2. Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim:

To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm:

1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program:

```
dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

def merge(dict1, dict2):
    res = {**dict1, **dict2}
    return res

dict3 = merge(dict1, dict2)
print(dict3)
```

## Output:

<img width="1078" height="163" alt="image" src="https://github.com/user-attachments/assets/33588b59-b6bf-4556-99c6-5394b0ed05b2" />

## Result:
Thus, the program that merges two dictionaries and combines their key-value pairs was executed successfully.




# 3. Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

## 🎯 Aim:

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

## 🧠 Algorithm:

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

## 🧪Program:
```
d={2:56,1:2,5:12,4:24,6:18,3:323}
l=[]
for i in d:
    l.append(i)
l.sort()
print("Keys and Values sorted in alphabetical order by the key")
for i in l:
    print(tuple([i,d[i]]),end=" ")
```

## Output:

<img width="1270" height="378" alt="image" src="https://github.com/user-attachments/assets/69c67396-54df-4b5c-921d-8bca9c178cc7" />

## Result:
Thus, the program that sorts a dictionary's Keys and Values in alphabetical order was executed successfully.




# 4. Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim:

To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm:

1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program:

```
lis=[5, 10, 20]
try:
    print(lis[5])
except:
    print("You're out of list range")
```

## Output:

<img width="614" height="294" alt="image" src="https://github.com/user-attachments/assets/87e25488-ea8f-4bf9-b118-8f0fcac0af7e" />

## Result:
Thus, the program that handles an IndexError when trying to access an element beyond the available range of a list was executed successfully.





# 5. File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim:

To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm:

1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program:

```
count = 0
with open("story.txt", "r") as file:
    for line in file:
        if line.strip() and not line.lstrip().startswith('T'):
            count += 1
print("Sum :", count)
```

## Output:

<img width="395" height="167" alt="image" src="https://github.com/user-attachments/assets/c3996f86-2b7f-466f-8f0f-49dc514cac4f" />

## Result:
Thus, the program that counts the number of lines in a text file story.txt that do not start with the alphabet 'T' was executed successfully.
