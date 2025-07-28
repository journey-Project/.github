# 여정(Journey)

## 프로젝트 소개

<img src="image/여정로고.png" alt="여정로고" width="180"/>

**여정(Journey)** 는 여행자들이 서로의 여행 계획을 공유하고 동행자를 구할 수 있는 여행 커뮤니티 서비스입니다.

이 서비스는 사용자들이 동행자를 구함으로써 보다 안전하고 즐거운 여행 경험을 할 수 있도록 설계할 예정입니다. <br>여행을 계획하는 사람들이 관심 있는 여행지, 일정, 여행 스타일 등을 기준으로 동행자를 찾고, 정보와 경험을 나눌 수 있는 플랫폼을 제공합니다.


![여정_메인.jpg](image/%EC%97%AC%EC%A0%95_%EB%A9%94%EC%9D%B8.jpg)

## 팀원 구성

|  |  |  |  |
|:--:|:--:|:--:|:--:|
| <img src="https://github.com/AshtonSW.png" width="150"/> <br> **김승원** <br> [@AshtonSW](https://github.com/AshtonSW) | <img src="https://github.com/jkchoi490.png" width="150"/> <br> **최정경** <br> [@jkchoi490](https://github.com/jkchoi490) | <img src="https://github.com/KwonSerim2.png" width="150"/> <br> **권세림** <br> [@KwonSerim2](https://github.com/KwonSerim2) | <img src="https://github.com/llleeco.png" width="150"/> <br> **이찬희** <br> [@llleeco](https://github.com/llleeco) |

**BackEnd**

| 이름 | Github | email                                               |
| --- | --- |-----------------------------------------------------|
| 김승원 | [https://github.com/AshtonSW](https://github.com/AshtonSW) | [sprauncy76@gmail.com](mailto:sprauncy76@gmail.com) |
| 최정경 | [https://github.com/jkchoi490](https://github.com/jkchoi490) | [jgchoideveloper490@gmail.com](mailto:jgchoideveloper490@gmail.com)             |

**FrontEnd**

| 이름 | Github | email |
| --- | --- | --- |
| 김승원 | [https://github.com/AshtonSW](https://github.com/AshtonSW) | [sprauncy76@gmail.com](mailto:sprauncy76@gmail.com) |
| 권세림 | [https://github.com/KwonSeRim2](https://github.com/KwonSeRim2) | [serimkwon1@gmail.com](mailto:serimkwon1@gmail.com) |
| 이찬희 | [https://github.com/llleeco](https://github.com/llleeco) | [lch80566@gmail.com](mailto:lch80566@gmail.com) |

**Design**

| 이름 | Github | email |
| --- | --- | --- |
| 김승원 | [https://github.com/AshtonSW](https://github.com/AshtonSW) | [sprauncy76@gmail.com](mailto:sprauncy76@gmail.com) |
| 장서윤 | | [jsy11220603@gmail.com](mailto:jsy11220603@gmail.com)  |

## 시스템 아키텍처
![찐최종여정시스템아키텍처.jpg](image/%EC%B0%90%EC%B5%9C%EC%A2%85%EC%97%AC%EC%A0%95%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.jpg)

## ERD

![여정erd.png](image/%EC%97%AC%EC%A0%95erd.png)

## 기술 스택

### 백엔드

Java 21, Gradle, SpringBoot, MySQL,

Docker, Github Actions, AWS EC2, RDS, S3, NginX

![백엔드기술스택.png](image/%EB%B0%B1%EC%97%94%EB%93%9C%EA%B8%B0%EC%88%A0%EC%8A%A4%ED%83%9D.png)

### 프론트엔드

JavaScript, Vue.js, CloudFront, Github Actions, Amazon S3, Axios, Pinia, Vue Router

![프론트기술스택.png](image/%ED%94%84%EB%A1%A0%ED%8A%B8%EA%B8%B0%EC%88%A0%EC%8A%A4%ED%83%9D.png)

### 디자인

Figma

![디자인기술스택.png](image/%EB%94%94%EC%9E%90%EC%9D%B8%EA%B8%B0%EC%88%A0%EC%8A%A4%ED%83%9D.png)

## 시스템 구성

### 🔐 사용자 인증 및 인가

- **기능**: 회원가입, 자체 로그인, 소셜 로그인, 세션 기반 인증 및 인가
- **설명**: 사용자가 회원가입 후 로그인하면 서버에서 세션을 생성하고, 클라이언트는 세션 ID를 통해 인증된 사용자로 다양한 서비스를 이용할 수 있습니다.
- **사용 기술**
    - **Backend :** Spring Security, Spring Session, Spring Boot, JPA, MySQL
    - **Frontend :** Vue.js, Vue Router, Axios, Pinia

---

### 🧑 사용자 프로필

- **기능**: 사용자 정보 조회, 수정 (닉네임, 프로필 이미지), 여행 일정 관리
- **설명**: 사용자가 자신의 프로필을 조회하고 편집할 수 있는 기능과 여행 일정 관리기능을 제공합니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, MySQL, AWS S3
    - **Frontend** : Vue.js, Axios, Pinia, Amazon S3, Vue Router

---

### 🧑‍🤝‍🧑 동행자 모집 및 커뮤니티

- **기능**: 게시글 작성, 조회, 수정, 삭제 (CRUD)
- **설명**:  여행 동행자를 모집할 수 있는 게시판 기능을 제공하며, 국가별 커뮤니티에서 자유롭게 게시글을 작성할 수 있습니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, MySQL, AWS S3, AWS RDS
    - **Frontend** : Vue.js, Axios, Pinia, Vue Router, Amazon S3

---

### 🔍 게시글 검색

- **기능**: 제목, 작성자, 여행 기간, 국가, 게시글 번호 기반 조건 검색
- **설명**: 다양한 필터 조건을 통해 게시글을 검색할 수 있으며, 페이징 처리도 지원됩니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, JPA Specification, Pagination
    - **Frontend** : Vue.js, Axios, Pinia, Vue Router

---

### 💬 댓글 기능

- **기능**: 댓글 등록, 수정, 삭제
- **설명**: 각 게시글에 대해 댓글을 CRUD 방식으로 관리하며, 댓글 삭제 시 soft delete(논리 삭제) 방식이 적용됩니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, MySQL
    - **Frontend** : Vue.js, Axios, Pinia

---

### 🔔 댓글 알림 기능

- **기능**: 게시글에 댓글이 작성되었을 때 작성자에게 알림 전송
- **설명**: WebSocket을 활용하여 사용자에게 실시간으로 댓글 알림을 전달합니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, MySQL, WebSocket (STOMP)
    - **Frontend** : Vue.js, WebSocket (STOMP), Pinia

---

### 🔗 팔로우 / 팔로잉 기능

- **기능**: 다른 사용자 팔로우, 언팔로우, 팔로워/팔로잉 목록 조회
- **설명**: 사용자가 관심 있는 유저를 팔로우하고, 자신의 팔로워 및 팔로잉 목록을 관리할 수 있습니다.
- **사용 기술**
    - **Backend** : Spring Boot, JPA, MySQL
    - **Frontend** : Vue.js, Axios, Pinia

---

### 🚀 배포 및 인프라

📦 **공통**

- **CI/CD 파이프라인**: GitHub Actions
- **정적 자산 호스팅 (프론트엔드)**: Amazon S3
- **CDN 가속 (프론트엔드)**: CloudFront

⚙️ **백엔드 서버**

- **서버 운영**: AWS EC2
- **배포 환경**: Docker, NginX
- **애플리케이션 런타임**: Java 21, Spring Boot
- **빌드 도구**: Gradle

🗄 **데이터베이스**

- **DBMS**: MySQL
- **DB 인프라**: AWS RDS

📁 **파일 스토리지**

- **이미지 및 정적 파일 저장**: Amazon S3

## 관련 저장소

여정 백엔드 레포 : https://github.com/journey-Project/Backend

여정 프론트엔드 레포 : https://github.com/journey-Project/Frontend

여정 피그마 : <br>
초안 : https://www.figma.com/design/oQFNYCoAE6Zr7qapSMC1O5/%EC%97%AC%EC%A0%95?node-id=0-1&t=5d0suT6F4L9AdQOW-1
<br>
최종 : https://www.figma.com/design/ZOYFmV7T7EmlQXDdwrXBQP/%EC%97%AC%EC%A0%95-%EB%94%94%EC%9E%90%EC%9D%B8---%EA%B9%80%EC%8A%B9%EC%9B%90?node-id=1164-3118&t=4EJ29MijhQW78ssD-1
