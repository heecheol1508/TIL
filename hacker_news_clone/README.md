## Hacker News Clone



##### START

![image-20210722210030627](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/00.jpg)





##### AJAX 사용하기

![image-20210722210349115](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/01.jpg)





##### 화면 전환하기

![image-20210722213615207](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/02.jpg)

- hashchange 이벤트로 content 가져오기





##### 현재 코드 문제점 & 해결 방안

- 코드의 실행 결과로써 UI를 만들었는데, 코드만 봐서는 마크업이 완성된 UI의 구조를 파악하기 어렵다.
- 코드가 훨씬 더 늘어나고 복잡해진다면, 그때는 거의 불가능할 듯
- DOM API를 이용해서 UI의 구조가 잘 드러나지 않는 문제점을 해결하는 가장 쉬운 방법은 DOM API 사용을 줄이는 것





##### DOM API 제거하기 (문자열 사용하기)

![image-20210723131337382](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/03.jpg)

- 임시 div 활용 (이전보다 나아졌지만 여전히 DOM API 존재)
- 중복 코드 제거 (함수 만들기)





##### 두 개의 화면으로 나누기 (내용 & 목록)

![image-20210723133526447](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/04.jpg)

- 한 번에 한 화면만 보여주는 구조를 위해, container에 추가하는 것이 아닌, 덮어쓰는 방법으로 구조 구축
- DOM API 제거 및 li 요소의 반복을 적용한 문자열을 만들기 위해, 배열 사용하기





##### 함수 분리 및 라우터 작성

![image-20210723134733052](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/05.jpg)

- 중복 제거 및 재사용을 위한 함수 분리
- 라우터 구현 (with location.hash)





##### 페이징 구현

![image-20210723144700786](https://github.com/heecheol1508/TIL/blob/master/hacker_news_clone/images/06.jpg)

- 현재 페이지 정보 등을 저장할 객체 생성
- 라우터에서 페이지와 아이디를 비교할 수 있도록 수정
- getData와 lastPage 등 개선 필요





