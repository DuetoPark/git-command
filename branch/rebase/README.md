## 🚧 커밋 재정비

> 다른 브랜치의 일부를 떼어다가 fast-forward 한다.

### 필요성

- 3-way
- 내가 000 기능에서 000-ui를 작업중인데, 000 이 너무 오래걸림
- 근데, 000-ui는 먼저 가져다 써야 하는 경우

⇒ 000-ui를 먼저 커밋으로 올려서 써야하므로, master 브랜치에 붙여줘야함. 이런 경우에 rebase를 사용

### 영혼의 짝궁뎅이

1. 해당 브랜치를 `혼자` 작업중일 것
2. 작업물이 `원격 서버`에 push 되어있지 않을 것

### 방법

실행 위치: rebase를 원하는 브랜치

1. fast-forward 하고싶은 브랜치로 이동

    ```
    git switch 브랜치명
    ```  

2. rebase 실행  
    rebase를 원하는 브랜치에 해야함

    ```
    git rebase master
    ```

3. master 브랜치로 이동

    ```
    git switch master
    ```

4. merge 실행

    ```
    git merge 브랜치명
    ```

### 방법 - --onto 옵션

❓ 이게 뭐냐면, 부모 브랜치의 내용은 가져오지 않고 자식 브랜치의 내용만을 가져오고 싶을 때 사용하는 옵션임.  
🌟 실행 위치: master 브랜치

1. master 브랜치로 이동

    ```
    git switch master
    ```  

2. rebase 실행 

    ```
    git rebase --onto master 갈라진_브랜치 붙일_브랜치
    ```
    
    - 갈라진 브랜치 ⇒ rebase 실행할 브랜치의 부모 브랜치
    - 붙일 브랜치 ⇒ rebase를 실행할 브랜치

3. merge 실행

    ```
    git merge 브랜치명
    ```
