# 김정욱 | Junior Backend Developer

정합성과 운영 안정성을 설계하는 Spring Boot 백엔드 개발자입니다.  
도메인 로직, 성능 최적화, 예외 처리 표준화를 기반으로 유지보수 가능한 REST API를 구현합니다.

---

## About Me

- Spring Boot 기반 백엔드에서 **도메인 중심 REST API 설계와 구현**을 주력으로 합니다.
- 기능 구현 이전에 **계층 경계(Controller-Service-Repository)와 데이터 흐름**을 먼저 설계해 유지보수성과 확장성을 확보합니다.
- 캐싱, 병렬 처리, Rate Limiting, 폴백 전략을 적용해 **성능과 안정성의 균형**을 맞춘 서비스 운영을 지향합니다.
- 댓글/대댓글 2Depth, 좋아요 토글 처리 등에서 **정합성과 예외 처리 표준화**를 기준으로 도메인 로직을 구현했습니다.
- 팀 프로젝트에서는 PR 총괄과 리뷰 흐름 관리까지 맡아 **협업 품질과 변경 이력의 추적 가능성**을 높였습니다.

---

## Tech Stack

### Core 10
![Java](https://img.shields.io/badge/Java-21-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.3.4-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-59666C?style=flat-square&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-7.0-DC382D?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

---

## Projects

- **전체 레포지토리**: [github.com/study-withme](https://github.com/study-withme)

### Mini Blog – Spring Boot/Java MVC 기본기 프로젝트
- **백엔드 초점**: Spring Boot + Java MVC 기반 REST API 기본기 체득
- **핵심 구현**: Controller-Service-Repository 계층 분리, JPA 엔티티 매핑 및 CRUD, DTO 기반 요청/응답 모델링
- **기술 포인트**: HTTP Method/Status 기반 API 설계, 공통 예외 처리 구조화, Gradle 기반 모듈 빌드
- **주요 기술**: Java, Spring Boot, Spring Web MVC, Spring Data JPA, Gradle
- **Repo 바로가기**: [miniblog](https://github.com/study-withme/miniblog)

### StudyWithMe 졸업논문 – AI 기반 스터디 매칭 플랫폼 (최우수 1등 작품 선정)
- **기간**: 2025.03 ~ 2025.12
- **역할**: 백엔드 아키텍처 설계/구현, AI 추천 서버 연동
- **핵심 구현**: Spring Boot API 서버와 FastAPI 추천 서버를 분리한 서비스 구조 설계, 서버 간 REST 통신 계약 정의
- **기술 포인트**: 추천 요청/응답 파이프라인 설계, 장애 시 폴백 처리, 서비스 경계 분리를 통한 확장성 확보
- **주요 기술**: Spring Boot, FastAPI, MySQL, Docker
- **Repo 바로가기**: [ai-website-studywithme](https://github.com/study-withme/ai-website-studywithme)

### NEXON OPEN API - 게임 커뮤니티 플랫폼
- **기간**: 2025 (개인 프로젝트)
- **역할**: 백엔드 중심 풀스택 개발
- **핵심 구현**: 외부 Open API 연동 데이터 가공 파이프라인 구축, Redis/Caffeine 기반 멀티 레벨 캐싱, CompletableFuture 병렬 호출
- **기술 포인트**: Rate Limiting + 재시도 + 키 로테이션으로 외부 API 안정성 확보, 캐시 TTL 차등 설계로 응답 성능 최적화
- **주요 기술**: Spring Boot, Redis, MariaDB, Next.js, Docker
- **성과 요약**: 캐시 히트 구간 10~50ms 응답, 병렬 처리 기반 조회 성능 개선, 외부 API 호출량 절감
- **Repo 바로가기**: [Nexon-OPEN-API---Sudden-Attack-Statistics-Search-Community-Platform](https://github.com/study-withme/Nexon-OPEN-API---Sudden-Attack-Statistics-Search-Community-Platform)

### 커피 주문/재고 – 프로그래머스 데브코스 백엔드 1차 팀 프로젝트 (우수팀 선정)
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 1차 프로젝트 (5인 팀)
- **담당 역할**: 내 주문내역 조회 API (고객, CUS-09) + 결제 완료된 모든 주문내역 조회 (업주, OWN-04)
- **핵심 구현**: 이메일,우편번호(주소) 검증 후, 결제 완료된 나의 주문내역을 반환 | 결제 완료된 고객들의 모든 주문내역을 이메일,우편번호로 리스트 전체 반환
- **기술 포인트**: 
- **주요 기술**: Spring Boot, Spring Data JPA, Spring Security
- **Repo 바로가기**: [NBE9-11-2-Team05](https://github.com/study-withme/NBE9-11-2-Team05)

### 합격시그널 – 프로그래머스 데브코스 백엔드 2차 팀 프로젝트
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 2차 프로젝트 (6인 팀)
- **담당 역할**: `COMMENT 02, 04`(댓글/대댓글 조회·삭제), `COMMENT 05`(댓글 좋아요 처리)
- **핵심 구현**: 댓글 도메인 2Depth 조회/삭제 로직과 권한·존재성 검증 예외 처리 구현
- **기술 포인트**: 좋아요 토글을 DB insert/delete 흐름으로 설계해 정합성 유지, 댓글 트리 구조에서 케이스별 예외 응답 표준화
- **협업/운영**: 프로젝트 PR 총괄로 리뷰 기준 정리, 충돌 조율, 머지 흐름 관리
- **주요 기술**: Spring Boot, Spring Data JPA, Spring Security, Redis, Next.js
- **Repo 바로가기**: [NBE9-11-2-Team01](https://github.com/study-withme/NBE9-11-2-Team01)

### Data Crawling Website – 게임 데이터 수집 및 시각화
- **기간**: 2024
- **역할**: 크롤링 서버 및 API 서버 개발
- **핵심 구현**: Playwright 기반 동적 페이지 크롤링 자동화, FastAPI 데이터 제공 API, Node.js 시각화 서버 분리
- **기술 포인트**: 스케줄링 수집 파이프라인 구성, 중복/실패 재시도 처리, Docker Compose 기반 멀티 서비스 오케스트레이션
- **주요 기술**: FastAPI, Playwright, Node.js/Express, Docker Compose
- **Repo 바로가기**: [data-crawling-website](https://github.com/study-withme/data-crawling-website)

---

## 기술 역량 요약

### 백엔드 아키텍처
- Controller-Service-Repository 계층 분리와 DTO 중심 API 경계 설계
- Spring Boot API 서버와 FastAPI 서비스 분리 등 역할 기반 서비스 경계 설정
- REST 계약 기반 서버 간 통신 설계 및 모듈 책임 분리

### 데이터 정합성 · 도메인 로직
- 댓글/대댓글 2Depth 구조에서 조회·삭제·좋아요 흐름의 예외 케이스 처리
- 좋아요 토글을 insert/delete 트랜잭션 흐름으로 구현해 상태 일관성 유지
- 외부 API/캐시/DB 폴백 순서 설계로 장애 상황에서도 일관된 응답 보장

### 성능 최적화
- Redis + Caffeine + DB 매핑 캐시를 조합한 멀티 레벨 캐싱 전략 적용
- CompletableFuture 기반 병렬 호출로 I/O 대기 시간 단축
- 데이터 성격별 TTL 차등 설정으로 실시간성-비용 균형 최적화

### 안정성 · 운영
- Rate Limiting(Bucket4j, 커스텀 정책), 재시도, 키 로테이션으로 외부 의존성 리스크 제어
- 공통 예외 처리와 표준 에러 응답 구조로 장애 원인 추적성 강화
- Spring Actuator 기반 메트릭 수집 및 캐시 히트율 모니터링 경험

### 인프라 · 협업
- Docker/Docker Compose 기반 멀티 서비스 개발·실행 환경 구성
- GitHub 중심 PR 리뷰, 충돌 조율, 머지 흐름 관리로 협업 생산성 개선
- 기능 단위 커밋/리뷰 기준 정리로 변경 이력의 추적 가능성 확보

---

## What I Value as a Developer
- **명확한 역할 분리와 구조**: 각 컴포넌트의 책임을 명확히 하고, 확장성과 유지보수를 고려한 설계
- **성능과 안정성**: 캐싱, 병렬 처리, Rate Limiting 등을 통한 성능 최적화와 안정성 확보
- **문제에 맞는 기술 선택**: 프로젝트 요구사항에 맞는 최적의 기술 스택 선택
- **읽기 쉬운 코드와 일관된 스타일**: 코드 리뷰와 리팩토링을 통한 코드 품질 개선
- **지속적인 학습**: 최신 기술 트렌드를 학습하고 프로젝트에 적용

---

## 향후 학습 계획
- **테스트 코드 작성**: 단위 테스트 및 통합 테스트 커버리지 향상
- **CI/CD 파이프라인**: GitHub Actions 등을 활용한 자동화 구축
- **대규모 시스템 경험**: 마이크로서비스 아키텍처 심화 학습 및 실무 적용
- **협업 경험**: 오픈소스 기여 또는 팀 프로젝트 참여를 통한 협업 경험 축적
---

## Contact
- **GitHub**: https://github.com/study-withme
- **BLOG**: https://velog.io/@kimjungwoook/posts
- **Email**: kju0606@naver.com
---

> *Spring Boot 백엔드를 중심으로  
> AI 연계 및 데이터 처리 경험을 보유한 신입 개발자*  
> *확장 가능한 아키텍처 설계와 성능 최적화에 관심이 많습니다.*
