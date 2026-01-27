# 김정욱 | Junior Backend Developer

Spring Boot 기반 신입 백엔드 개발자입니다.  
- AI 추천 시스템 연계와 데이터 수집, 처리 중심의 서버 아키텍처를 설계 구현했습니다.
- NEXON OPEN API 데이터를 활용하여 사용자 정보를 수집,가공,제공 했습니다.
- Playwright을 활용하여 data crawling 프로젝트를 수행하였습니다.

---

## About Me

- **Spring Boot 기반 웹 백엔드 개발**을 주력으로 하며, RESTful API 설계 및 구현 경험이 있습니다.
- 졸업작품으로 **AI 기반 스터디 매칭 플랫폼**을 설계·구현하여 사용자 맞춤형 추천 시스템을 구축했습니다.
- **마이크로서비스 아키텍처** 설계 경험: Java 백엔드 서버와 Python(FastAPI) AI 서버를 역할별로 분리하여 독립적 배포 및 확장 가능한 구조를 구현했습니다.
- **성능 최적화**에 관심이 많으며, 대용량 트래픽 환경에서 캐싱 전략, 병렬 처리, Rate Limiting 등을 적용한 경험이 있습니다.
- 데이터 흐름과 시스템 구조를 먼저 설계한 뒤 구현하는 개발 방식을 선호하며, 코드 리뷰와 테스트를 통해 품질을 개선하는 것에 가치를 둡니다.
- Docker를 활용하여 실제 프로젝트들을 배포·운영한 경험이 있으며, CI/CD 파이프라인 구축에도 관심이 있습니다.

---

## Tech Stack

### Backend
- **Java 21** / **Spring Boot 3.3.4**
- Spring Data JPA, Spring Security, Spring Cache
- REST API Design, OpenAPI 3 (Swagger)
- JWT 기반 인증/인가

### Cache & Performance
- **Redis 7.0** (분산 캐시)
- **Caffeine** (로컬 캐시)
- Bucket4j (Rate Limiting)
- CompletableFuture (비동기 병렬 처리)

### AI / Data Processing
- **Python** / **FastAPI**
- Vectorization, Cosine Similarity (추천 알고리즘)
- NumPy, Pandas (데이터 처리)

### Crawling / Automation
- **Playwright** (동적 웹 크롤링)
- 스케줄링 및 자동화

### Database
- **MySQL** / **MariaDB 10.6**
- Flyway (데이터베이스 마이그레이션)
- JPA/Hibernate

### Infrastructure & DevOps
- **Docker** / **Docker Compose**
- Cloudtype (PaaS 배포)
- Spring Actuator (모니터링)

### Tools
- Git / GitHub
- IntelliJ IDEA / VS Code
- Gradle

---

## Featured Projects

## StudyWithMe – AI 기반 스터디 매칭 플랫폼 (졸업작품)

**프로젝트 기간**: 2025년 03월 ~ 2025년 12월 (졸업작품)  
**역할**: 백엔드 아키텍처 설계 및 구현, AI 서버 연동  
**기술 스택**: Spring Boot, Python FastAPI, MySQL, Docker  
**GitHub**: https://github.com/study-withme/ai-website-studywithme

### 프로젝트 개요
사용자의 관심 태그와 학습 스타일을 분석하여 최적의 스터디 그룹을 추천하는 AI 기반 매칭 플랫폼입니다. Java 백엔드 서버와 Python AI 서버를 분리하여 확장 가능한 아키텍처를 설계했습니다.

### 핵심 구현 내용

#### 1. 마이크로서비스 아키텍처 설계
- **서버 분리 전략**: Spring Boot 웹 서버와 Python FastAPI 추천 서버를 독립적으로 설계
  - 각 서버의 독립적 배포 및 확장 가능
  - 서버 간 HTTP REST API 통신으로 느슨한 결합(Loose Coupling) 구현
  - 서비스별 역할 명확화로 유지보수성 향상

#### 2. AI 추천 알고리즘 구현
- **벡터화 및 유사도 계산**
  - 사용자 관심 태그를 TF-IDF 기반 벡터로 변환
  - 코사인 유사도(Cosine Similarity)를 활용한 사용자 간 유사도 측정
  - 유사도 점수 기반으로 최적의 스터디 그룹 추천 로직 구현
- **성능 최적화**: 벡터 연산을 NumPy로 최적화하여 추천 속도 개선

#### 3. Java-Python 서버 연동
- **프로세스 관리**
  - Java `ProcessBuilder`를 활용한 Python AI 서버 프로세스 실행 및 생명주기 관리
  - 프로세스 상태 모니터링 및 자동 재시작 로직 구현
- **비동기 통신 구조**
  - 웹 서버와 AI 서버 간 HTTP 통신으로 효율적 데이터 교환
  - 타임아웃 및 재시도 로직으로 안정성 확보
- **에러 핸들링**: AI 서버 장애 시 기본 추천 로직으로 폴백 처리

#### 4. 백엔드 API 설계
- RESTful API 설계 원칙 준수 (리소스 기반 URL, HTTP 메서드 활용)
- 전체 서버 아키텍처 설계 및 각 서비스 역할 분담 담당
- API 문서화를 통한 프론트엔드 팀과의 협업 효율화

### 성과 및 학습 경험
- 마이크로서비스 아키텍처의 장단점을 실무적으로 이해
- 이기종 언어 간 통신 및 프로세스 관리 경험
- AI 추천 시스템의 기본 원리와 구현 방법 학습

---

## NEXON OPEN API - 게임 커뮤니티 플랫폼

**프로젝트 기간**: 2025년 (개인 프로젝트)  
**역할**: 풀스택 개발 (Backend 중심)  
**기술 스택**: Spring Boot 3.3.4, Java 21, Redis 7.0, MariaDB 10.6, Next.js 16, Docker  
**GitHub**: https://github.com/study-withme/Nexon-OPEN-API---Sudden-Attack-Statistics-Search-Community-Platform

### 프로젝트 개요
Nexon OPEN API를 활용한 서든어택 게임 전적 조회 및 커뮤니티 플랫폼입니다. 대용량 트래픽 환경에서 외부 API 의존성을 최소화하고 데이터 정합성과 응답 속도를 동시에 유지하는 것이 핵심 과제였습니다.

### 핵심 구현 내용

#### 1. 외부 API 통합 및 데이터 가공
- **Nexon OPEN API 통합**
  - 실시간 유저 정보 조회 (프로필, 랭크, 티어, 매치 기록)
  - 원본 API 데이터를 비즈니스 로직에 맞게 가공 및 변환
  - 다양한 지표 계산 (승률, K/D, 평균 점수 등) 및 UI/UX에 최적화된 데이터 구조 설계
- **API 키 로테이션**: 최대 4개의 API 키를 순환 사용하여 호출 제한 회피

#### 2. 성능 최적화 - 멀티 레벨 캐싱 전략
- **Redis 기반 분산 캐싱**
  - Spring Cache Abstraction을 활용한 `@Cacheable` 어노테이션 기반 캐싱
  - 데이터 특성별 차등 TTL 적용
    - 프로필: 1시간 (변경 빈도 낮음)
    - 매치: 10분 (높은 실시간성 요구)
    - 통계: 30분 (중간 수준)
    - 메타데이터: 24시간 (변경 빈도 매우 낮음)
  - Redis 연결 실패 시 Caffeine fallback 자동 전환으로 무중단 서비스 보장
- **데이터베이스 캐싱**
  - `SearchHistory` 테이블을 통한 닉네임 → OUID 매핑 영구 캐시
  - 반복 검색 시 외부 API 호출 100% 제거
  - 비동기 저장(`@Async`)으로 응답 속도 향상
- **프론트엔드 캐싱**: 메모리 캐시(1시간 TTL) 및 디바운싱(500ms) 적용

#### 3. 병렬 API 호출 최적화
- **CompletableFuture 활용**
  - 4개의 외부 API를 동시 호출하여 대기 시간 최소화
  - 순차 호출 대비 응답 시간 **75% 단축** (2-3초 → 0.5-0.8초)
  - 부분 실패 허용으로 서비스 안정성 확보
- **지연 로딩(Lazy Loading)**: 프로필 조회 시 매치 정보 자동 조회 제거로 초기 로딩 시간 1-2초 단축

#### 4. 트래픽 제어 및 안정성
- **Rate Limiting (Bucket4j)**
  - IP 기반 Token Bucket 알고리즘 구현
  - 익명 사용자: 분당 100회, 인증 사용자: 분당 500회
  - DDoS 및 과도한 요청 방지
- **외부 API Rate Limiting**
  - 슬라이딩 윈도우 방식으로 초당 8회 제한
  - 429 에러 발생 시 자동 재시도 및 API 키 로테이션
- **예외 처리 및 폴백 전략**
  - 외부 API 실패 시 DB에 저장된 최신 데이터 활용
  - 캐시 → DB → 기본값 순서의 다단계 폴백 구조

#### 5. 모니터링 및 운영
- Spring Actuator를 통한 시스템 메트릭 수집
- `/api/metrics/cache` 엔드포인트로 캐시 히트율 실시간 모니터링
- 목표 캐시 히트율 80% 이상 유지

### 성과 및 개선 효과

#### API 호출량 감소
- 검색 API: 반복 검색 시 **100% 감소** (DB 캐시 활용)
- 프로필 API: 병렬 처리 및 지연 로딩으로 **60-80% 감소**
- 전체 예상: **60-80% API 호출량 감소**

#### 응답 속도 개선
- 검색(캐시 히트): **10-50ms** (기존 200-500ms 대비 약 **90% 개선**)
- 프로필 조회: **75% 시간 단축** (2-3초 → 0.5-0.8초)
- 초기 로딩: 매치 자동 조회 제거로 **1-2초 단축**

#### 안정성 향상
- 외부 API Rate Limit 초과 오류 대폭 감소
- 피크 시간대에도 응답 속도 및 안정성 유지
- Redis 장애 시에도 Caffeine fallback으로 무중단 서비스 제공

### 핵심 학습 경험
이 프로젝트를 통해 백엔드 개발자가 단순히 API를 연결하는 역할이 아니라, **외부 의존성과 트래픽 변동을 고려해 시스템을 통제하고 안정화하는 역할**임을 실무적으로 이해하게 되었습니다. 특히 캐싱 전략 수립, Rate Limiting 구현, 폴백 전략 설계 등 프로덕션 환경에서 필수적인 기술들을 직접 설계하고 구현하며 실전 경험을 쌓을 수 있었습니다.

---

## Data Crawling Website – 게임 데이터 수집 및 시각화

**프로젝트 기간**: 2024년  
**역할**: 크롤링 서버 및 API 서버 개발  
**기술 스택**: Python FastAPI, Playwright, Node.js/Express, Docker Compose  
**GitHub**: https://github.com/study-withme/data-crawling-website

### 프로젝트 개요
웹 크롤링 기반 게임 데이터 수집 및 대시보드 시각화 웹 서비스입니다. 동적 웹 페이지 크롤링, 데이터 처리, API 제공, 시각화까지 전 과정을 구현했습니다.

### 핵심 구현 내용

#### 1. 웹 크롤링 자동화
- **Playwright 활용**
  - 동적 웹 페이지 크롤링 구현 (JavaScript 렌더링 완료 후 데이터 수집)
  - Selenium 대비 더 빠른 성능과 안정성 확보
  - 헤드리스 브라우저 모드로 리소스 최적화
- **스케줄링 및 자동화**
  - 주기적 데이터 수집 자동화 (Cron 기반 스케줄링)
  - 에러 발생 시 자동 재시도 로직 구현
  - 데이터 중복 방지 및 증분 업데이트 로직

#### 2. 마이크로서비스 아키텍처
- **Python FastAPI 기반 데이터 제공 API 서버**
  - 크롤링된 데이터를 RESTful API로 제공
  - 비동기 처리로 높은 처리량 확보
  - OpenAPI 문서 자동 생성
- **Node.js/Express 기반 웹 UI 서버**
  - 대시보드 및 시각화 기능 제공
  - API 서버와 분리하여 독립적 개발 및 배포 가능
- **서비스 간 통신**: HTTP REST API를 통한 느슨한 결합

#### 3. Docker Compose 멀티 서비스 환경
- **컨테이너 구성**
  - 크롤링 서버, API 서버, 웹 서버를 각각 Docker 컨테이너로 구성
  - 서비스 간 네트워크 연결 및 의존성 관리
  - 환경 변수를 통한 설정 관리
- **개발/프로덕션 환경 일관성**
  - Docker Compose를 통한 로컬 개발 환경 구성
  - 프로덕션 배포 시에도 동일한 환경 보장

#### 4. 데이터 시각화
- 수집된 게임 데이터를 대시보드 형태로 시각화
- 실시간 데이터 업데이트 및 통계 정보 제공
- Chart.js 등을 활용한 인터랙티브 차트 구현

### 성과 및 학습 경험
- 동적 웹 크롤링의 기술적 이해 및 구현 경험
- 마이크로서비스 아키텍처의 실무 적용
- Docker를 활용한 멀티 서비스 환경 구성 경험

---

## 기술 역량 요약

### 아키텍처 설계
- 마이크로서비스 분리 설계 (Java-Python, Python-Node.js)
- 서버 간 통신 설계 (HTTP REST API)
- 확장 가능한 시스템 구조 설계

### 성능 최적화
- 멀티 레벨 캐싱 전략 (Redis + DB + Frontend)
- 병렬 처리 (CompletableFuture)
- 비동기 프로그래밍 (`@Async`, CompletableFuture)

### 외부 API 통합
- Rate Limiting (Bucket4j, 커스텀 구현)
- 에러 핸들링 및 재시도 로직
- API 키 로테이션

### 인프라 및 DevOps
- Docker, Docker Compose를 활용한 멀티 서비스 환경
- 실제 배포 경험 (Cloudtype)
- 모니터링 및 메트릭 수집 (Spring Actuator)

### 데이터 처리
- 웹 크롤링 자동화 (Playwright)
- 데이터 가공 및 변환
- 추천 알고리즘 구현 (벡터화, 코사인 유사도)

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
