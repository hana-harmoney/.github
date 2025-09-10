# 하나하모니 (Hana Harmony)

> **시니어의 경험과 시간을 가치로 바꾸는 금융·일자리 플랫폼**  
> “하나의 경험을 모두의 가치로”

<img width="1720" alt="image" src="https://github.com/user-attachments/assets/dfff5813-e509-414f-a513-2fb3ea65e0db" />


- `개발 기간` : **2025.08.21 ~ 2025.09.09**
- `서비스 배포 URL` :  [Hana Harmoney](https://frontend-nine-iota-61.vercel.app/) 
- `시연 영상 URL` : [https://youtu.be/3iGpzZEcClM](https://youtu.be/3iGpzZEcClM)
<br/>


## 📌 프로젝트 소개
**하나하모니**는 시니어 세대가 가진 경험, 지식, 시간을 소득과 자산으로 전환해주는 금융 기반 플랫폼입니다.  
단순한 아르바이트 제공이 아닌, 시니어의 삶의 경험과 노하우를 지역사회와 연결하고 이를 통해 **작은 수입을 만들고 저축·연금과 연계**할 수 있는 구조를 제안합니다.

- 시니어는 자존감을 유지하며 활동적인 노후를 보낼 수 있습니다.
- 지역사회와 가족은 어르신의 노하우와 따뜻한 교류를 얻을 수 있습니다.
- 금융사(하나은행)는 연금·저축 등 금융상품 가입으로 연결할 수 있습니다.


<br/>


## 🎯 주요 기능

- **사용자 프로필**
  - 가족(자녀·손주)이 대신 소개가능한 스토리텔링 프로필
  - 예: “우리 할머니는 20년 넘게 아이들을 가르친 경험이 있어요.”

- **일자리 등록 및 매칭**
  - 고용주가 지역 기반으로 일자리(아이돌봄, 교육, 농업, 청소 등) 등록
  - 시니어가 일자리 탐색 및 지원 가능
  - 채팅으로 조건 협의 후 매칭 확정

- **주머니 기능** 
  - 시니어의 활동 수입을 주머니로 관리 가능
  - 주머니별 목표 금액 설정 및 진행률 확인  
  - 지출/저축 내역을 주머니와 연동해 한눈에 관리 가능

- **위치 기반 일자리 목록**
  - 지도 및 반경 기반으로 가까운 일자리 탐색
  - 거리순 정렬 지원

- **금융 연계**
  - 수입 내역 자동 기록
  - 지출/저축 내역 관리
  - 연금·저축 상품과 연계

- **신뢰도 지표**
  - 매칭 횟수, 후기를 통한 신뢰도 반영 제공
  - 안전한 거래와 매칭을 도움
 
- **채팅 기능**  
  - WebSocket(STOMP) 기반 1:1 실시간 채팅  
  - 텍스트, **음성 메시지 전송 지원**  
  - 금칙어 **자동 필터링** 적용으로 안전한 대화 환경 제공  
  - 사용자 간 **신고하기 기능**으로 관리자에게 리포트

<br/>

### 📸 서비스 화면

| 프로필 등록 화면 | 홈 화면 | 계좌 상세 화면 | 구직 화면 |
|:---:|:---:|:---:|:---:|
| <img width="250" src="https://github.com/user-attachments/assets/93faab90-5302-4011-98db-3c19bd251779" /> <br/> | <img width="250" src="https://github.com/user-attachments/assets/04e54111-dd99-4676-a492-2f1196671102" /> <br/> | <img width="250" src="https://github.com/user-attachments/assets/360634da-93da-4f2d-b677-856dc00e3055" /> <br/> | <img width="250" src="https://github.com/user-attachments/assets/ea4693aa-9462-4983-a93c-6dbadcea66a7" /> <br/>  |

| 채팅 화면 | 후기 화면 | 하모니 수입 화면 | 내 정보 |
|:---:|:---:|:---:| :---:|
| <img width="250" src="https://github.com/user-attachments/assets/2c8f7ed3-2e20-44c3-94b6-c7edc4d0a093" /> <br/>  | <img width="250"  alt="후기화면" src="https://github.com/user-attachments/assets/03edaadc-0bad-4a81-a9fb-ef79afa61d71" /> |  <img width="250" src="https://github.com/user-attachments/assets/5deacd74-28f9-47a2-8431-c4b38bdcb353" /> <br/>  | <img width="250" src="https://github.com/user-attachments/assets/c12bfea5-1f98-4746-a5e4-cf97b4d9c2d5" /> <br/>  |




---
<br/>


## 🏗️ 시스템 아키텍처

<img width="870" height="512" alt="image" src="https://github.com/user-attachments/assets/99e3e950-280f-4f61-980a-985f4ac9c86b" />


<br/>
<br/>


## ERD
<img  height="700" alt="하나하모니erd" src="https://github.com/user-attachments/assets/a16c66d9-d4e5-4ada-b21c-10a9f5046d35" />

<br/>

---

## 📂 파일 구조

<details>
<summary><b>📁 Backend</b></summary>
  
```
├── main
│   ├── java
│   │   └── com
│   │       └── example
│   │           └── hanaharmonybackend
│   │               ├── config
│   │               ├── domain
│   │               ├── payload
│   │               ├── repository
│   │               ├── service
│   │               ├── util
│   │               ├── web
│   │               └── HanaharmonyBackendApplication.java
│   └── resources
│       ├── firebase
│       └── application.yml
└── test
    └── java
        └── com
            └── example
                └── hanaharmonybackend
                    ├── config
                    ├── repository
                    ├── service
                    └── HanaharmonyBackendApplicationTests.java


```
</details>


<details>
<summary><b>📁 Frontend</b></summary>
  
```
├── public
├── src
│  ├── app
│  │  ├── api 	
│  │  ├── asset
│  │  ├── auth
│  │  ├── chat
│  │  ├── chatroom
│  │  ├── education
│  │  ├── home
│  │  ├── jobs
│  │  ├── layout.tsx
│  │  ├── global-error.tsx
│  │  ├── NotificationProvider.tsx
│  │  ├── page.tsx
│  │  ├── globals.css
│  │  └── profile
│  ├── assets
│  │  ├── icons
│  │  ├── images
│  │  └── lottie
│  ├── components
│  │  ├── asset
│  │  ├── auth
│  │  ├── chat
│  │  ├── common
│  │  ├── education
│  │  ├── home
│  │  ├── jobs
│  │  ├── manual
│  │  ├── pocket
│  │  ├── profile
│  │  └── ui
│  ├── firebase
│  ├── fonts
│  ├── hooks
│  ├── lib
│  │  ├── api
│  │  ├── date
│  │  └── utils.ts
│  ├── middlewares.ts
│  ├── stores
│  └── types
```
</details>

<br/> 


## 🛠 Tech Stack

### Platforms & Languages
<p>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white"/>
  <img src="https://img.shields.io/badge/Zustand-000000?style=flat&logo=react&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/QueryDSL-009639?style=flat&logo=spring&logoColor=white"/>
  <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white"/>
  <img src="https://img.shields.io/badge/WebSocket-010101?style=flat&logo=socket.io&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white"/>
</p>

### Deployment & Infra
<p>
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS EC2-FF9900?style=flat&logo=amazonec2&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS S3-569A31?style=flat&logo=amazons3&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS RDS-527FFF?style=flat&logo=amazonrds&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=flat&logo=githubactions&logoColor=white"/>
</p>

### Communication & Notification
<p>
  <img src="https://img.shields.io/badge/Firebase Cloud Messaging-FFCA28?style=flat&logo=firebase&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kakao Map-FFCD00?style=flat&logo=kakao&logoColor=black"/>
</p>

### Development Environment
<p>
  <img src="https://img.shields.io/badge/IntelliJ IDEA-000000?style=flat&logo=intellijidea&logoColor=white"/>
  <img src="https://img.shields.io/badge/VSCode-007ACC?style=flat&logo=visualstudiocode&logoColor=white"/>
</p>

### Communication & Management
<p>
  <img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white"/>
  <img src="https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white"/>
  <img src="https://img.shields.io/badge/Slack-4A154B?style=flat&logo=slack&logoColor=white"/>
</p>

<br/>


## 📍 테스트 유형 및 내용

#### 1. **Repository 통합 테스트** (`@DataJpaTest`)
**BoardRepositoryDistanceStatusTest**
- **목적**: 위치 기반 게시글 검색 기능의 정확성 검증
- **테스트 내용**:
  - 반경 내 활성 게시글만 조회되는지 확인
  - 종료된 게시글(status=true) 제외 여부 검증
  - 거리순 정렬이 올바르게 작동하는지 확인
  - 네이티브 쿼리 `findNearbyIdsWithDistanceAll()` 동작 검증

#### 2. **성능 테스트** (`@SpringBootTest`)
**TransactionHistoryPerformanceTest**
- **목적**: JPQL vs QueryDSL 성능 비교
- **테스트 내용**:
  - 주머니별 거래내역 조회 성능 측정
  - 계좌별 거래내역 조회 성능 측정
  - 실행 시간 및 결과 데이터 크기 비교

#### 3. **Service 단위 테스트** (`@ExtendWith(MockitoExtension.class)`)
**BoardNearbyServiceTest**
- **목적**: 근처 게시글 조회 서비스 로직 검증
- **테스트 내용**:
  - 거리순 정렬이 DTO 변환 시에도 유지되는지 확인
  - 사용자 위치 정보가 없을 때 예외 처리 검증
  - Mock을 활용한 의존성 격리 테스트

#### 4. **애플리케이션 컨텍스트 테스트**
**HanaharmonyBackendApplicationTests**
- **목적**: Spring Boot 애플리케이션 정상 시작 확인
- **테스트 내용**:
  - 모든 Bean이 올바르게 로드되는지 확인
  - 의존성 주입이 정상적으로 작동하는지 검증

<br/>

### 주요 테스트 시나리오

#### 1. **위치 기반 검색 테스트**
- **시나리오**: 분당 지역(37.311, 127.074)을 기준으로 반경 6km 내 게시글 검색
- **검증 포인트**:
  - 활성 게시글만 조회됨
  - 종료된 게시글 제외됨
  - 거리순 정렬됨
  - 반경 밖 게시글 제외됨

#### 2. **성능 최적화 테스트**
- **시나리오**: 대용량 거래내역 데이터 조회 시 성능 비교
- **검증 포인트**:
  - JPQL vs QueryDSL 실행 시간
  - 메모리 사용량
  - 쿼리 최적화 효과

#### 3. **비즈니스 로직 테스트**
- **시나리오**: 근처 게시글 조회 서비스의 정상 동작
- **검증 포인트**:
  - 사용자 위치 정보 유효성 검사
  - 거리 정보 정확성
  - 예외 상황 처리


---
<br/> 

## 👩🏻‍💻 팀원 소개
| <img src="https://avatars.githubusercontent.com/hyo-joon" width="130"/> | <img src="https://avatars.githubusercontent.com/jhpark0888" width="130"/> | <img src="https://avatars.githubusercontent.com/jjinleee" width="130"/> | <img src="https://avatars.githubusercontent.com/rladbflaz" width="130"/> | <img src="https://avatars.githubusercontent.com/VarGun" width="130"/> | <img src="https://avatars.githubusercontent.com/youlimsongs" width="130"/> | <img src="https://avatars.githubusercontent.com/zzimnii" width="130"/> |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| **Hyo-joon**<br>[@hyo-joon](https://github.com/hyo-joon)<br/> | **Park Ji Hwan**<br>[@jhpark0888](https://github.com/jhpark0888)<br/> | **Jin Lee**<br>[@jjinleee](https://github.com/jjinleee)<br/> | **rladbflaz**<br>[@rladbflaz](https://github.com/rladbflaz)<br/> | **Heegun Kwak**<br>[@VarGun](https://github.com/VarGun)<br/> | **Yourim Song**<br>[@youlimsongs](https://github.com/youlimsongs)<br/> | **zzimnii**<br>[@zzimnii](https://github.com/zzimnii)<br/> |

<br/> 

