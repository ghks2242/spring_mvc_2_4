# spring_mvc_2_4
로그인처리 쿠키 세션

---

### 패키지 구조설계 

패키지 구조
* hello.login
  * domain
    * item
    * member
    * login
  * web
    * item
    * member
    * login

도메인이 가장중요하다
도메인 = 화면,UI 기술 인프라 등등의 영역은 제외한 시스템이 구현해야 하는 핵심 비즈니스 업무 영역을 말함

향후 WEB 을 다른 기술로 바꾸어도 도메인은 그대로 유지할 수 있어야한다.
이렇게 하려면 WEB 은 domain 을 알고있지만 domain은 web을 모르도록 설계해야한다. 이것을 web 은 domain을 의존하지만 
domain은 web을 의존하지 않는다고 표현한다. 예를들어 web 패키지들을 모두 삭제해도 domain 에는 전혀 영향이 없도록 의존관계를 설계하는것이 중요하다 
반대로 이야기하면 domain 은 web을 참조하면안된다.


