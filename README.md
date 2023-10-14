# 775
задачи по инфе


| № | Тип |
| ------ | ------ |
| 1 | p |
| 2 | p\c |
| 3 | e |
| 4 | p |
| 5 | c |
| 6 | c |
| 7 | p |
| 8 | c |
| 9 | e |
| 10 | p |
| 11 | p |
| 12 | c |
coding
| 13 | p\c |
| 14 | c |
| 15 | c |
| 16 | c |
| 17 | c+файл |
| 18 | e |
| 19 | p\c\e |
| 20 | p\c\e |
| 21 | p\c\e |
| 22 | e |
| 23 | c |
| 24 |c |
| 25 |c |
| 26 |c |
| 27 | |



read me
def f3():
    for n in range(4, 10000):
        s = '5' + n*'2'
        while '52' in s or '2222' in s or '1122' in s:
            s = s.replace('52', '11', 1)
            s = s.replace('2222', '5', 1)
            s = s.replace('1122', '25', 1)
            if sum(map(int, s)) == 64:
                print(n)
f3()
def f3():
    for n in range(4, 10000):
        s = '5' + n*'2'
        while '52' in s or '2222' in s or '1122' in s:
            s = s.replace('52', '11', 1)
            s = s.replace('2222', '5', 1)
            s = s.replace('1122', '25', 1)
            if sum(map(int, s)) == 64:
                print(n)

import sys        
def f16_2(n):
    sys.setrecursionlimit(2500)
    if n == 1 : return 1
    if n>1 : return n * f16_2(n-1)
print(f16_2(2023) / f16_2(2020))


def f17():
    with open('17.txt') as f:
        nums=[int(x) for x in f]
    maxi=[]
    s=[]
   
    for i in range(len(nums)):
      if nums[i]%10==3:
         maxi.append(nums[i])
    maximum=0
    for i in range(len(nums)-1):
        a=abs(nums[i])%10
        b=abs(nums[i+1])%10
        if ((a==3) and (b!=3)) or ((a!=3) and (b==3)):
            if (nums[i]**2+nums[i+1]**2) >= max(maxi)**2: 
                s.append(nums[i]+nums[i+1])
            if nums[i]**2+nums[i+1]**2>maximum:
                maximum=nums[i]**2+nums[i+1]**2
    print(len(s), maximum)
f17()
def f19_21
    def f(a,m):
        if a>77: return m%2==0
        if m==0: return 0
        actions=(a+1),(a+4),(a*4)
        steps=[f(a,m-1) for a in actions]
        if m%2==0: return all(steps)
        else: return any(steps)

        s20=[s for s in range(1,78) if not f(s,1) and f(s,3) ]
        print(s20)

        s21=[s for s in range(1,78) if f(s,4) ]
        print(min(s21))

    def f23(x,y):
        if x>y or x==17:
            return 0
        elif x==y:
            return 1
        return f23(x+1,y) +f23(x*2,y)
    print(f23(1,10)*f23(10,35))

def f24():
    with open('24.txt') as f:
        s=f.readline().replace('C','S').replace('D','S').replace('F','S')
    s=s.replace('A','G').replace('O','G')
    s=s.replace('SG','*')
    k=kmax=0
    for i in s:
        if i=='*':
            k+=1
            kmax=max(k,kmax)
        else:k=0
print(kmax)

