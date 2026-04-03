# 포트폴리오 디자인 스펙

## 개요

김재현(Jeric)의 개발자 포트폴리오. GitHub README 개선 + Next.js 독립 웹사이트 두 가지로 구성.

- **참고:** silverbeen.dev (Next.js + TypeScript + Tailwind + Framer Motion)
- **기술 스택:** Next.js 14 (App Router) + TypeScript + Tailwind CSS + Framer Motion
- **테마:** 다크/라이트 토글 지원

---

## 웹사이트 구조

### 페이지 흐름 (싱글 페이지, 스크롤)

```
Hero → About → Career → Projects → Contact → Footer
```

상단 고정 헤더: 로고(이름) + About / Career / Projects / Contact 앵커 링크 + 다크/라이트 토글

---

### 섹션별 명세

#### 1. Hero
- 풀스크린(100vh), 중앙 정렬
- 큰 이름: `김재현 / Jeric`
- 타이핑 애니메이션(useEffect + setTimeout): `"Backend Engineer"` → `"IoT Developer"` → `"Full-stack Engineer"` 순환
- 아이콘 링크: GitHub(github.com/jeric1223), 이메일(soehd0889@naver.com), Notion 포트폴리오
- 스크롤 유도 화살표 (bounce 애니메이션)

#### 2. About
- 섹션 제목: "About Me"
- 4개 카드 그리드 (2x2, 모바일 1x4)
- 각 카드: 아이콘 + 제목 + 설명
  - JavaScript 기반 Full-stack 엔지니어
  - 협업 툴 활용 (Jira, Confluence)
  - AWS 클라우드 인프라
  - 다양한 기술 경험
- Framer Motion: 스크롤 진입 시 stagger fade-in

#### 3. Career
- 섹션 제목: "Career"
- 수직 타임라인
- **(주)씨앤테크** (2022.10 ~ 현재, 3년 7개월)
  - 클릭/토글로 펼치기: OneMap, 동산담보 하위 항목 표시
  - 각 프로젝트: 기간 + 역할 요약 태그
- 학력: 대덕소프트웨어마이스터고등학교 (2020.03 ~ 2023.01)
- Framer Motion: 타임라인 라인이 위→아래로 그려지는 애니메이션

#### 4. Projects
- 섹션 제목: "Projects"
- 카드 2개 (세로 배치, 모바일 대응)

**OneMap** (2023.06 ~ 2023.12)
- 개요: IoT 디바이스 센서 모니터링, 차량 관제, 소물 위치 관제 실시간 확인
- 역할 태그: DB설계, 소켓서버, AWS Lambda, 웹소켓, SMS, API서버
- 참여: 백엔드 2인 중 80%

**동산담보** (2022.10 ~ 2025.02)
- 개요: 기업 자산 IoT 모니터링 웹 서비스
- 역할 태그: 유지보수, 성능최적화, 보안이슈해결, 리뉴얼
- hover 시 카드 살짝 위로 이동 (translateY -4px)

#### 5. Contact
- 섹션 제목: "Contact"
- 이메일 복사 버튼 (클릭 시 "복사됨!" 토스트)
- GitHub 링크 버튼
- Notion 포트폴리오 링크 버튼

#### 6. Footer
- 이름 + "© 2026 김재현" + 간단한 기술스택 표기

---

## GitHub README 구조

```markdown
# 김재현 / Jeric
백엔드 개발자, 프론트를 곁들인

🌐 포트폴리오 웹사이트 링크 (배포 후 추가)

## Stack
[기술 뱃지 - 현재와 동일하되 카테고리별로 정리]
Backend / Frontend / DB / Cloud / Tools

## GitHub Stats
github-readme-stats 카드 (어두운 테마)

hits 카운터
```

---

## 기술 결정

| 항목 | 결정 | 이유 |
|------|------|------|
| 프레임워크 | Next.js 14 App Router | SSG로 배포 간편 |
| 스타일링 | Tailwind CSS | 빠른 반응형 구현 |
| 애니메이션 | Framer Motion |  자연스러운 진입 효과 |
| 테마 | next-themes | 다크/라이트 토글 |
| 타이핑 효과 | 직접 구현 (useEffect) | 외부 라이브러리 불필요 |
| 배포 | Vercel | Next.js 최적화, 무료 |

---

## 파일 구조

```
Jeric1223/
├── app/
│   ├── layout.tsx          # 루트 레이아웃, ThemeProvider
│   ├── page.tsx            # 메인 페이지 (섹션 조합)
│   └── globals.css
├── components/
│   ├── layout/
│   │   ├── Header.tsx
│   │   └── Footer.tsx
│   └── sections/
│       ├── Hero.tsx
│       ├── About.tsx
│       ├── Career.tsx
│       ├── Projects.tsx
│       └── Contact.tsx
├── data/
│   └── portfolio.ts        # 프로젝트, 경력 데이터 상수
├── lib/
│   └── utils.ts
├── public/
├── README.md               # GitHub 프로필 README (개선)
└── ...config files
```

---

## 범위 외 (이번 스펙에 미포함)

- 블로그/글쓰기 기능
- 다국어(i18n)
- 백엔드 API (정적 데이터만 사용)
- 애널리틱스 연동
