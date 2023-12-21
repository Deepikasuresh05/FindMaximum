# Find the maximum of a list of numbers
## Aim:
To write a program to find the maximum of a list of numbers.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the list of marks as input
2.	Use the sort() function or max() function or use the for loop to find the maximum mark.
3.	Return the maximum value
## Program:

i)	# To find the maximum of marks using the list method sort.
```
''' 
Program for linear search method to match the item in a list
Developed by: S Deepika
RegisterNumber: 23002257
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i] == k):
            return i
    return -1
array = eval(input())
k = eval(input())
n = len(array)
array.sort()
result = linearSearch(array,n,k)
if(result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
   
```




ii)	# To find the maximum marks using the list method max().
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by: S Deepika
RegisterNumber: 23002257
'''
def binarySearchIter(array, k , low , high):
    while low <= high:
        mid = low + (high - low)//2
        if array[mid] == k:
            return mid
        elif array[mid] < k:
            low = mid + 1
        else:
            high = mid - 1
    return -1
array = eval(input())
array.sort()
k = eval(input())
result = binarySearchIter(array, k,0,len(array)-1)
if(result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```

iii) # To find the maximum marks without using builtin functions.
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: your name : S Deepika
RegisterNumber: 23002257
'''
def BinarySearch(arr, k, low, high):
    while low <= high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low = mid+1
        else:
            high = mid - 1
    return -1
    
array = eval(input())
array.sort()
k=eval(input())
result = BinarySearch(array , k, 0, len(array)-1)
print(array)
if result !=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")
```
## Sample Input and Output
![output](./img/max_marks1.jpg) 

## Output:
![image](https://github.com/Deepikasuresh05/FindMaximum/assets/148514509/6d49dc24-781e-4024-9034-cce880a22ecc)

![image](https://github.com/Deepikasuresh05/FindMaximum/assets/148514509/ef74c641-8064-447f-8377-9065e8e0f9ff)

![image](https://github.com/Deepikasuresh05/FindMaximum/assets/148514509/09665905-aaba-4d6c-9f9a-18825d458130)




## Result:
Thus the program to find the maximum of given numbers from the list is written and verified using python programming.
