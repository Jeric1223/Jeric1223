<div align="center">

# 김재현 · Jeric

**백엔드 개발자입니다.** IoT 센서 데이터를 다루는 일을 하고 있고,<br/>
요즘은 **AI 에이전트가 실제로 일하게 만드는 도구**를 만들고 있습니다.

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Jeric1223)
[![Velog](https://img.shields.io/badge/Velog-20C997?style=flat-square&logo=velog&logoColor=white)](https://velog.io/@hoohoo0889)
[![npm](https://img.shields.io/badge/npm-CB3837?style=flat-square&logo=npm&logoColor=white)](https://www.npmjs.com/package/@soehd0889/tossinvest-mcp)

</div>

---

## 요즘 만드는 것

AI 에이전트에게 부족한 건 두 가지라고 생각합니다 — **무엇을 할 수 있는지(도구)**, 그리고 **어떻게 해야 하는지(절차)**. 요즘은 그 둘을 채우는 쪽을 만들고 있습니다.

### [tossinvest-mcp](https://github.com/Jeric1223/tossinvest-mcp) — 에이전트에게 *능력*을 준다

Claude에서 토스증권 계좌로 국내·미국 주식을 조회하고 주문하는 **MCP 서버**. 시세·호가·체결·차트·투자자 수급·보유 종목·환율을 읽고, 사용자 확인 절차를 거쳐 일반 주문과 SINGLE·OCO·OTO 조건주문을 등록합니다.

돈이 오가는 도구라 **주문 전 확인 절차를 프로토콜에 넣었습니다.** 에이전트가 혼자 체결하지 못합니다.

`TypeScript` · [npm에 배포](https://www.npmjs.com/package/@soehd0889/tossinvest-mcp) — 월 500+ 다운로드

### [my-claude-skills](https://github.com/Jeric1223/my-claude-skills) — 에이전트에게 *판단 기준*을 준다

반복 작업의 순서·형식·검증 기준을 `SKILL.md`로 문서화한 **Claude Code 플러그인 마켓플레이스**. 한 번 쓰고 버리는 프롬프트 대신, 다음에도 같은 품질이 재현되게 만드는 것이 목적입니다.

정착한 규칙은 넷입니다. **시효성 있는 사실은 검색으로 검증하고 못 찾으면 "확인 필요"로 남깁니다** / **날짜 계산은 LLM에 맡기지 않습니다** / **출력 형식은 템플릿으로 강제합니다** / **모호하면 넘겨짚지 않고 묻습니다.**

[**등록된 스킬 둘러보기 →**](https://my-claude-skills-site.vercel.app) · 사이트는 [my-claude-skills-site](https://github.com/Jeric1223/my-claude-skills-site) (`Next.js` `TypeScript` `Tailwind`)

### [타슈 최적 경로 찾기](https://github.com/Jeric1223/TASHU-OPTIMAL-ROUTE-FINDER) — 대전 공공자전거

출발지와 도착지를 넣으면 가까운 타슈 정류소를 찾아 최적 경로를 안내하는 **PWA**. 실시간 대여 가능 수량을 표시합니다. 제가 쓰려고 만들었고, **서버 비용 0원**으로 운영하고 있습니다.

`React` `TypeScript` `Leaflet` · [**데모 →**](https://jeric1223.github.io/TASHU-OPTIMAL-ROUTE-FINDER/)

---

## 회사에서 하는 일

**(주)씨앤테크** · 2022.10 ~ 현재 · 백엔드

| 프로젝트 | 기간 | 한 일 |
| :--- | :--- | :--- |
| **동산담보** | 2022.10 ~ 현재 | 기업 자산 IoT 모니터링 웹 서비스. 유지보수, 성능 최적화, 보안 이슈 해결, 리뉴얼 |
| **OneMap** | 2023.06 ~ 2023.12 | IoT 센서 모니터링 · 차량/소물 위치 관제 실시간 서비스. DB 설계, 소켓 서버, 웹소켓, AWS Lambda, SMS, API 서버 — 백엔드 2인 중 80% 담당 |

대덕소프트웨어마이스터고등학교 졸업 (2020.03 ~ 2023.01)

---

## 스택

**Language**<br/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=black" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white" />

**Backend**<br/>
<img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" /> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=Express&logoColor=white" /> <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />

**Frontend**<br/>
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black" /> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white" /> <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />

**Database & Cloud**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" /> <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" /> <img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white" />
