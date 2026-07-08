# 자동화 도구 비교 분석 보고서

1. 보고서 개요

2. 비교 대상

3. 비교 환경

4. 동일 Workflow 소개

5. 세부 비교

6. 프로젝트 적용 결과

7. 결론

---

# 📖 보고서 개요

본 보고서는 동일한 자동화 Workflow를 Make와 Zapier에서 각각 구현한 뒤,
두 플랫폼의 특징과 차이점을 분석하기 위해 작성하였다.

비교는 단순히 기능 유무를 확인하는 것이 아니라

- 구현 과정
- 사용성
- 유지보수성
- 확장성
- 무료 플랜
- 실행 로그

등 실제 프로젝트에서 영향을 주는 요소를 중심으로 진행하였다.

이를 통해 프로젝트에 적합한 자동화 플랫폼을 선정하는 기준을 도출하는 것을 목표로 한다.

---

# 🔧 비교 환경

운영체제

- Windows 11

브라우저

- Chrome

자동화 플랫폼

- Make
- Zapier

연동 서비스

- Google Forms
- Google Sheets
- 제미나이
- Discord

테스트 횟수

- Make : 5회 이상

- Zapier : 5회 이상

---

| 비교항목    | Make              | Zapier       | 프로젝트 영향                     |
| ------- | ----------------- | ------------ | --------------------------- |
| UI      | ⭐⭐⭐⭐⭐             | ⭐⭐⭐⭐         | Workflow가 길어질수록 Make가 보기 편함 |
| 설정 난이도  | 중                 | 쉬움           | 초기 학습은 Zapier가 쉬움           |
| 무료 플랜   | 1000 Ops          | 100 Tasks    | 장기 사용은 Make 유리              |
| 조건 분기   | Router            | Filter       | 프로젝트2에서 Router 선택 이유        |
| 로그      | Execution History | Task History | 디버깅은 Make가 편리               |
| 데이터 처리  | Iterator 지원       | 제한적          | 대량 데이터는 Make                |
| Webhook | 강력                | 보통           | API 연동은 Make                |
| AI 연동   | 쉬움                | 보통           | ChatGPT 사용 시 Make 유리        |

---

## UI 비교

Make는 Node 기반 인터페이스를 제공하여 전체 Workflow를 하나의 화면에서 확인할 수 있었다.

이번 프로젝트에서는

Google Form

↓

Router

↓

Sheets

↓

Discord

구조를 사용하였는데

모든 연결 관계를 한눈에 볼 수 있었다.

반면 Zapier는 리스트 기반으로 표현되기 때문에

Workflow가 길어질수록 이전 단계를 확인하기 위해 스크롤을 반복해야 했다.

따라서

5단계 이하 Workflow에서는 큰 차이가 없었지만

10단계 이상에서는 Make가 훨씬 관리하기 쉬웠다.

---

# 프로젝트 적용 결과

비교 결과

프로젝트2에서는 Make를 선택하였다.

그 이유는

① Router

회의록

↓

AI

↓

결정사항

↓

Discord

↓

Sheets

처럼 분기가 존재하였다.

Router를 사용하는 Make가 구조를 훨씬 보기 쉬웠다.

② Execution History

AI 결과를 단계별로 확인할 수 있어

Prompt 수정이 매우 편리하였다.

③ 무료 플랜

프로젝트 규모에서는 Make의 무료 사용량이 충분하였다.

따라서

이번 프로젝트에는 Make가 더욱 적합하다고 판단하였다.

---

# 결론

Make와 Zapier 모두 반복 업무 자동화를 수행할 수 있는 우수한 플랫폼이었다.

그러나

단순한 개인 업무 자동화는

Zapier가 더 적합하였다.

반대로

여러 개의 조건 분기

AI 연동

Webhook

복잡한 Workflow

에서는 Make가 더욱 효율적이었다.

이번 프로젝트는 AI 요약, 조건 분기, Google Sheets 저장, Discord 전송 등 여러 개의 모듈을 포함하고 있었기 때문에 Make를 선택하였다.

향후 Workflow가 더욱 복잡해질수록 이러한 차이는 더욱 커질 것으로 판단된다.
