````markdown
# SurveyPulse 글로벌 서비스 모듈

마이크로서비스 전반에서 공통으로 사용되는 기능들을 모듈화하여 JitPack을 통해 배포하는 글로벌 서비스 라이브러리입니다.

## 주요 기능 모듈

### 1. 인증 및 인가 (Security)
- **Spring Security 설정**
- **JWT 지원**
  - JWT 생성/검증 컴포넌트 제공
- **login filter 기능**

### 2. 글로벌 예외 처리기
- **공통 예외 계층**
  - `BaseException` 추상 클래스 및 `ExceptionType` 인터페이스 정의
- **`@ControllerAdvice` 기반 핸들러**
  - `GlobalExceptionHandler` 클래스 제공
  - HTTP 상태 코드, 에러 코드, 메시지, 타임스탬프 등을 일관된 형식으로 응답

