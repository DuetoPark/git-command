## 👉 병합하기 👈

### fast-forward

- 새로운 브랜치로 생성한 커밋을 그대로 두고, `merge` + `head` 이동해서 커밋을 깨끗하게 병합하는 방법
- 커밋 메세지가 깨끗하게 병합됨(merge history 안 남음)
- 마치 한 사람이 꾸준히 작업한 것처럼 보인다.
- 작업을 마치면 브랜치를 삭제한다.

### 명령어 - fast-forward

```
git merge featureA
```

- featureA의 모든 커밋을 현재 브랜치로 병합

### 명령어 - fast-forward-X

```
git merge --no-ff featureA
```

- merge 히스토리가 남는다.

### 그 외

```
🌟 git merge --continue #conflict 해결 후 merge 진행
```

```
git merge --abort #merge 취소
```

```
git mergetool #mergetool 열기
```
