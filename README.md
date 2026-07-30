# public — 류하늘 웹게임 갤러리

GitHub Pages 허브. **에이전트/작업자용 구조·추가 방법은 이 README를 본다.** 갤러리 UI(`index.html`)에는 레포 구조/경로 설명을 넣지 않는다.

- 갤러리: https://ryuhaneul.github.io/public/
- 게임 예: https://ryuhaneul.github.io/public/magical-lumi/ · https://ryuhaneul.github.io/public/magical-ryuhaneul/

## 구조

```
/
  index.html              # 갤러리 (GAMES 배열만 편집)
  README.md               # 이 파일 (작업 지침)
  magical-lumi/           # 게임
    index.html
    assets/
  magical-ryuhaneul/
    index.html
    assets/
  <next-slug>/            # 이후 게임
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
  cover: './slug/assets/art.normal.png', // 또는 전용 커버
  tags: ['장르'],
  accent: '#ffcf5c',
  badge: 'NEW', // 선택
}
```

3. `main` 에 push → Pages 자동 반영 (branch `main` / root)

## 로컬

```bash
python3 -m http.server 8080
# http://localhost:8080/
```

## 라이선스

개인·비상업 공개. AI 생성 일러스트 포함 가능.
