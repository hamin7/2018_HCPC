a=[]
b=[]
n=1

while(n!='0'):
    n=input()
    a.append(n)
del a[-1]
for i in range(3):
    n=input()
    b.append(n)
for i in range(len(b)):
    b[i]=b[i].replace('WHO',b[0])
    b[i]=b[i].replace('WHERE',b[1])
    b[i]=b[i].replace('WHAT',b[2])

for i in range(len(a)):
    a[i]=a[i].replace('WHO',b[0])
    a[i]=a[i].replace('WHERE',b[1])
    a[i]=a[i].replace('WHAT',b[2])
    
for i in range(len(a)):
    print(a[i])

