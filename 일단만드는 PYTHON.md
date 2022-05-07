#

```python
import random #랜덤 모듈

print(random.choice(["된장찌개", "피자", "제육볶음"]))
```

리스트의 내용을 랜덤으로 하나 출력하는 코드

```python
import random
import time

while True:
    print(random.choice(["된장찌개","치킨","떡볶이","라면","감자튀김"]))
    break
    print("이 문장도 반복되나")
    time.sleep(1)
```

for : 반복 횟수 지정 가능

while : 무한 루프를 돌림. 멈추는 법 break, 시간을 주는 법 sleep

```python
import random

lunch = random.choice(["된장찌개","피자","제육볶음"])
lunch = "냉장고"
dinner = random.choice(["김밥","쫄면","돈까스"])
print(lunch)
```

변수에 랜덤 값 지정

```python
information = {"고향":"수원", "취미":"영화관람", "좋아하는 음식":"국수"}
print(information)
print(information.get("취미"))

information = {"특기":"피아노", "사는곳":"서울"}
print(information.get("특기"))
print(information.get("사는곳"))
```

딕셔너리 작성법 {key:value} key로 찾는법 .get

```python
information = {"고향":"수원", "취미":"영화관람","좋아하는 음식":"국수"}
foods = ["된장찌개", "피자", "제육볶음"]
print(information.get("취미"))
information["특기"] = "피아노"
information["사는곳"] = "서울"
del information["좋아하는 음식"]
print(information)
print(len(information))
information.clear()
print(information)
print(foods[3]) #-> Index error
```

리스트[index] → 해당 값에 접근한다. 0부터 시작 음수의 경우 -1부터 맨 뒤부터 접근

리스트 추가:append, 리스트 삭제:del

```python
for x in range(30):
    print(x)

foods = ["된장찌개", "피자", "제육볶음"]
for x in range(3):
    print(foods[x])
for x in foods:
    print(x)

information = {"고향":"수원", "취미":"영화관람", "좋아하는 음식":"국수"}
for x, y in information.items():
    print(x)
    print(y)
```

for문으로 리스트 값을 바로 접근할 수 있다. 딕셔너리도 가능하다. .items()

set은 리스트의 중복을 제거해준다.(집합)

합집합, 차집합도 가능하다(+, -)

```python
import random

food = random.choice(["된장찌개","피자","제육볶음"])

print(food)
if(food == "제육볶음"):
    print("곱배기 주세요")
else:
    print("그냥 주세요")
print("종료")
```

if-else문으로 값에 따른 처리 가능

1. while문으로 반복 입력 가능(추가/삭제)
2. if문으로 입력값에 따라 break로 종료 가능
3. set으로 리스트의 중복을 제거한다.
4. sleep으로 출력 타이밍 조절 가능

```python
import random
import time

lunch = ["된장찌개", "피자", "제육볶음", "짜장면"]

while True:
    print(lunch)
    item = input("음식을 추가 해주세요 : ")
    if(item == "q"):
        break
    else:
        lunch.append(item)
print(lunch)

set_lunch = set(lunch)
while True:
    print(set_lunch)
    item = input("음식을 삭제해주세요 : ")
    if(item == "q"):
        break
    else:
        set_lunch = set_lunch - set([item])

print(set_lunch, "중에서 선택합니다.")
print("5")
time.sleep(1)
print("4")
time.sleep(1)
print("3")
time.sleep(1)
print("2")
time.sleep(1)
print("1")
time.sleep(1)
print(random.choice(list(set_lunch)))
```

---

함수 만들기
`def 함수명(): 코드 작성`

질문과 답을 {key:value} 딕셔너리 형태로 저장
먼저 질문을 입력받고 while문이 종료되면 답변을 입력하는 while문 실행
