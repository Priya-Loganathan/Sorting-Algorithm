# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```python
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Delli Priya L 
RegisterNumber: 22006375
def SelectionSort(array,size):
    for ind in range(size):
        min_index = ind
        for j in range(ind + 1, size):
             if array[j] < array[min_index]:
               min_index = j
               (array[ind],array[min_index]) = (array[min_index],array[ind])
arr = eval(input())
size = len(arr)
SelectionSort(arr,size)
print(arr)
```
ii)	#Insertion Sort
```python
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Delli Priya L
RegisterNumber: 22006375 
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j >=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```
## Output:
![Screenshot 2023-01-23 200533](https://user-images.githubusercontent.com/121166075/214066834-f828eeec-4e95-4f4a-828f-b2081602e42d.png)
![Screenshot 2023-01-23 200627](https://user-images.githubusercontent.com/121166075/214066882-dac25171-6814-47aa-a100-09c1e4bf4f18.png)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
