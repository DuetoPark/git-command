## ๐  ๋ก์ปฌ ์ํฉ ๋ณ๊ฒฝ

### ์ํผ์ ์ง๊ถ๋์ด

1. ํด๋น ๋ธ๋์น๋ฅผ `ํผ์` ์์์ค์ผ ๊ฒ
2. ์์๋ฌผ์ด `์๊ฒฉ ์๋ฒ`์ push ๋์ด์์ง ์์ ๊ฒ

### staged area์์ ๋ด๋ฆฌ๊ธฐ

๋ง์ฝ, ํด๋น ํ์ผ์ด ์์ฑ๋๊ธฐ ์ ์ ์ปค๋ฐ ์ํ๋ก ๋๋๋ฆฌ๋ฉด ๊ทธ ํ์ผ์ ์ญ์ ๋๋ค.

```
git restore --staged file.txt
git reset HEAD file.txt
git restore --source=hash file.txt #file.txt๋ฅผ hash์ฃผ์์ ์ปค๋ฐ ์ํ๋ก ๋๋๋ฆฌ๊ธฐ
git restore --source=HEAD~2 file.txt #file.txt๋ฅผ ํ์ฌ ํค๋๋ก๋ถํฐ 2๊ฐ ์ ์ ์ปค๋ฐ ์ํ๋ก ๋๋๋ฆฌ๊ธฐ
```

### discard ํ๊ธฐ(modified ๋ด์ฉ ๋๋๋ฆฌ๊ธฐ)

```
git restore file.txt
git restore . #working directory ์์ ๋ชจ๋  ํ์ผ discard
```

### untracked(staged area์ ๋ชป ์ฌ๋ผ๊ฐ ํ์ผ๋ค)

```
git clean -fd
```
