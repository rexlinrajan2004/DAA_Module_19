# EX 1C Quick Sort
## DATE:
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Select the last element as pivot.
2. Partition the array around the pivot.
3. Recursively quick sort left subarray.
4. Recursively quick sort right subarray.
5. Take float inputs, sort, and print the result.  

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: Rexlin R
Register Number:  212222220034
*/
```
```
def quickSort(nums,l,r):
    if len(nums)==1:
        return nums
    if l<r:
        pi=part(nums,l,r)
        quickSort(nums,l,pi-1)
        quickSort(nums,pi+1,r)
def part(nums,l,r):
    pi,ptr=nums[r],l
    for i in range(l,r):
        if nums[i]<=pi:
            nums[i],nums[ptr]=nums[ptr],nums[i]
            ptr+=1
    nums[ptr],nums[r]=nums[r],nums[ptr]
    return ptr
n=int(input())
arr=[float(input()) for i in range(n)]
quickSort(arr,0,n-1) 
print("Sorted array is:")
for i in range(n):
    print(arr[i])
```

## Output:
![image](https://github.com/user-attachments/assets/78cf6575-5df5-41c2-8aae-f2bad7abdaa0)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
