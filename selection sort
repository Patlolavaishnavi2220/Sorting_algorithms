def selectionsort(arr):
    n = len(arr)
    for i in range(0, n):
        Min = i
        for j in range(i+1, n):
            if arr[j] < arr[Min]:
                Min = j
        arr[i], arr[Min] = arr[Min], arr[i]

arr = list(map(int, input().split()))
selectionsort(arr)
print(arr)
