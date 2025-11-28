# HugmeEXP

Goorm EXP 클론 - 종합 학습 관리 플랫폼 + 카카오지도 API를 활용한 기능 확장(스터디룸 예약, 취업공고 확인)

## 프로젝트 소개

Goorm EXP의 핵심 기능을 재구현한 학습 관리 시스템입니다. 미션, 태스크, 그룹 학습을 통한 체계적인 학습 환경을 제공합니다.
또한, 카카오지도 API를 활용한 스터디룸 예약, 취업공고 확인 기능을 자체적으로 확장 및 추가하였습니다.

<img width="1470" height="800" alt="1" src="https://github.com/user-attachments/assets/21369950-176a-4bc3-be5c-f1753effedbd" />
<img width="1626" height="1058" alt="2" src="https://github.com/user-attachments/assets/ad5de284-c95c-4d70-bda8-7899d53198eb" />
<img width="1838" height="1252" alt="3" src="https://github.com/user-attachments/assets/5a74e3c7-0819-4a54-a4d7-bc79803812c8" />


## 주요 기능

### 학습 관리
- 미션 시스템: 생성, 진행, 완료, 리뷰 관리
- 태스크 관리: 세부 학습 과제 추적
- 그룹 학습: 팀 기반 학습 환경
- 학습 일지: 개인 학습 기록 관리

### 성과 관리
- 출석 체크 및 통계
- 칭찬 시스템 (P2P 칭찬 및 포인트)
- 포인트 상점
- 실시간 진행률 추적

### 스터디룸 예약
- Kakao Map API 기반 지도 검색
- 실시간 예약 시스템
- 위치 기반 필터링

### 기타
- 실시간 알림 시스템
- 마크다운 에디터
- 드래그 앤 드롭 UI

## 기술 스택

### Backend
- Spring Boot 3.5, Spring Security, Spring Data JPA
- Java 21
- MySQL 8.0, Redis
- JWT
- AWS (S3, EC2)
- Gradle

### Frontend
- React 19, Vite 6.x
- TypeScript
- Styled-Components
- Zustand
- React Kakao Maps SDK
- Recharts

## 도메인 구조

```
src/main/java/org/example/hugmeexp/domain/
├── mission/         # 미션 관리
├── missionTask/     # 태스크 관리
├── missionGroup/    # 그룹 학습
├── attendance/      # 출석 관리
├── praise/          # 칭찬 시스템
├── shop/            # 포인트 상점
├── notification/    # 알림 시스템
├── studydiary/      # 학습 일지
└── user/            # 사용자 관리
```

## 설치 및 실행

```bash
# 레포지토리 클론
git clone [repository-url]

# Backend 실행
cd backend
./gradlew bootRun

# Frontend 실행
cd frontend
npm install
npm run dev
```

## 문서

Swagger UI: `http://localhost:8080/swagger-ui.html`
<img width="1864" height="1436" alt="4" src="https://github.com/user-attachments/assets/18c05b58-d7d2-4f70-8f92-8d446bbcc618" />
<img width="3430" height="1582" alt="5" src="https://github.com/user-attachments/assets/98797f1f-277b-431c-8c1d-3491618a9e05" />
<img width="1790" height="1232" alt="6" src="https://github.com/user-attachments/assets/7d3b623e-8d65-4a8b-818e-096ddff80fb9" />
<img width="1490" height="712" alt="7" src="https://github.com/user-attachments/assets/a6bbe1b5-1a66-44ba-a2f3-4e1b6f21aab2" />
