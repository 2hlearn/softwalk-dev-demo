# 7주차 강의: Python 심화 - 강의 내용

### 섹션 1: 파일 입출력이란?
파일 입출력은 프로그램이 외부 파일을 읽거나 쓰는 작업입니다. Python에서는 `open()` 함수를 통해 파일을 열고, 데이터를 읽거나 쓰고, 작업이 끝나면 `close()` 함수를 통해 파일을 닫습니다. 파일 입출력은 로그 저장, 데이터 파일 생성 등에 자주 사용됩니다.

### 섹션 2: 파일 열기와 닫기
파일을 열 때는 읽기 모드(`r`), 쓰기 모드(`w`), 추가 모드(`a`) 중 하나를 선택할 수 있습니다. `with` 문을 사용하면 파일 작업 후 자동으로 파일이 닫히므로 안전합니다.
```python
with open('example.txt', 'r') as file:
    content = file.read()
```

### 섹션 3: 파일 읽기 (read, readline, readlines)
파일을 읽는 방법은 read()로 전체 파일을 읽거나, readline()으로 한 줄씩 읽을 수 있습니다. readlines()는 파일의 각 줄을 리스트로 반환해줍니다.
```python
with open('example.txt', 'r') as file:
    for line in file:
        print(line)
```

### 섹션 4: 파일 쓰기
파일에 데이터를 쓰는 방법입니다. write() 함수를 사용하면 텍스트를 파일에 기록할 수 있으며, 기존 파일이 덮어쓰여집니다.
```python
with open('example.txt', 'w') as file:
    file.write("이 파일은 Python으로 작성되었습니다.")
```

### 섹션 5: 예외 처리란 무엇인가?
프로그램을 실행하는 도중 오류가 발생할 수 있습니다. 예외 처리는 이러한 오류를 처리하는 방법으로, 프로그램이 갑자기 멈추지 않고 부드럽게 예외 상황을 해결하도록 돕습니다.

```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("0으로 나눌 수 없습니다.")
```

### 섹션 6: 다양한 예외 처리
Python에서는 여러 종류의 예외를 처리할 수 있으며, except 구문을 여러 개 사용하여 각각의 예외 상황에 맞게 처리할 수 있습니다.
```python
try:
    file = open('nonexistent_file.txt', 'r')
except FileNotFoundError:
    print("파일이 없습니다.")
except IOError:
    print("파일을 읽는 중 오류가 발생했습니다.")
```

### 섹션 7: 예외 처리의 장점
예외 처리를 사용하면 프로그램이 예외 상황에서 멈추지 않고 계속 실행되며, 사용자가 잘못된 입력을 하거나 외부 요인으로 문제가 발생했을 때도 안전하게 처리할 수 있습니다. 또한 오류 메시지를 사용자에게 의미 있게 전달할 수 있습니다.

### 섹션 8: 모듈이란 무엇인가?
모듈은 미리 정의된 Python 코드 파일로, 여러 프로그램에서 재사용할 수 있는 함수나 변수를 담고 있습니다. Python에서 모듈을 가져오려면 import를 사용합니다.
```python
import math
print(math.sqrt(16))  # 4.0 출력
```

### 섹션 9: 모듈 만들기
자신의 모듈을 만들려면 Python 파일에 함수를 정의한 후, 이를 다른 파일에서 import하여 사용할 수 있습니다.
```python
# my_module.py 파일에 작성
def hello(name):
    return f"안녕하세요, {name}!"

# 다른 파일에서 import
from my_module import hello
print(hello("SoftWalk"))
```

### 섹션 10: 패키지 사용하기
패키지는 여러 모듈을 포함한 폴더 구조입니다. 패키지는 대규모 프로젝트에서 코드를 체계적으로 관리하는 데 유용합니다. 패키지 디렉토리에는 __init__.py 파일이 포함되어야 합니다.
```plaintext
my_package/
    __init__.py
    module1.py
    module2.py
```

### 외부 리소스
- [YouTube 강의: Python 파일 입출력 튜토리얼](https://www.youtube.com/watch?v=Uh2ebFW8OYM)
- [YouTube 강의: 예외 처리 가이드](https://www.youtube.com/watch?v=P0F3h9OF1WY)
- [Python 모듈과 패키지 설명 - 생활코딩](https://youtu.be/45pERzGJM64?si=aI8S66z3jn6OYqF3)
