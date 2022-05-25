## ✂️ 커밋 쪼개기

1. 커밋 rebase 실행
    
    ```bash
    git rebase -i 해쉬코드(원하는 코드 바로 전 해쉬코드)
    ```
    
2. commit reset하기
    
    ```bash
    git reset HEAD~1
    ```
    
3. add(staged area에 보내기) + commit(히스토리 남기기)로 커밋 분할
4. rebase —continue

→ history로 틈틈히 확인할 땐 브랜치가 분리된 것처럼 보이는데, rebase로 합치면 ff되어 있음.
