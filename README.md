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

