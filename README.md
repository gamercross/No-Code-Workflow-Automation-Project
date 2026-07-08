<div align="center">

# ⚙️ No-Code Workflow Automation Project
### *Building Smart Business Automation with No-Code Tools*

<img src="https://img.shields.io/badge/Mission-B2--2-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/No--Code-Automation-success?style=for-the-badge">
<img src="https://img.shields.io/badge/Make-violet?style=for-the-badge">
<img src="https://img.shields.io/badge/Zapier-orange?style=for-the-badge">
<img src="https://img.shields.io/badge/GitHub-README-black?style=for-the-badge">
<img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge">

---

### 🚀 AI & No-Code Workflow Automation Project

**Make와 Zapier를 활용하여 동일한 자동화 워크플로우를 구현하고 비교 분석한 프로젝트입니다.**

**반복 업무를 자동화하기 위한 Trigger, Action, Filter 구조를 설계하고,  
실무에 적합한 자동화 파이프라인을 구축하여 업무 효율성을 향상시키는 것을 목표로 했습니다.**

---

### 🎯 Project Objectives

✔️ **동일한 자동화 워크플로우를 2개의 노코드 플랫폼으로 구현**  
✔️ **Trigger · Action · Filter 기반 자동화 구조 설계**  
✔️ **도구별 UI/UX, 기능, 비용, 확장성 비교 분석**  
✔️ **실제 업무를 위한 자동화 파이프라인 설계 및 구현**

---

### 🛠️ Tech Stack

<img src="https://skillicons.dev/icons?i=gmail,discord&theme=light" />

<br>

| Category | Tools |
|----------|-------|
| ⚙️ Automation | **Make**, **Zapier** |
| 📊 Database | **Google Sheets** |
| 📧 Trigger | **Gmail / Google Forms / Webhook** |
| 💬 Notification | **Discord / Slack** |
| 🤖 AI (Bonus) | **ChatGPT API / Claude API** |
| 📄 Documentation | **GitHub README, Markdown** |

---

## 📖 문서 구성

본 README는 아래와 같은 순서로 진행된다.

1. 📌 프로젝트 소개
2. ⚙️ 자동화 개념 이해
3. 🛠️ 프로젝트 1 - 자동화 도구 비교 구현
4. 📊 프로젝트 1 비교 분석
5. 🚀 프로젝트 2 - 자유 주제 자동화 구현
6. 🔍 워크플로우 분석
7. ⭐ 보너스 구현
8. 💡 프로젝트를 통해 배운 점
9. 📚 참고 자료

---

## ⚙️ Chapter 2. 자동화 개념 이해

# 📖 자동화란 무엇인가?

자동화(Automation)는 사람이 반복적으로 수행하는 작업을 시스템이 대신 수행하도록 만드는 기술을 의미한다. 과거에는 이러한 자동화를 구현하기 위해 프로그래밍 언어를 사용하여 직접 코드를 작성해야 했지만, 최근에는 **노코드(No-Code)** 및 **로우코드(Low-Code)** 플랫폼의 발전으로 프로그래밍 경험이 없어도 자동화 시스템을 구축할 수 있게 되었다.

대표적인 노코드 자동화 플랫폼인 **Make**와 **Zapier**는 다양한 서비스를 서로 연결하여 하나의 업무 흐름(Workflow)을 구성할 수 있도록 지원한다. 사용자는 각 서비스를 시각적으로 연결하는 것만으로도 복잡한 자동화 프로세스를 구현할 수 있으며, 반복 업무를 줄이고 업무 효율을 크게 향상시킬 수 있다.

자동화 워크플로우는 일반적으로 **Trigger → 조건 확인 → Action**의 순서로 동작하며, 필요에 따라 여러 개의 조건 분기와 작업을 추가하여 더욱 복잡한 프로세스를 구성할 수 있다.

---

# 🎯 Trigger (시작 이벤트)

## Trigger란?

**Trigger**는 자동화를 시작시키는 이벤트(Event)를 의미한다.

즉, 특정 조건이나 이벤트가 발생하면 자동화 시스템은 이를 감지하고 미리 정의된 워크플로우를 실행하게 된다.

Trigger는 모든 자동화의 시작점이며, Trigger가 발생하지 않으면 이후의 작업(Action)도 실행되지 않는다.

### 💡 대표적인 Trigger 예시

* 📧 Gmail에 새로운 이메일이 도착했을 때
* 📝 Google Form에 새로운 응답이 제출되었을 때
* 📂 Google Drive에 새로운 파일이 업로드되었을 때
* 📄 Google Docs 문서가 생성되었을 때
* 🌐 Webhook으로 외부 요청이 들어왔을 때
* 💬 Slack 또는 Discord에 새로운 메시지가 작성되었을 때

---

## Trigger 동작 과정

```text
이벤트 발생

↓

Trigger 감지

↓

Workflow 실행 시작
```

Trigger는 자동화의 시작 버튼과 같은 역할을 수행하며, 이후 연결된 Action들이 순차적으로 실행된다.

---

# ⚡ Action (실행 작업)

## Action이란?

**Action**은 Trigger가 발생한 이후 실제로 수행되는 작업을 의미한다.

하나의 워크플로우에는 하나 이상의 Action이 포함될 수 있으며, 여러 Action을 순차적으로 연결하여 복잡한 업무를 자동화할 수 있다.

예를 들어 새로운 설문 응답이 제출되었다면,

* Google Sheets에 데이터 저장
* Slack으로 알림 전송
* 이메일 발송

과 같은 여러 작업을 연속적으로 수행할 수 있다.

---

## 💡 대표적인 Action 예시

* 📊 Google Sheets에 새로운 행 추가
* 💬 Slack 채널에 메시지 전송
* 📧 이메일 자동 발송
* 📁 Google Drive에 파일 저장
* 🤖 ChatGPT를 이용한 텍스트 요약
* 📱 Discord 알림 전송

---

## Action 동작 과정

```text
Trigger 발생

↓

Action 1

↓

Action 2

↓

Action 3

↓

자동화 완료
```

Action은 자동화 시스템의 핵심 기능으로, 실제 업무를 대신 수행하는 역할을 한다.

---

# 🔀 Filter (조건 분기)

## Filter란?

**Filter**는 특정 조건을 만족하는 경우에만 다음 단계를 실행하도록 하는 기능이다.

조건을 만족하지 못하면 해당 경로는 실행되지 않고 워크플로우가 종료되거나 다른 경로로 이동한다.

이를 통해 불필요한 작업을 줄이고 필요한 경우에만 자동화를 수행할 수 있다.

---

## Filter 예시

학생들의 시험 점수를 자동으로 처리한다고 가정하면 다음과 같이 구성할 수 있다.

```text
Google Form 제출

↓

점수 확인

↓

점수 ≥ 80점

↓

Slack 합격 알림
```

80점 미만이라면 Slack 알림은 실행되지 않는다.

---

## Filter의 장점

* ✅ 불필요한 작업 실행 방지
* ✅ 조건에 맞는 데이터만 처리
* ✅ 자동화 효율 향상
* ✅ 리소스 절약

---

# 🔀 Router (다중 분기)

## Router란?

**Router**는 하나의 워크플로우를 여러 개의 경로로 나누어 각각 다른 작업을 수행하도록 하는 기능이다.

Make에서는 Router를 사용하여 하나의 Trigger에서 여러 개의 작업 흐름을 동시에 설계할 수 있다.

---

## Router 예시

```text
Google Form 제출

↓

Router

├── 점수 ≥ 80
│      ↓
│   합격 시트 저장
│      ↓
│   Slack 합격 알림
│
└── 점수 < 80
       ↓
   불합격 시트 저장
       ↓
   Slack 재도전 안내
```

이처럼 하나의 Trigger에서도 조건에 따라 서로 다른 자동화 프로세스를 실행할 수 있다.

---

## Router의 장점

* 🔹 복잡한 업무를 하나의 워크플로우에서 처리 가능
* 🔹 여러 조건을 동시에 관리 가능
* 🔹 유지보수가 용이
* 🔹 시각적으로 이해하기 쉬운 구조 제공

---

# 🔄 Trigger · Filter · Router · Action의 관계

자동화 시스템은 일반적으로 다음과 같은 흐름으로 동작한다.

```text
Trigger

↓

Filter 또는 Router

↓

Action

↓

Action

↓

Workflow 종료
```

각 요소는 서로 독립적인 기능이 아니라 하나의 워크플로우 안에서 유기적으로 연결되어 자동화를 완성한다.

---

# 📝 Chapter 정리

이번 Chapter에서는 노코드 자동화의 핵심 구성 요소인 **Trigger**, **Action**, **Filter**, 그리고 **Router**의 개념과 역할을 살펴보았다.

* 🚀 Trigger는 자동화를 시작하는 이벤트이다.
* ⚡ Action은 실제 업무를 수행하는 작업이다.
* 🔀 Filter는 조건에 따라 실행 여부를 결정한다.
* 🌳 Router는 여러 개의 작업 경로를 생성하여 다양한 상황에 대응할 수 있도록 한다.

이러한 개념들은 이후 프로젝트에서 구현할 자동화 워크플로우의 기반이 되며, 각 플랫폼이 이를 어떻게 제공하는지 비교하는 중요한 기준이 된다.

---

## ➡️ 다음 Chapter

이제 자동화의 기본 개념을 이해했으므로, 다음 Chapter에서는 **동일한 워크플로우를 Make와 Zapier에서 각각 구현**하며 두 플랫폼의 구성 방식과 실행 과정을 단계별로 살펴본다.


프로젝트를 진행하기에 앞서, 자동화 도구를 이해하기 위해서는 **Trigger**, **Action**, **Filter**, **Router**와 같은 핵심 개념을 먼저 이해해야 한다.

다음 Chapter에서는 이러한 요소들이 자동화에서 어떤 역할을 수행하며, 실제 워크플로우 안에서 어떻게 활용되는지를 자세히 살펴본다.

---

# 🛠️ Chapter 3. 프로젝트 1 - 자동화 도구 비교 구현

## 📖 프로젝트 개요

자동화 플랫폼마다 제공하는 인터페이스와 기능은 서로 다르지만, 대부분 **Trigger(시작 이벤트)**와 **Action(실행 작업)**을 중심으로 워크플로우를 구성한다는 공통점을 가지고 있다.

이번 프로젝트에서는 이러한 차이점을 객관적으로 비교하기 위해 **동일한 자동화 시나리오를 두 개의 플랫폼(Make, Zapier)에서 각각 구현**하였다.

동일한 기능을 구현하면서 각 플랫폼의 설정 방식, 조건 분기 방법, 실행 과정, 그리고 사용자 경험(UI/UX)의 차이를 직접 확인하는 것이 이번 프로젝트의 핵심 목표이다.

---

# 🎯 구현 목표

이번 프로젝트에서는 다음과 같은 목표를 설정하였다.

* ✅ 동일한 자동화 워크플로우를 두 개 이상의 플랫폼에서 구현한다.
* ✅ Trigger, Action, 조건 분기(Filter/Router)를 모두 포함한다.
* ✅ 실제 동작하는 자동화 환경을 구축한다.
* ✅ 플랫폼별 설정 과정과 실행 결과를 비교 분석한다.

---

# 📝 자동화 시나리오

이번 프로젝트에서 구현한 자동화 워크플로우는 다음과 같다.

> **Google Form에 새로운 응답이 제출되면 점수를 확인하고, 조건에 따라 Google Sheets에 저장한 후 Slack으로 결과를 전송하는 자동화 시스템**

해당 시나리오는 실제 설문 조사, 시험 결과 관리, 지원자 평가 등 다양한 업무에서 활용할 수 있는 대표적인 자동화 사례이다.

---

# 🔄 전체 워크플로우

```text
Google Form 제출

        │
        ▼
Trigger 발생

        │
        ▼
점수 확인

        │
        ▼
조건 분기

 ┌──────────────┴──────────────┐
 │                             │
 ▼                             ▼
80점 이상                  80점 미만

 │                             │
 ▼                             ▼
합격 시트 저장             불합격 시트 저장

 │                             │
 ▼                             ▼
Slack 합격 알림          Slack 재도전 안내
```

이번 워크플로우는 다음과 같은 요소를 모두 포함한다.

| 구성 요소      | 설명                 |
| :--------- | :----------------- |
| 🚀 Trigger | Google Form 응답 제출  |
| 🔀 조건 분기   | 점수 기준(80점 이상 / 미만) |
| ⚡ Action 1 | Google Sheets 저장   |
| ⚡ Action 2 | Slack 메시지 전송       |

---

# ⚙️ Make 구현

## 📌 구현 방식

Make는 **노드(Node) 기반의 시각적인 인터페이스**를 제공한다.

각 서비스를 하나의 모듈(Module)로 연결하며, Router를 이용하여 하나의 흐름을 여러 개의 경로로 분기할 수 있다.

이번 구현에서는 아래와 같은 순서로 워크플로우를 구성하였다.

```text
Google Forms

↓

Router

├── 합격
│
├── Google Sheets
│
└── discord

불합격

├── Google Sheets

└── discord
```

---

## 🚀 Trigger

사용한 Trigger

> Google Forms - Watch Responses

새로운 응답이 제출되는 즉시 워크플로우가 실행되도록 설정하였다.

📷 **전체 구현 화면**

<img width="1393" height="490" alt="화면 캡처 2026-07-08 171054" src="https://github.com/user-attachments/assets/aa4aa8e8-a70a-43c4-b2d5-03894dae530f" />

---

## 🔀 Router

Make의 Router 기능을 이용하여 점수에 따라 두 개의 경로를 생성하였다.

* ✔️ 80점 이상
* ✔️ 80점 미만

각 경로에는 서로 다른 Action이 연결되어 있다.

📷 **Router 설정 화면**

<img width="479" height="613" alt="화면 캡처 2026-07-08 171227" src="https://github.com/user-attachments/assets/af5960ad-199e-4887-91c4-dc0621ef8bac" />

---

## ⚡ Action 1

Google Sheets

* 새로운 행 추가
* 점수 저장
* 응답 시간 저장

📷 **Google Sheets 설정 화면**

<img width="452" height="844" alt="화면 캡처 2026-07-08 171557" src="https://github.com/user-attachments/assets/db8f0296-b3e9-4d00-8bdf-7d7e19f175d2" />

---

## ⚡ Action 2

discord

* 회의록 요약 보고서

📷 **discord 설정 화면**

<img width="457" height="929" alt="화면 캡처 2026-07-08 172030" src="https://github.com/user-attachments/assets/15368cd9-f33c-4ff3-970c-b22c8a5ccbf6" />

---

## ✅ 실행 결과

Google Form을 제출하자 Make가 자동으로 실행되었으며,

* Router에서 조건을 판별하고
* Google Sheets에 데이터를 저장한 뒤
* discord으로 결과를 전송하는 것을 확인하였다.

📷 **실행 로그**

<img width="434" height="632" alt="화면 캡처 2026-07-08 171346" src="https://github.com/user-attachments/assets/69af4ae1-d8af-4c15-abde-ad71d5a440bf" />

📷 **discord 결과**

<img width="414" height="480" alt="화면 캡처 2026-07-08 171742" src="https://github.com/user-attachments/assets/16fb5f57-6a00-4a20-95f6-de7512b44586" />

📷 **Google Sheets 결과**

<img width="1272" height="759" alt="화면 캡처 2026-07-08 171936" src="https://github.com/user-attachments/assets/add48d79-b674-43d8-bae9-e40e70d004c7" />

---

# ⚡ Zapier 구현

## 📌 구현 방식

Zapier는 **리스트(List) 기반 인터페이스**를 제공하며, 단계별로 Trigger와 Action을 추가하는 방식으로 워크플로우를 구성한다.

조건 분기는 Filter를 이용하여 구현하였다.

전체 흐름은 다음과 같다.

```text
Google Forms

↓

Filter

↓

Google Sheets

↓

Discord
```

---

## 🚀 Trigger

사용한 Trigger

> Google Forms - New Response in Spreadsheet

새로운 응답이 등록되면 자동으로 실행되도록 설정하였다.

📷 **전체 설정 화면**

<img width="668" height="776" alt="화면 캡처 2026-07-08 172204" src="https://github.com/user-attachments/assets/73a242ac-687f-4d08-9a41-e57a1661359b" />

---

## 🔀 Filter

Zapier의 Filter 기능을 이용하여

조건

```
점수 ≥ 80
```

인 경우에만 이후 Action이 실행되도록 구성하였다.

📷 **Filter 설정 화면**

<img width="408" height="791" alt="화면 캡처 2026-07-08 172309" src="https://github.com/user-attachments/assets/e6116f3f-35f5-4822-8fd3-c8481522cf2c" />

---

## ⚡ Action 1

Google Sheets

* 새로운 행 생성
* 점수 저장
* 응답 시간 기록

📷 **스크린샷 삽입**

<img width="423" height="800" alt="화면 캡처 2026-07-08 172400" src="https://github.com/user-attachments/assets/5b43a7d7-2705-4d48-8009-94f0fab014b6" />

---

## ⚡ Action 2

Discord

* 회의 요약 메시지 자동 전송

📷 **스크린샷 삽입**

<img width="405" height="790" alt="화면 캡처 2026-07-08 172458" src="https://github.com/user-attachments/assets/c70af390-8422-4663-9337-085b126f7947" />

---

## ✅ 실행 결과

테스트 응답을 제출한 결과

* Trigger가 정상적으로 실행되었으며
* Filter 조건을 통과한 데이터만
* Google Sheets와 Slack으로 전달되는 것을 확인하였다.

📷 **Task History**

<img width="424" height="813" alt="화면 캡처 2026-07-08 172558" src="https://github.com/user-attachments/assets/e3e3c5f4-1755-4ea4-b6d9-2f399465058f" />

📷 **Discord 결과**

<img width="1529" height="566" alt="화면 캡처 2026-07-08 172706" src="https://github.com/user-attachments/assets/a5d1624f-1e0c-47f8-8b71-17ddf59218fd" />

📷 **Google Sheets 결과**

<img width="1272" height="759" alt="화면 캡처 2026-07-08 171936" src="https://github.com/user-attachments/assets/39dbeec5-b374-4c0a-96b2-cb4487b1ccb8" />

---

# 📌 프로젝트 1 구현 결과

이번 프로젝트에서는 동일한 자동화 시나리오를 **Make**와 **Zapier**에서 모두 성공적으로 구현하였다.

두 플랫폼 모두 Trigger와 Action을 기반으로 자동화를 구성할 수 있었지만, 조건 분기를 구현하는 방식과 워크플로우를 설계하는 인터페이스에는 차이가 있었다.

이러한 차이는 자동화의 복잡도, 유지보수 편의성, 그리고 사용자의 학습 난이도에도 영향을 미치는 요소였다.

---

## ➡️ 다음 Chapter

이번 Chapter에서는 동일한 자동화를 두 플랫폼에서 구현하는 과정을 살펴보았다.

다음 Chapter에서는 **Make와 Zapier를 다양한 관점에서 비교 분석**하여 UI/UX, 설정 난이도, 무료 플랜, 실행 로그, 연동 서비스, 장단점 등을 종합적으로 평가하고, 어떤 상황에서 각각의 플랫폼이 적합한지 살펴본다.


---
> **"Automate repetitive tasks, focus on meaningful work."**

**No-Code Workflow Automation with Make & Zapier**

</div>
