# ebook-landing

전자책 「비전공자도 됩니다」의 판매 랜딩 페이지.

Threads 등에서 유입된 방문자가 도착하는 착지점이다. 무료 샘플(29쪽)을
조건 없이 내려받거나, 구매 채널로 넘어가는 두 가지 동선만 가진다.

## 구성

```
ebook-landing/
├── index.html   랜딩 페이지 본체 (단일 파일, CSS 인라인, 외부 의존성 없음)
├── sample.pdf   무료 샘플 (본편 287쪽 중 29쪽, Part 1 전체 + 1주차 첫 챕터)
├── assets/cover.png  표지 이미지
└── README.md    이 파일
```

`index.html`은 정적 파일이라 별도 빌드 과정이 없다. 아무 정적 호스팅
(GitHub Pages, Vercel, Netlify 등)에 두 파일(`index.html`, `sample.pdf`)만
올리면 바로 동작한다.

## 배포

이 레포는 `ebook-ai-dev-job`(책 본문 저장소)과 분리되어 있다. 본문이
갱신되어도 이 레포는 영향받지 않으며, 샘플 PDF를 교체할 때만 수동으로
`sample.pdf`를 다시 복사해 넣는다.

## 구매 채널 링크를 바꾸는 곳

`index.html`에서 `id="buy"` 섹션의 구매 버튼 `href`를 실제 구매 링크로
바꾸면 된다. 카피 톤·문구 원칙은 비공개 저장소에 별도로 정리되어 있다.
