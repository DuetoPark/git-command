## 🤔 파일 상태 확인

```
> git status
```

- untracked 파일은 빨간색으로 표시
- tracked 파일은 초록색으로 표시

  <img width="479" alt="스크린샷 2022-05-19 오후 3 51 15" src="https://user-images.githubusercontent.com/69448900/169228754-c365f2b9-6624-4623-9559-8d1d79165a52.png">

## 🔨 파일 stage area로 이동

### 새 파일

```
> git add 파일명
```

- 여러개의 파일을 동시에 올리고 싶은 경우, 띄어쓰기로 구분
- 동일한 확장자를 모두 올리고 싶은 경우, `*.확장자` 입력

  ```
  > git add *.txt
  ```
  
  <img width="478" alt="스크린샷 2022-05-19 오후 3 54 20" src="https://user-images.githubusercontent.com/69448900/169229323-33a684a7-20b0-4cc3-8693-f6d608255781.png">
  <img width="487" alt="스크린샷 2022-05-19 오후 3 54 34" src="https://user-images.githubusercontent.com/69448900/169229341-a844de9e-4b49-40b9-b596-9fa86b5a9d1f.png">

### 수정된 파일
- 파일 수정하면, tracked 파일의 상태가 'modified'로 변경된다.

  <img width="484" alt="스크린샷 2022-05-19 오후 3 59 23" src="https://user-images.githubusercontent.com/69448900/169230167-67f12039-bd62-47ac-9dc5-76d2f177d65f.png">

  ```
  - add된 파일 = commit될 준비가 끝남, stage area에 위치
  - 'modified' 상태의 파일 = 그저 수정이 된 상태, working directory에 위치
  ```
- 수정이 끝난 파일을 add하여 stage area로 이동

  ```
  > git add 파일명
  ```
  
  <img width="482" alt="스크린샷 2022-05-19 오후 4 05 44" src="https://user-images.githubusercontent.com/69448900/169231228-d2d973f7-1588-4add-ba97-57cb929f0b8c.png">

## 🙊 working directory로 이동

```
> git rm --cached 파일명
```

<img width="484" alt="스크린샷 2022-05-19 오후 4 07 04" src="https://user-images.githubusercontent.com/69448900/169231552-9e346ce4-874e-416b-bd4e-5b634fe5aad5.png">
