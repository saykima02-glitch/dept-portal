# 부서포털 사용법

## 폴더 구조

```
부서포털/
├── index.html                          # 포털 메인 페이지 (구 recruit.html)
├── files/                               # 첨부 자료 (PDF 등)
│   ├── recruitment-notice-2026-h1.pdf   # 채용공고 (2026년 상반기)
│   └── culture-and-values-guide.pdf     # 인재상·조직문화 소개서
└── 이전버전/
    └── recruit.html                     # 이름 변경 전 원본 사본
```

## 열어보는 방법

1. `index.html` 파일을 더블클릭하면 기본 웹 브라우저에서 포털이 열립니다.
2. 상단 메뉴(홈 / 채용 절차 / 직무 소개 / FAQ / 자료실)를 클릭하면 해당 섹션으로 이동합니다.
3. "자료실" 섹션에서 채용공고와 인재상·조직문화 소개서 PDF를 바로 열어볼 수 있습니다.

## 파일 관리 규칙

- 새로운 PDF·Word 자료는 `files` 폴더에 넣고, 파일명은 **영문 소문자 + 하이픈(-)** 조합으로 작성합니다 (예: `onboarding-guide.pdf`). 한글이나 공백이 들어간 파일명은 링크가 깨질 수 있으니 피해 주세요.
- 자료를 추가했다면 `index.html`의 "자료실" 섹션에 아래와 같은 형식으로 링크를 추가해 주세요.

  ```html
  <a href="files/새파일명.pdf" target="_blank" rel="noopener">📄 자료 제목</a>
  ```

- `index.html`을 수정하기 전에 이전 버전을 보관하고 싶다면 `이전버전` 폴더에 사본을 먼저 복사해 두세요.

## 변경 이력

- `recruit.html` → `index.html`로 이름 변경 (원본 사본은 `이전버전/recruit.html`에 보관)
- `채용공고_2026년_상반기.pdf` → `files/recruitment-notice-2026-h1.pdf`
- `인재상_조직문화_소개서.pdf` → `files/culture-and-values-guide.pdf`
- `index.html`의 "자료실" 섹션에 두 PDF 링크 추가
