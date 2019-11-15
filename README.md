# python-3
<for문> 
for + 변수 + in + 시퀀스

새파일
for fruit in["바나나","사과","배","감"]:
    print("과일 이름:"+fruit)
저장(F5)
과일 이름:바나나
과일 이름:사과
과일 이름:배
과일 이름:감

for num in[0,1,2,3,4,5,6,7,8,9]:
    print(num)
0
1
2
3
4
5
6
7
8
9

for num in[0,1,2,3,4,5,6,7,8,9]:
    print(num,end="")
0123456789

for num in[0,1,2,3,4,5,6,7,8,9]:
    print("정수 %d입니다."%num)
정수 0입니다.
정수 1입니다.
정수 2입니다.
정수 3입니다.
정수 4입니다.
정수 5입니다.
정수 6입니다.
정수 7입니다.
정수 8입니다.
정수 9입니다.

for num in[0,1,2,3,4,5,6,7,8,9]:
    print("%d번째값, 정수 %d입니다."%(num+1,num)) 
1번째값, 정수 0입니다.
2번째값, 정수 1입니다.
3번째값, 정수 2입니다.
4번째값, 정수 3입니다.
5번째값, 정수 4입니다.
6번째값, 정수 5입니다.
7번째값, 정수 6입니다.
8번째값, 정수 7입니다.
9번째값, 정수 8입니다.
10번째값, 정수 9입니다.

<range( 숫자)>- 0에서 숫자  -1까지 정수 출력(실수는 입력하지 않음)
for num in range(10):
    print(num) 
0
1
2
3
4
5
6
7
8
9

for num in range(0,10): -> 0부터 10개!!
    print(num) 
0
1
2
3
4
5
6
7
8
9

1~10까지 합 55가 출력
sum=0
for num in range(1,11):
    sum=sum+num
print(sum)
55

for num in range(start,stop,step) -> start에서 stop-1숫자까지 step간격으로 정수 출력
for num in range(0,10,2):
    print(num)
0
2
4
6
8

for문
for cha in "abcde":
    print(cha,end=" ")
a b c d e

<While문>
0에서 9까지 정수는 찍는 코드
i=0
while i <10:
    print(i)
    i=i+1
0
1
2
3
4
5
6
7
8
9

구구단 5단을 완성하자
i=1
while i<10:
    print("5*%d=%d"%(i,5*i))
    i=i+1
5*1=5
5*2=10
5*3=15
5*4=20
5*5=25
5*6=30
5*7=35
5*8=40
5*9=45

<break문>
i=0
while i<10:
    i=i+1
    if i ==5:
        print("if문을 통해 break.")
        break
    print(i)
1
2
3
4
if문을 통해 break.

<continue문>
i=0
while i<10:
    i=i+1
    if i ==5:
        print("if문을 통해 continue.")
        continue
    print(i)
1
2
3
4
if문을 통해 continue.
6
7
8
9
10

<turtle을 이용한 별 그리기>
import turtle

t= turtle.Pen()

for i in range(5):
    t.forward(50)
    t.right(144)
    
<함수 만들기>
def 함수이름 (매개변수1, 매개변수2):->매개변수 없어도 괜찮아
    실행할 문장
    실행할 문장

- 매개변수 없는 함수 만들기
def greeting():
    print("만나서 반가워")
    print("나는 채오니야")
    print("친하게 지내자")
>>> greeting()
만나서 반가워
나는 채오니야
친하게 지내자
    
- 매개변수 1개
def greeting(name):
    print("만나서 반가워")
    print("나는 %s이야"%name)
    print("친하게 지내자")
>>> greeting("채원")
만나서 반가워
나는 채원이야
친하게 지내자

- 매개변수 2개
def greeting(name,age):
    print("만나서 반가워")
    print("나는 %s이야"%name)
    print("나는 %d살이야"%age)
    print("친하게 지내자")
>>> greeting("채원",18)
만나서 반가워
나는 채원이야
나는 18살이야
친하게 지내자
