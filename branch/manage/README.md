## ๐ ๋ธ๋์น ๊ด๋ฆฌํ๊ธฐ

- ๋ธ๋์น ๋ฆฌ์คํธ

```
git branch
git branch --all #์๋ฒ์ ์๋ ๋ธ๋์น๊น์ง ํ์ธ
git branch -v #๋ธ๋์น ๋ฆฌ์คํธ + ์ต์  ์ปค๋ฐ
git branch --merged #ํ์ฌ ๋ธ๋์น์ merge๋ ๋ธ๋์น ๋ฆฌ์คํธ
git branch --no-merged #ํ์ฌ ๋ธ๋์น์ merge๋ ์ ๋ ๋ธ๋์น ๋ฆฌ์คํธ
```

- ์ญ์ 

```
git branch -d ๋ธ๋์น๋ช
git push origin --delete testing #์๋ฒ ์๊ฒฉ์ ๋ฑ๋ก๋ ๋ธ๋์น๋ ์ญ์ 
```

- ์ด๋ฆ ๋ณ๊ฒฝ

```
git branch --move ๋ณ๊ฒฝ์  ๋ณ๊ฒฝํ
git push --set-upstream origin correct #์ด๋ฆ ๋ณ๊ฒฝํ ์๊ฒฉ์ ๋ฐ์
```
