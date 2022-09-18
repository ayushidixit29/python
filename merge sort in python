def merge_sort(arr, begin, end):
    if end - begin > 1:
        middle = (begin + end)//2
        merge_sort(arr, begin, middle)
        merge_sort(arr, middle, end)
        merge_list(arr, begin, middle, end)
 
def merge_list(arr, begin, middle, end):
    left = arr[begin:middle]
    right = arr[middle:end]
    k = begin
    i = 0
    j = 0
    while (begin + i < middle and middle + j < end):
        if (left[i] <= right[j]):
            arr[k] = left[i]
            i = i + 1
        else:
            arr[k] = right[j]
            j = j + 1
        k = k + 1
    if begin + i < middle:
        while k < end:
            arr[k] = left[i]
            i = i + 1
            k = k + 1
    else:
        while k < end:
            arr[k] = right[j]
            j = j + 1
            k = k + 1
 
 
arr = input('Enter the list of numbers: ').split()
arr = [int(x) for x in arr]
merge_sort(arr, 0, len(arr))
print('Sorted list: ', end='')
print(arr)
