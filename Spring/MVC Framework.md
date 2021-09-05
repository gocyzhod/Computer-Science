    Servlet 이란?
    자바로 웹을 만들기 위해 필요한 기술

    스프링의 동작원리

![image](https://user-images.githubusercontent.com/44426450/132116419-25192446-ecd8-4ff1-b137-85dc8d088cd1.png)


1. 클라이언트가 url 요청 - 웹 브라우저에서 스프링으로 request 가 보내진다.
2. Dispatcher Servlet 이 request 를 받는다 - Handler Mapping 을 통해 url 을 담당하는 Controller 를 탐색 후 찾아낸다.
3. 찾아낸 Coontroller 로 request 를 보낸다. 보내주기 위한 Model 를 구성한다.
4. Model 에서 페이지 처리에 필요한 정보들을 DB 에 접근하여 퀴리문을 통해 가져온다.
5. 데이터를 통해 얻은 Model 정보를 Controller 에게 reponse 를 보내준다. - Controller 는 이를 받아 Model 를 완성시켜 Dispatcher Servlet 에게 전달
6. Dispatcher Servlet 은 View Resolver 를 통해 request 에 해당하는 view 파일을 탐색 후 받아낸다.
7. 받아낸 view 페이지 파일에 Model 을 보낸 후 클라이언트에게 보낼 페이지를 완성시켜 받아낸다.

    Dispacher Servlet
   
모든 request 를 처리하는 중심 컨트롤러

기존에는 web.xml 에 모두 등록해줬어야 했지만, 디스패처 서블릿이 모든 request 를 관리하면서 작업을 편리하게 할 수 있다.

    Handler Mapping
    
클라이언트의 request url 을 어떤 컨트롤러가 처리해야 할지 찾아서 Dispacher Servlet 에게 전달해주는 역할

컨트롤러 상에서 url 을 매핑시키기 위해 @RequestMapping 을 사용하는데, 핸들러가 이를 찾아주는 역할을 한다.

    Controller
    
실질적인 요청을 하는 곳.

Dispatcher Servlet 이 프론트 컨트롤러라면, 이곳은 백엔드 컨트롤러라고 볼 수 있다.

모델의 처리 결과를 담아 Dispatcher Servlet 에게 반환하여준다.

    View Reslver
    
컨트롤러의 처리 결과를 만들 view 를 결정해주는 역할을 담당.

다양한 종류가 존재한다.
