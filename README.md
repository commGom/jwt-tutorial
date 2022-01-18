# jwt-tutorial
[Inflearn JWT Video(5)](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8-jwt/dashboard, "JWT Inflearn Lecture link")

## 1. JWT 소개, 프로젝트 생성 및 Controller Test
### JWT
- Header : 시그니처 해싱하기 위한 알고리즘 정보
- Payload : 시스템 실제 사용하는 정보
- Signature : 토큰의 유효성 검증을 위한 문자열

장점 :
1. 중앙의 인증서버, 데이터 스토어에 대한 의존성 없음, 수평확장 용이
2. Base64 URL Safe Encoding 방식으로 URL, Cookie, Header에 모두 사용 가능한 범용성

단점
1. 페이로드에 담는 정보가 많아지면 트래픽의 크기가 커질 수 있다(고려할 요소)
2. 각 토큰은 클라이언트에 저장, 서버가 직접 조작하지 못한다.

### 프로젝트 생성 (gradle 의존성 주입)
- Spring Web
- Lombok
- Spring Security (Security로 인한 환경 설정 별도 필요)
- H2Database
- Spring Data Jpa
- Validation
- DevTools

