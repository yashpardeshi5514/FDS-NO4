def create_float_list():
    try:
        n = int(input("Enter the number of student:"))
        float_list = []
        for _ in range(n):
            num = float(input("Enter a % number: "))
            float_list.append(num)
        return float_list
    except ValueError:
        print("Invalid input. Please enter numeric values.")
user_float_list = create_float_list()
print("The created student  % list:",user_float_list)
 
def selection_sort(arr):
    for i in range (0,len(arr)):
        a=i
        for j in range(i+1,len(arr)):
            if arr[a]>arr[j]:
                a=j
        arr[i],arr[a]=arr[a],arr[i]
    return arr
 
 
def bubble_sort(arr):
    for i in range(len(arr)):
        for i in range (0,len(arr)):
            if i==len(arr)-1:
                break
            elif arr[i]>arr[i+1]:
                arr[i],arr[i+1]=arr[i+1],arr[i]
    return arr
print (f" 1st selection sort student % and 2nd bubble sort student
%:\n{selection_sort(user_float_list),bubble_sort(user_float_list)}\n")
