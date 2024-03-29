## Hacker News Clone



##### START

![image-20210722210030627](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/00.jpg)

<br/><br/>



##### AJAX 사용하기

![image-20210722210349115](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/01.jpg)

<br/><br/>



##### 화면 전환하기

![image-20210722213615207](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/02.jpg)

- hashchange 이벤트로 content 가져오기

<br/><br/>



##### 현재 코드 문제점 & 해결 방안

- 코드의 실행 결과로써 UI를 만들었는데, 코드만 봐서는 마크업이 완성된 UI의 구조를 파악하기 어렵다.
- 코드가 훨씬 더 늘어나고 복잡해진다면, 그때는 거의 불가능할 듯
- DOM API를 이용해서 UI의 구조가 잘 드러나지 않는 문제점을 해결하는 가장 쉬운 방법은 DOM API 사용을 줄이는 것

<br/><br/>



##### DOM API 제거하기 (문자열 사용하기)

![image-20210723131337382](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/03.jpg)

- 임시 div 활용 (이전보다 나아졌지만 여전히 DOM API 존재)
- 중복 코드 제거 (함수 만들기)

<br/><br/>



##### 두 개의 화면으로 나누기 (내용 & 목록)

![image-20210723133526447](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/04.jpg)

- 한 번에 한 화면만 보여주는 구조를 위해, container에 추가하는 것이 아닌, 덮어쓰는 방법으로 구조 구축
- DOM API 제거 및 li 요소의 반복을 적용한 문자열을 만들기 위해, 배열 사용하기

<br/><br/>



##### 함수 분리 및 라우터 작성

![image-20210723134733052](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/05.jpg)

- 중복 제거 및 재사용을 위한 함수 분리
- 라우터 구현 (with location.hash)

<br/><br/>



##### 페이징 구현

![image-20210723144700786](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/06.jpg)

- 현재 페이지 정보 등을 저장할 객체 생성
- 라우터에서 페이지와 아이디를 비교할 수 있도록 수정
- getData와 lastPage 등 개선 필요

<br/><br/>



##### 현재 코드 문제점 & 해결 방안

- 문자열 방식으로 UI 구조 파악이 조금은 쉬워졌지만, 배열로 되어있다보니 코드가 분리되어있고, 양이 늘어나다보면 또 파악이 어려워질 것이다.
- 템플릿 방식으로 바꿔보기 (틀을 만들어두고 채워넣는 느낌)

<br/><br/>



##### 템플릿 활용

![image-20210803134609183](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/07.jpg)

- 코드와 UI의 성격이 다르기 때문에 분리해주면 복잡도를 줄일 수 있음

<br/><br/>



##### tailwindcss 사용하기

![image-20210803140253274](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/08.jpg)

<br/><br/>



##### 댓글, 대댓글, 대대댓글 처리하기

![image-20210809121009143](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/09.jpg)

<br/><br/>



##### 읽은 글 표시하기

##### 마지막 페이지 설정하기



끝
