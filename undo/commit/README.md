## 🥕 커밋 되돌리기

### 영혼의 짝궁뎅이

1. 서버에 올리지 않은 커밋
2. 혼자서 브랜치를 관리

### 최신 커밋 되돌리기 (--amend)

```
git commit --amend
```

- 최신 커밋을 수정할 수 있다.
- 커밋 메세지를 유지한 채, 새로운 파일을 add 할 수 있다.

### 커밋/작업파일 되돌리기 (reset)

```
git reset --soft HEAD
git reset --mixed HEAD
git reset --hard HEAD
```

- 커밋 초기화
- `--mixed`: 히스토리에서 커밋은 사라지지만, 작업 파일은 working directory에 옮겨짐
- `--soft`: 히스토리에서 커밋이 사라짐, 작업 파일은 staged area에 있음 (커밋 다시하기~)  
    명령 순서는 `git reset —soft HEAD~1` → `git commit -m “커밋 메세지”`
- `--hard`: 커밋과 작업파일 완전 삭제🔥 주의해서 사용할 것!!!

### 실수로 `reset --hard`한 내역 되돌리기 (reflog)

```
git reflog
git reset --hard 되돌리고싶은hash
```

- reflog: reference log, 지금까지의 명령한 내역이 저장되어 있음

### 과거의 작업 내역을 삭제 (revert)

```
git revert hash
git revert HEAD~1 
git revert --no-commit hash #revert 커밋 없이 실행
```

- **이미 만들어 놓은 기능에 큰 이슈나 버그가 발생해서 해당 작업 내용을 삭제해야하는 경우**
- revert 커밋이 생성된다.
- 해상 해쉬코드의 변경 사항을 모두 취소하고 `이전 상태`로 되돌린다.
- master 브랜치에 치명적 || 히스토리에 남기고 싶다 ⇒ reset(히스토리 수정)이 아니라 revert(히스토리 유지)하자
