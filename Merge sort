def ms(arr,low,high):
    if(low>=high): #base condition 
        return
    mid=(low+high)//2  
    #to divide the array logic    
    ms(arr,low,mid)#low to mid =part1
    ms(arr,mid+1,high)#mid+1 to high =part2
    sort(arr,low,mid,high)# for sorting the array
def sort(arr,low,mid,high):
    #merge 2 sorted arrays logic
    i=low
    j=mid+1
    k=[]
    while(i<=mid and j<=high):
        if(arr[i]<=arr[j]):
            k.append(arr[i])
            i+=1
        else:
            k.append(arr[j])
            j+=1
    while(i<=mid):
        k.append(arr[i])
        i+=1
    while(j<=high):
        k.append(arr[j])
        j+=1
        #to replace k in original array we use for loop 
    for ind,val in enumerate(k):
        arr[low+ind]=val # arr[0+index]
arr=list(map(int,input().split()))
low=0
high=len(arr)-1
ms(arr,low,high)                           
print(arr)
