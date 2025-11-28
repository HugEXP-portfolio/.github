# HugmeEXP

Goorm EXP 클론 - 종합 학습 관리 플랫폼 + 카카오지도 API를 활용한 기능 확장(스터디룸 예약, 취업공고 확인)

## 프로젝트 소개

Goorm EXP의 핵심 기능을 재구현한 학습 관리 시스템입니다. 미션, 태스크, 그룹 학습을 통한 체계적인 학습 환경을 제공합니다.
또한, 카카오지도 API를 활용한 스터디룸 예약, 취업공고 확인 기능을 자체적으로 확장 및 추가하였습니다.

![스크린샷 2025-11-27 오전 5.10.54.png](attachment:9078d525-321e-4944-99a2-7c722db0dd68:스크린샷_2025-11-27_오전_5.10.54.png)
![image.png](attachment:f9799374-545e-403a-bb33-4f3b54cace55:image.png)
![image.png](attachment:f58c508a-2f72-4623-8478-3b15a9a0b13c:image.png)

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
![image.png](attachment:05472707-9290-401c-b21e-5a8123750ae9:image.png)
![HugExp.png](attachment:17a8f477-493b-4c96-bcbb-3a23a99b0e4f:HugExp.png)
![StudyRoom.png](attachment:fffffc95-09b8-4b1c-b717-4d07e955387a:StudyRoom.png)
![지도 api.png](attachment:7967d763-c526-4ccc-8de2-b44b79c33ce4:지도_api.png)
