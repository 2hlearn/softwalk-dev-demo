# 11주차: 실습 및 리서치 과제

### 실습 과제 1: OOP 원칙 적용하기
1. **객체 지향 프로그래밍 실습**  
   간단한 클래스 구조를 설계하고 OOP의 4대 원칙을 적용하세요. 예를 들어, "동물원"이라는 프로그램을 만들어, 다양한 동물들이 공통적으로 가지고 있는 속성과 동작(캡슐화)을 정의한 후, 특정 동물 클래스에서 상속과 다형성을 적용하세요.
   
```python
   class Animal:
       def __init__(self, name):
           self.name = name
           
       def sound(self):
           raise NotImplementedError("이 메서드는 서브클래스에서 구현해야 합니다.")
   
   class Dog(Animal):
       def sound(self):
           return "멍멍"
   
   class Cat(Animal):
       def sound(self):
           return "야옹"
   
   animals = [Dog("강아지"), Cat("고양이")]
   for animal in animals:
       print(f"{animal.name}: {animal.sound()}")
```

### 실습 과제 2: 디자인 패턴 적용하기
싱글턴 패턴 적용하기
프로그램에서 한 번만 생성되어야 하는 객체(예: 데이터베이스 연결)를 싱글턴 패턴을 사용하여 구현하세요. Python으로 싱글턴 패턴을 구현하는 방법을 학습하고, 이를 통해 간단한 데이터베이스 연결 클래스를 만들어 보세요.
```python
class DatabaseConnection:
    _instance = None
    
    def __new__(cls):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
            cls.connection = cls.create_connection()
        return cls._instance
    
    @staticmethod
    def create_connection():
        return "데이터베이스 연결 설정 완료"
    
db1 = DatabaseConnection()
db2 = DatabaseConnection()

print(db1.connection)  # 출력: 데이터베이스 연결 설정 완료
print(db1 is db2)      # 출력: True (싱글턴 확인)
```

### 리서치 과제 1: OOP와 절차적 프로그래밍 비교
#### OOP와 절차적 프로그래밍 비교하기
객체 지향 프로그래밍과 절차적 프로그래밍의 차이점을 조사하고, 각각의 장단점을 요약하여 제출하세요. OOP가 더 적합한 상황과 절차적 프로그래밍이 더 유리한 경우를 구체적으로 설명하세요.

### 리서치 과제 2: 디자인 패턴의 실제 적용 사례
#### 디자인 패턴의 실제 적용 사례 조사
실제 소프트웨어 개발에서 사용된 디자인 패턴 사례를 조사하세요. 각 사례에서 사용된 디자인 패턴이 문제 해결에 어떻게 기여했는지 설명하고, 그 효과를 요약하여 제출하세요.

### 제출 방법
실습 코드를 마크다운 파일로 작성하고, GitHub에 업로드하여 Pull Request를 통해 제출하세요.
리서치 과제의 요약본을 마크다운 파일로 작성하여 제출하세요.
