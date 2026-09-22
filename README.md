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
- OPEN API를 연동하는 과정에서 호출 제한이 있는 외부 API 환경을 고려하여, 불필요한 반복 호출을 줄이기 위한 **데이터 재사용 전략**을 설계했습니다.
- Redis/Caffeine 기반 캐싱 전략과 TTL 차등 설정을 적용해 외부 API 호출량을 최소화하고, **캐시 히트 구간의 응답 성능**을 개선한 경험이 있습니다.
- API 명세, 예외 응답 형식, 브랜치 전략, PR 리뷰 기준을 정리하며 팀 프로젝트의 **협업 품질을 높인 경험**이 있습니다.
- **부하테스트를 통해 API 응답 시간, 처리량, 에러율**을 확인하고 캐싱, 병렬 처리, 쿼리 최적화의 개선 효과를 검증 합니다.
- 댓글 좋아요 기능에서 Redis 분산락을 사용하지 않고도 **DB Unique 제약 조건과 트랜잭션 기반**으로 중복 요청을 제어 경험이 있습니다.
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

### 크라우드 펀딩 플랫폼 Seed Link - 프로그래머스 데브코스 백엔드 최종 프로젝트
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 최종 프로젝트 (5인 팀)
- **프로젝트 개요**: 청년취창업자들을 위한 아이디어 투자 플랫폼
- **담당 역할**: Toss Payments 결제API 연동, Mock 가상계좌 결제 시스템 구축, PR 총괄
- **핵심 구현**: 보증급 선납 결제 제약조건 설정, 결제 검증 및 상태전이와 가상계좌 발급, 출금제어, 동시성 제어, 선정산 출금, 보증급 환급 및 몰수 제약조건 설정, 이행중단시 상태 및 처리, 결제 내역 조회, 펀딩 취소(스폰서)
- **기술 포인트**: Webhook, Websocket, Redis
- **주요 기술**: Java, Spring Boot, Redis, Webhook, Websocket
- **Repo 바로가기**: [NBE9-11-final-Team04](https://github.com/prgrms-be-devcourse/NBE9-11-final-Team04)

### StudyWithMe 졸업논문 – AI 기반 스터디 매칭 플랫폼 (최우수 1등 작품 선정)
- **기간**: 2025.03 ~ 2025.12
- **역할**: 백엔드 아키텍처 설계/구현, AI 추천 서버 연동
- **핵심 구현**: Spring Boot API 서버와 FastAPI 추천 서버를 분리한 서비스 구조 설계, 서버 간 REST 통신 계약 정의
- **기술 포인트**: 추천 요청/응답 파이프라인 설계, 장애 시 폴백 처리, 서비스 경계 분리를 통한 확장성 확보
- **주요 기술**: Spring Boot, FastAPI, MySQL, Docker
- **Repo 바로가기**: [ai-website-studywithme](https://github.com/study-withme/ai-website-studywithme)

### 커피 주문/재고 – 프로그래머스 데브코스 백엔드 1차 팀 프로젝트 (우수팀 선정)
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 1차 프로젝트 (5인 팀)
- **프로젝트 개요**: 특정 주문조건 + 요구사항 명세서가 존재하는 환경에서 간편 주문,재고 확인 API 개발
- **담당 역할**: 내 주문내역 조회 API (고객, CUS-09) + 결제 완료된 모든 주문내역 조회 (업주, OWN-04)
- **핵심 구현**: 이메일,우편번호(주소) 검증 후, 결제 완료된 나의 주문내역을 반환 | 결제 완료된 고객들의 모든 주문내역을 이메일,우편번호로 리스트 전체 반환
- **기술 포인트**: Spring Boot DTO 패턴 사용 및 조회 처리속도 개선
- **주요 기술**: Spring Boot, Spring Data JPA, Spring Security
- **Repo 바로가기**: [NBE9-11-2-Team05](https://github.com/study-withme/NBE9-11-2-Team05)

### 합격시그널 – 프로그래머스 데브코스 백엔드 2차 팀 프로젝트
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 2차 프로젝트 (6인 팀)
- **프로젝트 개요**: 파편화된 정보들을 한곳에서 볼 수 있는 취업준비생들을 위한 취준생 커뮤니티
- **담당 역할**: `COMMENT 02, 04`(댓글/대댓글 조회·삭제), `COMMENT 05`(댓글 좋아요 처리)
- **핵심 구현**: 댓글 도메인 2Depth 조회/삭제 로직과 권한·존재성 검증 예외 처리 구현
- **기술 포인트**: 좋아요 토글을 DB insert/delete 흐름으로 설계해 정합성 유지, 댓글 트리 구조에서 케이스별 예외 응답 표준화
- **협업/운영**: 프로젝트 PR 총괄로 리뷰 기준 정리, 충돌 조율, 머지 흐름 관리
- **주요 기술**: Spring Boot, Spring Data JPA, Spring Security, Redis, Next.js
- **Repo 바로가기**: [NBE9-11-2-Team01](https://github.com/study-withme/NBE9-11-2-Team01)

### 합격시그널 – 프로그래머스 데브코스 백엔드 3차 팀 프로젝트 (Java -> Kotlin 마이그레이션)
- **프로젝트 유형**: 프로그래머스 데브코스 백엔드 엔지니어링 3차 프로젝트 (6인 팀)
- **프로젝트 개요**: 파편화된 정보들을 한곳에서 볼 수 있는 취업준비생들을 위한 취준생 커뮤니티
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
- **기술 포인트**: 데이터 크롤링, 스케줄링 수집 파이프라인 구성, 중복/실패 재시도 처리, Docker Compose 기반 멀티 서비스 오케스트레이션
- **주요 기술**: FastAPI, Playwright, Node.js/Express, Docker Compose
- **Repo 바로가기**: [data-crawling-website](https://github.com/study-withme/data-crawling-website)

### NEXON OPEN API - 게임 커뮤니티 플랫폼
- **기간**: 2025 (개인 프로젝트)
- **역할**: 백엔드 중심 풀스택 개발
- **핵심 구현**: 외부 Open API 연동 데이터 가공 파이프라인 구축, Redis/Caffeine 기반 멀티 레벨 캐싱, CompletableFuture 병렬 호출
- **기술 포인트**: Rate Limiting + 재시도 + 키 로테이션으로 외부 API 안정성 확보, 캐시 TTL 차등 설계로 응답 성능 최적화, 외부 API연동 및 데이터가공 및 시각화
- **주요 기술**: Spring Boot, Redis, MariaDB, Next.js, Docker, OPEN API
- **성과 요약**: 캐시 히트 구간 10~50ms 응답, 병렬 처리 기반 조회 성능 개선, 외부 API 호출량 절감
- **Repo 바로가기**: [NEXON OPEN API를 이용한 게임전적조회 API](https://github.com/study-withme/Nexon-OPEN-API---Sudden-Attack-Statistics-Search-Community-Platform)

### Mini Blog – Spring Boot/Java MVC 기본기 프로젝트
- **백엔드 초점**: Spring Boot + Java MVC 기반 REST API 기본기 체득
- **핵심 구현**: Controller-Service-Repository 계층 분리, JPA 엔티티 매핑 및 CRUD, DTO 기반 요청/응답 모델링
- **기술 포인트**: HTTP Method/Status 기반 API 설계, 공통 예외 처리 구조화, Gradle 기반 모듈 빌드
- **주요 기술**: Java, Spring Boot, Spring Web MVC, Spring Data JPA, Gradle
- **Repo 바로가기**: [miniblog](https://github.com/study-withme/miniblog)

---
## 기술 경험 타임라인

### 백엔드 아키텍처
* Controller-Service-Repository 계층 분리와 DTO 중심 API 경계 설계
* Spring Boot API 서버와 FastAPI 서비스 분리 등 역할 기반 서비스 경계 설정
* REST 계약 기반 서버 간 통신 설계 및 모듈 책임 분리

### 데이터 정합성 · 도메인 로직
* 댓글/대댓글 2Depth 구조에서 조회·삭제·좋아요 흐름의 예외 케이스 처리
* 좋아요 토글을 insert/delete 트랜잭션 흐름으로 구현해 상태 일관성 유지
* 외부 API/캐시/DB 폴백 순서 설계로 장애 상황에서도 일관된 응답 보장
* DB Unique 제약 조건과 트랜잭션 기반으로 중복 좋아요 요청 방지
* 삭제된 댓글, 존재하지 않는 댓글, 권한 없는 요청 등 도메인 상태별 예외 처리 표준화
* Soft Delete 기반 삭제 처리로 댓글 흐름과 데이터 이력 보존

### 성능 최적화
* Redis + Caffeine + DB 매핑 캐시를 조합한 멀티 레벨 캐싱 전략 적용
* CompletableFuture 기반 병렬 호출로 I/O 대기 시간 단축
* 데이터 성격별 TTL 차등 설정으로 실시간성-비용 균형 최적화
* JPA 연관관계 조회 시 발생할 수 있는 N+1 문제를 분석하고 Fetch Join으로 해결
* 댓글/대댓글 조회 API에서 필요한 연관 데이터를 한 번에 조회하도록 쿼리 최적화
* 캐시 히트 구간 기준 10~50ms 응답 속도 확보
* 외부 API 호출량 절감 및 응답 지연 구간 개선
* 부하테스트를 통해 API 응답 시간, 처리량, 병목 구간을 확인하고 개선 경험 보유

### 안정성 · 운영
* Rate Limiting(Bucket4j, 커스텀 정책), 재시도, 키 로테이션으로 외부 의존성 리스크 제어
* 공통 예외 처리와 표준 에러 응답 구조로 장애 원인 추적성 강화
* Spring Actuator 기반 메트릭 수집 및 캐시 히트율 모니터링 경험
* 외부 API 장애 또는 호출 제한 상황에서 캐시/DB/기본 응답으로 이어지는 폴백 구조 설계
* 잘못된 요청, 중복 요청, 권한 없는 요청에 대해 일관된 예외 응답 제공
* API 응답 시간과 부하테스트 결과를 기반으로 성능 병목을 확인하고 개선한 경험

### 동시성 · 멱등성 제어
* 댓글 좋아요 기능에서 동시에 동일 요청이 들어오는 상황을 고려하여 데이터 정합성 확보
* Redis 분산락을 사용하지 않고도 DB Unique 제약 조건과 트랜잭션 기반으로 중복 좋아요 방지
* 좋아요 insert/delete 흐름에서 중복 요청, 연속 클릭, 동시 요청 시 발생할 수 있는 상태 불일치 문제를 고려
* 비관적 락과 낙관적 락의 차이를 학습하고, 데이터 충돌 가능성과 성능 비용에 따라 적용 방식을 비교
* 재고 차감, 좋아요 수 증가, 조회수 증가 등 상태 변경 로직에서 동시성 문제가 발생할 수 있는 지점 분석
* 낙관적 락을 활용해 충돌 발생 가능성이 낮은 상태 변경 로직에서 버전 기반 정합성 제어 경험
* 비관적 락을 활용해 충돌 가능성이 높은 데이터 수정 상황에서 선점 기반 정합성 제어 방식 이해
* 좋아요 API처럼 동일 사용자의 반복 요청이 발생할 수 있는 기능에서 멱등성 있는 응답 흐름 설계
* DB 제약 조건, 트랜잭션, 예외 처리를 조합하여 애플리케이션 레벨과 데이터베이스 레벨에서 이중 안정성 확보

### 쿼리 최적화 · JPA 성능 개선
* JPA 연관관계 조회 과정에서 발생하는 N+1 문제를 식별하고 Fetch Join으로 해결
* 댓글과 대댓글 조회 시 필요한 작성자, 게시글, 부모 댓글 정보를 한 번에 조회하도록 쿼리 최적화
* 불필요한 Lazy Loading 발생 구간을 분석하고 조회 목적에 맞는 Repository 메서드 분리
* Entity 직접 반환 대신 DTO 변환을 적용하여 API 응답 구조 안정화
* 조회 API와 상태 변경 API의 트랜잭션 범위를 분리하여 불필요한 DB 부하 감소
* Query Log를 확인하며 실제 실행 SQL을 기반으로 병목 구간 분석
* 페이징, 정렬, 조건 검색이 필요한 API에서 조회 조건을 명확히 분리하여 확장 가능한 쿼리 구조 설계

### 성능 측정 · 부하테스트
* API 응답 시간, 처리량, 병목 구간을 확인하기 위한 부하테스트 경험
* 캐시 적용 전후 응답 속도 비교를 통해 성능 개선 효과 확인
* 캐시 히트 구간 기준 10~50ms 응답 속도 확보
* 외부 API 병렬 호출 적용 전후의 응답 지연 차이 분석
* N+1 문제 해결 전후 SQL 실행 횟수 및 응답 시간 개선 효과 확인
* 부하 상황에서 DB 조회, 외부 API 호출, 캐시 조회 중 어느 구간이 병목인지 분석
* 단순 기능 구현 이후 실제 요청량 증가 상황을 가정하여 API 안정성 검증

### 공공 API 및 OPEN API
* NEXON OPEN API 기반 외부 데이터 조회, 가공, 캐싱 경험
* 외부 API 응답 구조를 서비스 도메인에 맞는 DTO로 변환하는 데이터 가공 파이프라인 구현
* Rate Limiting, 재시도, API Key 로테이션을 통해 외부 API 호출 안정성 확보
* 외부 API 장애 또는 제한 상황에서 캐시/DB/기본 응답으로 이어지는 폴백 구조 설계
* 외부 API 호출량 절감을 위한 TTL 기반 캐싱 전략과 병렬 호출 최적화 경험

### 인프라 · 협업
* Docker/Docker Compose 기반 멀티 서비스 개발·실행 환경 구성
* GitHub 중심 PR 리뷰, 충돌 조율, 머지 흐름 관리로 협업 생산성 개선
* 기능 단위 커밋/리뷰 기준 정리로 변경 이력의 추적 가능성 확보
* 팀 프로젝트에서 PR 총괄 역할을 수행하며 리뷰 기준 정리, 충돌 조율, 머지 흐름 관리
* API 명세, 예외 응답, 브랜치 전략 등 협업 과정에서 필요한 개발 규칙 정리 경험


---
## What I Value as a Developer

### 명확한 역할 분리와 유지보수 가능한 구조

저는 각 컴포넌트의 책임을 명확히 나누는 구조를 중요하게 생각합니다.
Controller, Service, Repository, DTO의 역할을 분리하고, API 서버와 추천 서버처럼 서비스의 책임이 다른 경우에는 경계를 나누어 확장성과 유지보수성을 높이는 방향을 지향합니다.

### 성능과 안정성을 함께 고려하는 개발

단순히 기능이 동작하는 것에 그치지 않고, 실제 요청이 증가했을 때도 안정적으로 동작할 수 있는 구조를 고민합니다.
Redis, Caffeine 캐싱, CompletableFuture 병렬 처리, Rate Limiting, 재시도, 폴백 전략 등을 활용해 응답 속도와 외부 의존성 리스크를 함께 개선하려고 합니다.

### 문제에 맞는 기술 선택

기술을 먼저 정하고 문제에 끼워 맞추기보다, 프로젝트 요구사항과 제약 조건을 기준으로 적절한 기술을 선택하려고 합니다.
예를 들어 댓글 좋아요 기능에서는 Redis 분산락을 무조건 도입하기보다, DB Unique 제약 조건과 트랜잭션만으로도 충분히 안정성을 확보할 수 있는지 먼저 판단했습니다.

### 데이터 정합성과 예외 상황을 고려하는 설계

백엔드 개발에서 가장 중요한 부분 중 하나는 데이터가 항상 일관된 상태를 유지하도록 만드는 것이라고 생각합니다.
중복 요청, 동시 요청, 삭제된 데이터 접근, 권한 없는 요청 등 실제 서비스에서 발생할 수 있는 예외 상황을 고려하여 도메인 로직과 예외 응답을 설계하려고 합니다.

### 읽기 쉬운 코드와 일관된 스타일

함께 일하는 개발자가 빠르게 이해할 수 있는 코드를 작성하는 것을 중요하게 생각합니다.
기능 구현 이후에도 DTO 분리, 메서드 책임 분리, 공통 예외 처리, 코드 리뷰와 리팩토링을 통해 코드 품질을 개선하려고 노력합니다.

### 지속적인 학습과 실전 적용

새로운 기술을 학습하는 것에서 끝내지 않고, 프로젝트에 직접 적용하며 장단점을 이해하려고 합니다.
캐싱, 락, N+1 문제 해결, 부하테스트, 외부 API 안정화처럼 백엔드 실무에서 자주 마주치는 문제들을 프로젝트 안에서 직접 경험하며 성장하고 있습니다.

---
## Learning Roadmap

### 테스트 코드 고도화
* 단위 테스트와 통합 테스트 작성 역량 강화
* Controller, Service, Repository 계층별 테스트 전략 학습
* MockMvc, Mockito, SpringBootTest를 활용한 API 테스트 경험 확장
* 예외 케이스와 동시성 상황에 대한 테스트 코드 작성

### CI/CD 파이프라인 구축
* GitHub Actions 기반 자동 빌드 및 테스트 파이프라인 구성
* PR 생성 시 테스트 자동 실행 및 코드 품질 검증 자동화
* Docker 기반 배포 환경과 CI/CD 연동 학습
* AWS 환경에서 무중단 배포 또는 자동 배포 구조 학습

### 대규모 시스템 설계 경험 확장
* 트래픽 증가 상황을 고려한 캐싱, 큐, 비동기 처리 구조 학습
* Redis, Kafka, Message Queue 기반 이벤트 처리 구조 학습
* 마이크로서비스 아키텍처와 모놀리식 구조의 장단점 비교
* 장애 전파를 막기 위한 폴백, 재시도, 서킷 브레이커 패턴 학습

### JPA와 데이터베이스 성능 최적화 심화
* N+1 문제, Fetch Join, EntityGraph 등 조회 성능 최적화 학습
* 인덱스 설계와 실행 계획 분석 경험 확장
* 낙관적 락, 비관적 락을 활용한 동시성 제어 심화
* 트랜잭션 격리 수준과 데이터 정합성 문제 학습

### 부하테스트와 운영 관점 강화
* JMeter, k6 등을 활용한 API 부하테스트 경험 확장
* 응답 시간, 처리량, 에러율, 병목 구간 분석 역량 강화
* Actuator, Prometheus, Grafana 기반 모니터링 구조 학습
* 실제 운영 환경을 가정한 장애 대응 및 성능 개선 경험 축적

### 협업 경험 확장
* GitHub 기반 PR 리뷰, 이슈 관리, 브랜치 전략 경험 강화
* 팀 프로젝트에서 API 명세, 예외 응답, 코드 스타일 기준 정리
* 오픈소스 프로젝트 분석 및 기여 경험 축적
* 함께 유지보수하기 좋은 코드와 문서화 역량 강화

---

## Contact
- **GitHub**: https://github.com/study-withme
- **BLOG**: https://velog.io/@kimjungwoook/posts
- **Email**: kju0606@naver.com
---

> *Spring Boot 백엔드를 중심으로  
> AI 연계 및 데이터 처리 경험을 보유한 신입 개발자*  
> *확장 가능한 아키텍처 설계와 성능 최적화에 관심이 많습니다.*
