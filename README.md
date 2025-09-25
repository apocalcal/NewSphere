# 📰 NewSphere – 뉴스 수집 및 검색 플랫폼

## 📄 프로젝트 개요
- **진행 기간**: 2025.07.18 ~ 2025.09.10  
- **프로젝트 설명**:  
  MSA(Micro Service Architecture) 기반 뉴스 플랫폼 구축 프로젝트.  
  뉴스 크롤링, 개인화 추천, 뉴스레터, 스크랩, 뉴스 요약 기능을 구현하며,  
  CI/CD 및 클라우드 배포까지 실무 환경과 유사한 경험을 진행했습니다.  

---

## 👤 담당 역할 (이채희)
- **회원 서비스 및 인증**
  - JWT 기반 회원가입/로그인, 마이페이지 구현
  - HttpOnly 쿠키 인증 방식 적용 → XSS 공격 대응
  - Google/Kakao OAuth 소셜 로그인 연동 (뉴스레터 기능과 연계)

- **보안 및 인프라 구축**
  - Config Service: 공통 환경변수 및 JWT 키 중앙 관리
  - Discovery Service (Eureka): 마이크로서비스 동적 등록/발견
  - Gateway Service: API Gateway를 통한 인증/라우팅/로드밸런싱
  - Swagger 연동: API 문서 자동화 및 팀 협업 효율화

- **DevOps 경험**
  - Jenkins + AWS 기반 CI/CD 파이프라인 참여
  - Docker Compose를 활용해 개발·테스트 환경 표준화

---

## 📊 기여 성과 (Troubleshooting 중심)

### 🔐 보안 강화
- **문제**: OAuth2 소셜 로그인 과정에서 JWT 토큰이 URL/LocalStorage에 노출 → XSS 공격 위험  
- **해결**: HttpOnly 쿠키 방식으로 전환, 클라이언트 접근 차단  
- **결과**: 로그인 편의성과 보안성을 동시에 확보, 사용자 신뢰도 향상  

### 🐳 환경 표준화
- **문제**: 팀원별 PC 환경 차이로 서비스 실행 시 충돌 발생  
- **해결**: 각 서비스별 Dockerfile 작성 + Docker Compose 도입  
- **결과**: 명령어 한 줄로 동일한 환경 재현 가능, 협업 효율성·안정성 확보  

### 🌐 확장성 있는 인프라 구축
- Gateway, Discovery, Config 서비스를 직접 구축  
- 서비스 간 유연한 확장 및 운영 효율성 확보  

### 🚀 실무 수준의 DevOps 경험
- Jenkins + AWS 기반 CI/CD 파이프라인 참여  
- 코드 작성 → 빌드/테스트 → 자동 배포까지 엔드투엔드 사이클 경험  

---

## 💭 개인 회고
이번 프로젝트에서 저는 **회원 서비스와 보안/인프라 전반**을 담당하며,  
단순 기능 구현을 넘어 **서비스 안정성과 협업 효율성**을 높이는 문제 해결 경험을 할 수 있었습니다.  

특히,  
- HttpOnly 쿠키 인증 방식으로 전환 → **실제 보안 취약점 대응 경험**  
- Docker Compose 도입 → **팀 협업 생산성 향상**  
- OAuth 소셜 로그인 연동 → **뉴스레터 기능과의 서비스 연계 강화**  

이 과정을 통해 **문제 상황을 발견 → 원인 분석 → 해결책 설계 → 결과 검증**의 사이클을 실무에 가깝게 경험했습니다.  
이는 단순한 개발 능력을 넘어, **안정적인 서비스 아키텍처 설계와 문제 해결 역량**을 갖춘 개발자로 성장하는 데 중요한 밑거름이 되었습니다.  

---

## 🛠 Tech Stack
- **Backend**: Java, Spring Boot  
- **Infra**: Spring Cloud (Config, Gateway, Discovery), Swagger  
- **Auth**: JWT, HttpOnly Cookie, Google OAuth, Kakao Login  
- **DevOps**: Jenkins, Docker, Docker Compose, AWS (EC2, S3, RDS)  
- **Database**: MySQL  
