## 🐻 Interactive Rebasing

- 해당 커밋부터 새로운 커밋으로 업데이트 된다.
- conflict 주의!
- 내가 **수정하고 싶은 해쉬코드 바로 전 해쉬코드**부터 시작해야 함
- i 옵션 까먹지 마ㅠㅠ
- r: 커밋 수정
- d: 커밋 삭제 (git rebase -i 해쉬코드→ 옵션 수정 → git rebase —continue)
- e: 해당 커밋 작업할거고, 작업 내용도 바꿀거야

```
git rebase -i HEAD~2
git rebase --continue #rebase 이어서 실행 (conflict 등을 대응한 뒤)
git rebase --abort #rebase 취소
```
