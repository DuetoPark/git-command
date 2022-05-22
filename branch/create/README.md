## 🌲 브랜치 생성/이동

- 생성

```
git branch 브랜치명
```

- 이동

```
git checkout 브랜치명 (구버전)
git switch 브랜치명 (신버전)
```

- 생성 & 이동

```
git checkout -b testing
git switch -C testing
```

### checkout과 switch의 차이

- checkout은 switch과 restore 기능이 합쳐진 명령어다.
- checkout은 hash를 이용한 head 이동이 가능하다.
- switch는 브랜치의 이동만을 제공한다.
