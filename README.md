## Git 연습
- GitHub와 Git을 사용하며 겪은 여러 오류들과 지식들을 모두 적는 곳

<br>

# 브랜치
- 작업 전에 해당 브랜치 이동하기

<br>

## 브랜치 이동
- 변경된 사항이 있는 경우에는 다른 브랜치로 이동할 수 없음. stash해서 임시 저장 후 이동 가능
    - `git stash` 변경 내역 임시 저장
    - `git stash list` 스택에 저장된 스태시 출력
    - `git stash pop` 변경 내역 다시 불러오기

<br>

# Pull Request
- 완성한 코드를 main 브랜치에 병합하기 전에 코드 리뷰 및 수정 사항 피드백을 받기 위해 요청하는 것
- 원격에서는 못하고 GitHub 웹에서 풀 리퀘 생성 후 리뷰어가 변경 내용 검토하고 승인하면 병합됨

<br>

# Merge
- 로컬 브랜치 간의 변경 사항 병합 후 원격에 푸시
    - `git checkout main` main 브랜치로 이동
    - `git pull origin main` main 브랜치 최신 상태로 업데이트
    - `git merge 다른 브랜치` 다른 브랜치를 (main 브랜치에) 병합
    - `git push origin main` 원격 레포에 main 브랜치 푸시

<br>

# Issue
- 기능 추가
- 버그 수정
- 이 커밋들이 지금 이슈에 해당되는 것들이다

```
태그: 제목
본문
issue: #0
```