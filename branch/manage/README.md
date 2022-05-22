## 🚀 브랜치 관리하기

- 브랜치 리스트

```
git branch
git branch --all #서버에 있는 브랜치까지 확인
git branch -v #브랜치 리스트 + 최신 커밋
git branch --merged #현재 브랜치에 merge된 브랜치 리스트
git branch --no-merged #현재 브랜치에 merge된 안 된 브랜치 리스트
```

- 삭제

```
git branch -d 브랜치명
git push origin --delete testing #서버 원격에 등록된 브랜치도 삭제
```

- 이름 변경

```
git branch --move 변경전 변경후
git push --set-upstream origin correct #이름 변경후 원격에 반영
```
