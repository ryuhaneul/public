# public — 류하늘 웹게임 갤러리

GitHub Pages 허브.

- 갤러리: https://ryuhaneul.github.io/public/
- 예시 게임: https://ryuhaneul.github.io/public/magical-lumi/

## 구조

```
/
  index.html           # 갤러리 (GAMES 배열)
  magical-lumi/        # 게임 1
    index.html
    assets/
  <next-slug>/         # 이후 게임
```

## 게임 추가

1. 폴더 `slug/` 만들고 `index.html` (+ 에셋) 배치
2. 루트 `index.html` 의 `GAMES` 배열에 항목 추가:

```js
{
  id: 'slug',
  title: '제목',
  subtitle: '한 줄 설명',
  href: './slug/',
  cover: './slug/cover.png',
  tags: ['장르'],
  accent: '#ffcf5c',
  badge: 'NEW', // 선택
}
```

3. `main` 에 push → Pages 자동 반영

## 로컬

```bash
python3 -m http.server 8080
# http://localhost:8080/
```

## 라이선스

개인·비상업 공개. AI 생성 일러스트 포함 가능.
