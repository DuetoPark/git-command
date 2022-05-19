## 🗂 파일 이름 바꾸기

- shell command
  
  ```
  > mv 파일명 바꿀파일명
  ```
  
  파일명이 변해도 해당 사항은 stage되지 않는다.
  
  <img width="488" alt="스크린샷 2022-05-19 오후 6 08 36" src="https://user-images.githubusercontent.com/69448900/169257992-a6c0dd90-e823-4397-9dd6-e6682e13f604.png">


- git command
  
  ```
  > git mv 파일명 바꿀파일명
  ```
  
  파일명이 변한 내용이 stage 된다.
  
  <img width="489" alt="스크린샷 2022-05-19 오후 6 08 15" src="https://user-images.githubusercontent.com/69448900/169257871-12017c95-c50c-414f-a175-6e10fdcda952.png">
  
## 📑 파일 삭제

- shell command

  ```
  > rm 파일명
  ```
  
  파일을 삭제한 내역이 stage에 반영되지 않는다.
  
  <img width="485" alt="스크린샷 2022-05-19 오후 6 15 59" src="https://user-images.githubusercontent.com/69448900/169258966-15f607ab-5cad-488c-b3cb-fd1311b0a8cf.png">


- git command

  ```
  > git rm 파일명
  ```
  
  파일 삭제한 내역이 stage에 반영된다.
  
  <img width="489" alt="스크린샷 2022-05-19 오후 6 16 08" src="https://user-images.githubusercontent.com/69448900/169258984-1707f55a-233e-4fef-b50a-7993e1874277.png">
