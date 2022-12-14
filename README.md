# descending-order-without-library-functions
l=[]
n=int(input('Enter how many numbers you want:'))
a=list(map(int,input('Enter any number:').split()))
for i in range(0,n-1):
    for j in range(i+1,n):
        if a[i]<a[j]:
            t=a[i]
            a[i]=a[j]
            a[j]=t
for i in range(0,n):
    print(a[i],end=' ')
