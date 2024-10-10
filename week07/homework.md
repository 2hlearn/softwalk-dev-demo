# 7주차 과제

### 실습 과제
1. **파일 입출력 실습**  
   새로운 파일을 생성하여 간단한 텍스트를 작성한 후, 다시 그 파일을 읽어서 출력하세요. 이 작업을 `with` 문을 사용하여 안전하게 처리하세요.
   
   ```python
   with open('homework.txt', 'w') as file:
       file.write("이것은 숙제 파일입니다.")
   
   with open('homework.txt', 'r') as file:
       content = file.read()
       print(content)
```
