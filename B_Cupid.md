~~~py
a=input()
a=a.split(' ')
r=[]
n=int(input())
for i in range(n):
    s=input()
    s=s.split(' ')
    if(len(s)!=3):break
    if(a[1]=='FM' or a[1]=='MF'):
        if(int(a[2])>=int(s[2])):
            r.append(s[0])
    elif(a[1]==s[1]):
        if(int(a[2])>=int(s[2])):
            r.append(s[0])

r = sorted(r)

if(len(r)==0):
    print('No one yet')
else:
    for i in r:
        print(i)      

~~~
