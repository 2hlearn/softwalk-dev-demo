# 10주차: # Week 10: 웹 프레임워크 사용법 (Django/Flask) - 강의 내용

### 섹션 1: 웹 프레임워크란 무엇인가?
웹 프레임워크는 개발자가 웹 애플리케이션을 더 쉽게 개발할 수 있도록 도와주는 도구입니다. HTML, CSS, JavaScript와 같은 클라이언트 측 기술뿐만 아니라, 데이터베이스와의 상호작용, 인증 시스템, 라우팅 등을 처리할 수 있는 기능을 제공합니다. 프레임워크는 일종의 "기초 공사"라고 볼 수 있습니다.

### 섹션 2: 웹 프레임워크의 진화
초기의 웹 개발은 모든 기능을 직접 코딩해야 했기 때문에 복잡하고 시간이 많이 걸렸습니다. 하지만 2000년대에 들어서면서 **Ruby on Rails**와 같은 프레임워크가 등장하여, 표준화된 방식으로 웹 애플리케이션을 개발할 수 있게 되었습니다. 이후 다양한 언어로 여러 웹 프레임워크가 등장하게 되며, Python 기반의 **Django**와 **Flask**가 대표적인 예입니다.

### 섹션 3: 웹 프레임워크의 핵심 구성 요소
대부분의 웹 프레임워크는 공통적으로 다음과 같은 요소를 포함합니다:
- **라우팅**: 사용자가 요청한 URL을 처리할 코드를 지정합니다.
- **템플릿 엔진**: 동적인 HTML 페이지를 생성하는 데 사용됩니다.
- **ORM(Object-Relational Mapping)**: 데이터베이스와의 상호작용을 코드로 처리할 수 있게 해줍니다.
- **보안**: 사용자 인증 및 권한 부여 시스템을 제공합니다.

### 섹션 4: Django와 Flask의 비교
**Django**는 "모든 것을 포함한 프레임워크"로 불리며, 대규모 애플리케이션을 쉽게 개발할 수 있도록 도와줍니다. 반면 **Flask**는 가볍고 유연한 프레임워크로, 개발자가 필요한 기능을 추가하여 사용하는 방식입니다. Django는 강력한 관리 인터페이스를 제공하지만, Flask는 단순하고 빠른 개발을 지원합니다.
- [Django와 Flask의 차이점](https://velog.io/@wonjun12/Django-Flask%EC%99%80-%EC%B0%A8%EC%9D%B4%EC%A0%90)

### 섹션 5: Django의 특징
Django는 **"빠르게 개발하라"**는 철학을 가지고 있으며, 보안, 확장성, 유지보수를 중요하게 생각하는 프레임워크입니다. 주요 특징으로는 다음이 있습니다:
- **ORM**: 데이터베이스와의 상호작용을 위한 강력한 ORM 제공
- **Admin 패널**: 관리자가 데이터를 쉽게 관리할 수 있는 자동화된 인터페이스 제공
- **보안**: CSRF, XSS와 같은 보안 위협에 대한 기본적인 보호 기능 포함

### 섹션 6: Flask의 특징
Flask는 **"가벼운 프레임워크"**로, 개발자가 필요한 기능을 선택적으로 추가할 수 있습니다. Flask는 다음과 같은 특징을 가지고 있습니다:
- **단순함**: 최소한의 설정으로 웹 애플리케이션 개발 가능
- **확장성**: 필요한 확장 모듈을 쉽게 추가할 수 있음
- **유연성**: 프로젝트의 특성에 따라 다양한 구조로 개발 가능
- [YouTube: Flask 튜토리얼](https://www.youtube.com/watch?v=Z1RJmh_OqeA)

### 섹션 7: 라우팅과 템플릿 엔진
웹 프레임워크에서 라우팅은 URL 요청을 특정 함수와 연결하는 역할을 합니다. Django와 Flask는 모두 URL 패턴을 정의하고, 그에 맞는 함수나 클래스를 실행하는 라우팅 기능을 제공합니다. 또한 **Jinja**(Flask)와 **Django 템플릿**(Django)과 같은 템플릿 엔진을 사용해 동적 웹 페이지를 생성할 수 있습니다.
```python
# Flask의 라우팅 예시
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template('home.html')
```

### 섹션 8: ORM을 통한 데이터베이스 상호작용
ORM(Object-Relational Mapping)은 개발자가 SQL을 직접 작성하지 않고도 데이터베이스와 상호작용할 수 있게 해줍니다. Django는 기본 ORM을 제공하여 데이터베이스 작업을 쉽게 할 수 있으며, Flask는 SQLAlchemy와 같은 외부 ORM을 사용할 수 있습니다.
```python
# Django ORM 예시
from myapp.models import Article
article = Article.objects.get(id=1)
```

### 섹션 9: 웹 프레임워크와 최신 기술
웹 프레임워크는 최신 기술과 결합하여 더 강력한 웹 애플리케이션을 개발할 수 있습니다. 예를 들어, GraphQL은 REST API를 대체하는 기술로 주목받고 있으며, Django와 Flask에서도 GraphQL을 사용할 수 있습니다. 또한 AI와 머신러닝을 결합한 웹 애플리케이션도 가능해졌습니다.

- [GraphQL에 대한 소개 - 생활코딩](https://youtu.be/c6qHnYa9pUk?si=pHwMF0eLyLIbomrR)

### 섹션 10: 클라우드 기반 웹 프레임워크
클라우드 기술과 웹 프레임워크의 결합으로 인해, 웹 애플리케이션을 더욱 쉽게 배포하고 관리할 수 있게 되었습니다. Django와 Flask 모두 AWS, Google Cloud, Azure 등의 클라우드 플랫폼에 배포할 수 있습니다.

- [YouTube 코딩애플: AWS에 Django 애플리케이션 배포하기](https://youtu.be/cOUhREAWJNw?si=ZkXpjJ9MyRvQ1pfu)

### 섹션 11: 웹 프레임워크 선택 기준
어떤 웹 프레임워크를 선택할지는 프로젝트의 성격과 규모에 따라 달라집니다. 대규모 프로젝트나 관리 인터페이스가 필요한 경우 Django가 적합하며, 소규모 프로젝트나 간단한 API 서버가 필요하다면 Flask가 적합합니다.

---
추가로 읽어볼 사항 - Supabase 및 Firebase 플랫폼

### 섹션 12: Supabase란?

**Supabase**는 최근 급성장하는 오픈 소스 기반의 서버리스 백엔드 플랫폼으로, Firebase의 대안으로 자주 언급됩니다. Supabase는 PostgreSQL 데이터베이스를 기반으로 하여, 풀스택 애플리케이션을 빠르게 구축할 수 있도록 도와줍니다. 특히, 실시간 데이터베이스, 인증(Authorization), 스토리지, 호스팅 등의 기능을 제공하여 백엔드 개발을 단순화하는 것이 특징입니다.

#### Supabase의 주요 기능
- **PostgreSQL 데이터베이스**: Supabase는 PostgreSQL을 기본 데이터베이스로 사용하며, 강력한 관계형 데이터베이스의 모든 기능을 활용할 수 있습니다.
- **실시간 기능**: 데이터베이스에서 변화가 발생하면 실시간으로 클라이언트에 데이터를 전달할 수 있는 기능을 제공합니다.
- **인증(Authentification)**: OAuth와 이메일 기반 인증을 쉽게 통합할 수 있으며, Google, GitHub, Apple 등 다양한 소셜 로그인 방식을 지원합니다.
- **스토리지**: 사용자가 업로드한 파일을 클라우드에 저장하고 관리할 수 있습니다.
- **RESTful API 자동 생성**: 데이터베이스 스키마를 기반으로 RESTful API를 자동으로 생성하여, 개발자가 API 구축에 시간을 들이지 않고도 데이터베이스와 상호작용할 수 있습니다.

#### Supabase와 Firebase 비교
- Firebase는 **NoSQL** 데이터베이스인 Firestore를 사용하지만, Supabase는 **관계형 데이터베이스**인 PostgreSQL을 사용합니다. 
- Supabase는 성숙한 데이터베이스 기능을 제공하기 때문에 복잡한 관계형 데이터 구조가 필요한 프로젝트에 적합합니다. 반면, Firebase는 데이터가 구조화되지 않은 애플리케이션에 유리합니다.

#### Supabase 사용 사례
1. **채팅 애플리케이션**: 실시간 데이터베이스 기능을 사용하여 실시간 채팅 기능을 빠르게 구현할 수 있습니다.
2. **블로그나 e-commerce 시스템**: RESTful API와 PostgreSQL을 활용해 빠르게 백엔드를 구축할 수 있습니다.
3. **실시간 대시보드**: 실시간 데이터를 처리하고 대시보드를 만들 때도 Supabase의 실시간 기능이 유용합니다.

### 참고 링크
- [Supabase 공식 홈페이지](https://supabase.io)
- [Supabase 사용 가이드](https://supabase.com/docs)
- [YouTube: Supabase란 무엇인가?](https://www.youtube.com/watch?v=gpB6gR7q6bU)
