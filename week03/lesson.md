# 3주차 강의: 프로그래밍 기초 (Python) - 강의 내용

### 섹션 1: Python이란 무엇인가?
Python은 간결하고 가독성이 좋은 프로그래밍 언어입니다. 다양한 플랫폼에서 실행 가능하며, 초보자부터 전문가까지 폭넓게 사용됩니다. Python은 범용 언어로 웹 개발, 데이터 분석, 인공지능 등에 사용됩니다.

### 섹션 2: Python 설치 및 환경 설정
Python을 설치하는 방법과 개발 환경을 설정하는 방법을 다룹니다. Python.org에서 Python을 다운로드하고 설치할 수 있으며, 기본적인 텍스트 편집기나 IDE(예: VS Code, PyCharm)를 사용하여 코드를 작성할 수 있습니다.

- [Python 다운로드 링크](https://www.python.org/downloads/)
- [YouTube: Python 설치 및 환경 설정](https://www.youtube.com/watch?v=kLZuut1fYzQ)

### 섹션 3: 변수와 데이터 타입
Python에서 변수는 값을 저장하는 공간입니다. 변수를 선언할 때 데이터 타입을 지정하지 않아도 되며, Python은 자동으로 데이터 타입을 결정합니다. 주요 데이터 타입에는 숫자, 문자열, 리스트, 딕셔너리 등이 있습니다.
```python
name = "SoftWalk"
age = 53
height = 1.75
is_enrolled = True

### 섹션 4: 산술 연산 및 변수 조작
Python에서 다양한 산술 연산을 수행할 수 있습니다. 더하기(+), 빼기(-), 곱하기(*), 나누기(/)와 같은 기본 연산 외에도 지수 연산(**)이나 나머지 연산(%) 등을 활용할 수 있습니다.

result = 5 + 3  # result는 8
python```

### 섹션 5: 제어문 - if 조건문
if 문을 사용하여 조건에 따라 다른 코드를 실행할 수 있습니다. Python의 조건문은 들여쓰기를 통해 코드 블록을 구분합니다.

if age > 50:
    print("중년층입니다.")
else:
    print("젊은층입니다.")

### 섹션 6: 반복문 - for, while
for 문과 while 문을 사용하여 반복 작업을 수행할 수 있습니다. 특히 for 문은 리스트, 튜플 등과 같은 데이터 구조의 항목을 순차적으로 처리할 때 유용합니다.

for i in range(5):
    print(i)

### 섹션 7: 함수 정의 및 호출
Python에서 함수는 코드의 재사용성을 높이고, 코드를 모듈화하는 데 유용합니다. 함수를 정의한 후, 필요한 곳에서 호출하여 사용할 수 있습니다.

def greet(name):
    return f"Hello, {name}!"

greeting = greet("SoftWalk")
print(greeting)

### 섹션 8: 리스트와 딕셔너리
리스트는 순차적으로 값을 저장하는 자료 구조이며, 딕셔너리는 키-값 쌍으로 데이터를 저장하는 구조입니다.

fruits = ["apple", "banana", "cherry"]
scores = {"math": 90, "english": 85}

### 섹션 9: Python의 내장 함수 활용
Python은 다양한 내장 함수를 제공하여, 기본적인 작업을 쉽게 처리할 수 있습니다. 예를 들어, len() 함수는 리스트나 문자열의 길이를 반환합니다.

print(len(fruits))  # 3 출력

### 섹션 10: 실습 - 간단한 프로그램 작성
학습한 내용을 바탕으로 간단한 계산기 프로그램을 작성합니다. 이 프로그램은 두 수를 입력받아 더하기, 빼기, 곱하기, 나누기를 수행합니다.

def calculator(num1, num2, operation):
    if operation == "add":
        return num1 + num2
    elif operation == "subtract":
        return num1 - num2
    elif operation == "multiply":
        return num1 * num2
    elif operation == "divide":
        return num1 / num2

print(calculator(10, 5, "add"))  # 15 출력

### 외부 리소스
[YouTube 강의: Python 기초] (https://www.youtube.com/watch?v=tRZGeaHPoaw)
[Python 기초 학습 자료 (freeCodeCamp - 한국어 버전)] (https://www.freecodecamp.org/korean/news/python-projects-for-beginners/)


---

이 파일은 Python의 기초 문법을 이해하기 위한 다양한 주제를 다루며, 실제로 접근 가능한 외부 리소스도 포함했습니다. 추가로 수정할 사항이 있으면 말씀해 주세요!
