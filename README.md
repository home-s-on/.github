# 🏡 HOME'S ON

## 프로젝트 소개

### 집안일 분담 관리 플랫폼, HOME’S ON

HOME’S ON은 가족 또는 룸메이트와 함께 집안일을 체계적으로 관리할 수 있도록 지원하는 플랫폼입니다.  
앱을 통해 언제 어디서나 쉽게 접근할 수 있으며, AI 챗봇, 자동화된 할일 관리, 푸시 알림 등의 기능을 통해 보다 효율적인 집안일 분담을 돕습니다.

## ⏱️ 개발기간

- 2024.11 ~ 2024.12 (5w)

## 👥 팀원 소개

![Image](https://github.com/user-attachments/assets/8298fc2d-f741-4333-ae8a-79b74a950f1a)

## 📌 주요 기능

- **할일 목록**: 모든 멤버가 함께 볼 수 있는 집안일 리스트
- **나의 할일**: 개인별 할당된 집안일 확인 가능
- **맞춤형 할일 추가**: 필요에 따라 직접 할일 추가
- **멤버 초대**: 함께 집안일을 관리할 멤버 초대
- **AI 챗봇 지원**: OpenAI ChatGPT를 활용한 집안일 관련 질문 응답
- **주간 리뷰 AI**: 주간 집안일 수행률 분석 및 동기부여 메시지 제공
- **Apple Push 알림**: 중요한 일정 및 할일을 놓치지 않도록 푸시 알림 지원
- **SNS 로그인**: 카카오, 애플 로그인 지원

HOME’S ON을 통해 스마트하고 효율적인 집안일 관리를 시작해보세요! 😊

## 🏛️ 시스템 아키텍처

<img width="987" alt="Image" src="https://github.com/user-attachments/assets/50f9b51f-e88f-49d5-a113-a7ff42bfc05a" />
HOME’S ON의 아키텍처 개요:

1. 사용자는 이메일, 카카오, 애플 계정을 통해 로그인
2. 로그인 API를 통해 인증 후 서비스 이용 가능
3. 주요 데이터는 PostgreSQL에 저장, 이미지 등은 Blob Storage 활용
4. AI 기능은 Azure OpenAI를 활용하여 제공
5. GitHub Actions를 통해 자동 빌드 및 배포 진행
6. Docker 컨테이너로 패키징하여 최신 상태 유지

## 주요 기능 상세

<img width="1232" alt="Image" src="https://github.com/user-attachments/assets/8659ffc4-aac7-4aa6-bf43-7839cddf4489" />

### 1️⃣ 체계적인 가사분담

- 멤버 전체의 집안일을 한눈에 파악할 수 있어요
- 각 멤버별로 할 일을 구분하여 더 효율적으로 관리

### 2️⃣ 효율적인 집안일

- 오늘 해야 할 집안 일을 쉽게 확인해보세요
- 일정과 할일 목록을 통해 오늘 해야 할 일을 바로 파악하고 처리 가능

### 3️⃣ 맞춤형 설정

- 담당자 지정부터 반복 일정까지 할일의 세부 사항을 원하는 대로 설정하세요
- 각 집안일에 대해 필요한 조건을 세부적으로 설정하여 개인화된 관리 가능

### 4️⃣ 멤버 초대

- 같이 사는 사람과 함께 어플을 사용해보세요
- 멤버를 초대하여 집안일을 함께 관리하고 협력할 수 있어요

### 5️⃣ SNS 로그인

- 카카오 및 애플 계정을 활용한 간편 로그인 지원
- OAuth 기반 인증 절차를 통해 안전한 로그인 환경 제공
- 로그인 후 액세스 토큰을 활용하여 세션 유지

### 6️⃣ Apple Push 알림

- 중요 일정 및 할일을 푸시 알림으로 제공
- 사용자가 알림을 허용하면 APNs(Apple Push Notification Service)에 디바이스 등록
- 집안일 추가/완료 시 APNs를 통해 즉각적인 알림 전송

### 7️⃣ AI 챗봇 기능

- OpenAI ChatGPT 기반의 챗봇
- 사용자가 입력한 집안일 관련 질문을 분석하여 적절한 응답 제공
- 질문 내용은 서버를 통해 OpenAI로 전송되며 응답 후 DB 저장

### 8️⃣ 주간 리뷰 AI

- 사용자의 집안일 수행률 분석 및 동기부여 메시지 제공
- 일주일 동안 완료한 집안일을 분석하여 개인 맞춤형 피드백 제공
- AI 기반 메시지 생성으로 더욱 친근한 동기부여 지원

## 📺 시연영상

[홈즈온 시연영상](https://photos.app.goo.gl/Cz1mgaDdUtSBtZv17)

## ⚙️ 기술 스택

### Frontend (FE)

- **Language**: Swift 5
- **Frameworks**: SwiftUI, Alamofire
- **SDKs**: KakaoSDK, Sign In with Apple
- **IDE**: Xcode

### Backend (BE)

- **Language**: Node.js
- **Frameworks**: Express
- **ORM**: Sequelize
- **AI Service**: Azure OpenAI
- **IDE**: Visual Studio Code

### Database (DB)

- **Primary DB**: Azure Database for PostgreSQL
- **Management Tool**: DBeaver

### Deployment

- **Tools**: Docker, Azure App Service, Azure Container Registry

### CI/CD

- **Platform**: GitHub Actions

### Design

- **Tool**: Figma, Mockplus

### Collaboration

- **Tool**: Notion, Discode

### Image Storage

- **Platform**: Azure Storage Account (Blob Storage)

## 📝 관련 자료

- **WBS / Gantt Chart / 요구사항정의서**: [Google Sheets ](https://docs.google.com/spreadsheets/d/1XoDhlzspNsflMcFXgnUGdKeh5nYBracT6QKc5NLqhZw/edit?usp=sharing)

- **Postman**: [postman](https://documenter.getpostman.com/view/33053461/2sAYQZHsA4)

- **ERD 다이어그램**: [dbdiagram.io ](https://dbdiagram.io/d/6732f60ce9daa85aca1fc364)

## 👀 추가 정보
