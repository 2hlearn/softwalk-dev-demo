# 6주차 강의: GitHub 협업 심화 - 강의 내용

### 섹션 1: GitHub 협업의 중요성
GitHub는 개발자들이 협업할 수 있는 플랫폼으로, 소스 코드 관리를 돕습니다. GitHub는 버전 관리, 코드 리뷰, 협업 도구 제공을 통해 팀이 더 효율적으로 소프트웨어를 개발할 수 있게 합니다.

### 섹션 2: 브랜치 관리
브랜치는 Git에서 변경 사항을 독립적으로 관리할 수 있게 도와줍니다. 각 개발자는 자신의 브랜치를 생성하여 작업한 후, 이를 병합(Merge)하여 메인 프로젝트에 반영할 수 있습니다.
```bash
# 브랜치 생성 및 이동
git checkout -b feature-branch
```

### 섹션 3: Fork와 Pull Request
Fork는 다른 사용자의 저장소를 복사하여 자신의 저장소로 가져오는 작업입니다. 이 후 변경 사항을 반영할 때는 Pull Request를 통해 원래의 저장소로 변경 사항을 요청할 수 있습니다. Pull Request는 GitHub 협업에서 중요한 요소입니다.

- [YouTube: Pull Request 튜토리얼](https://www.youtube.com/watch?v=rgbCcBNZcdQ)

### 섹션 4: Merge와 충돌 해결
브랜치를 병합(Merge)할 때 코드 충돌이 발생할 수 있습니다. 충돌은 두 명 이상의 개발자가 동일한 파일의 같은 부분을 수정할 때 발생하며, 이를 해결하려면 수동으로 코드를 조정해야 합니다.
```bash
# 병합 명령어
git merge feature-branch
```

### 섹션 5: Pull Request에서 코드 리뷰
Pull Request를 생성하면, 다른 팀원들이 코드를 검토(리뷰)할 수 있습니다. 코드 리뷰는 코드 품질을 높이고, 협업 팀원 간의 상호 피드백을 통해 코드의 버그를 줄일 수 있습니다.

- [YouTube: GitHub 코드 리뷰 가이드](https://www.youtube.com/watch?v=P88k-NwR1nA)

### 섹션 6: GitHub Actions
GitHub Actions는 자동화된 워크플로우를 설정할 수 있는 도구입니다. 예를 들어, Pull Request가 생성되면 자동으로 테스트를 실행하고, 결과를 팀에게 전달할 수 있습니다. 이 기능을 통해 협업 프로세스를 자동화하고 효율적으로 관리할 수 있습니다.

- [GitHub Actions 공식 가이드](https://docs.github.com/en/actions)

### 섹션 7: 팀 협업에서의 브랜치 전략
협업에서 브랜치를 관리하는 방법에는 여러 가지가 있습니다. 가장 일반적인 방법으로는 Git Flow, GitHub Flow, 그리고 Trunk-Based Development가 있습니다. 각 전략은 프로젝트 규모나 팀에 따라 적절한 방법을 선택할 수 있습니다.

### 섹션 8: Git 태그(Tag)
태그는 프로젝트의 특정 지점을 "마크"하여, 중요한 버전이나 배포 시점을 기록하는 데 사용됩니다. 일반적으로 릴리즈 버전을 나타내는 데 사용됩니다.
```bash
# 태그 생성
git tag v1.0
```

### 섹션 9: Git Rebase와 Cherry-pick
Rebase는 브랜치의 변경 사항을 다른 브랜치에 적용하는 방식으로, 병합 기록을 깔끔하게 유지하는 데 사용됩니다. Cherry-pick은 특정 커밋만 선택하여 다른 브랜치에 적용할 때 사용됩니다.
```bash
# Rebase 명령어
git rebase main
```

### 섹션 10: GitHub 프로젝트 관리 도구
GitHub는 프로젝트 관리를 위한 Kanban 보드 기능을 제공합니다. 이를 통해 개발팀은 작업의 상태를 시각적으로 관리하고, 작업 진행 상황을 추적할 수 있습니다.

* [GitHub Projects 사용법] (https://docs.github.com/en/issues/organizing-your-work-with-project-boards)

