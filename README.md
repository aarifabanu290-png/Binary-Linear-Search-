# Binary-Linear-Search-
Data Structure Practicle program
23.Linear Search Program

def linear_search(arr, x):
    for i in range(len(arr)):
        if arr[i] == x:
            return i
    return -1

arr = [10, 20, 30, 40, 50]
x = 30

result = linear_search(arr, x)

if result != -1:
    print("Element found at index", result)
else:
    print("Element not found")

Output:
Element found at index 2


Binary Search Program:

def binary_search(arr, x):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) / 2

        if arr[mid] == x:
            return mid
        elif arr[mid] < x:
            low = mid + 1
        else:
            high = mid - 1

    return -1

arr = [10, 20, 30, 40, 50]
x = 40

result = binary_search(arr, x)

if result != -1:
    print("Element found at index", result)
else:
    print("Element not found")
