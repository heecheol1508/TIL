## 타입스크립트로 전환해보기 (Porting)

<br/>

그리고 그 과정에서 생각해 볼 것들

- 타입스크립트와 자바스크립트가 얼마나 다른지
- 타입스크립트로 앱을 전환하면서 코드상에서 얼마나 더 유용한 기능들을 사용할 수 있게 되는지

<br/><br/>



#### 1. Typescript 환경 설정

JavaScript로 프로그래밍하면서는 index.html, app.js 만으로도 모던 웹 개발이 가능하도록 parcel.js라는 번들러가 거의 다 만들어줬음. Typescript 프로그래밍에서도 parcel.js를 사용할 수 있지만, 조금의 설정과 셋업이 필요.

<br/>

`tsconfig.json` 

typescript는 트랜트파일러여서 브라우저에서 실행시키려고 하면 자바스크립트로 변환시켜야 하는데, 자바스크립트로 변환하는 과정(컴파일)에서 여러 옵션을 줄 수 있음.

[tsconfig.json overview](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html)

[tsconfig.json compiler options](https://www.typescriptlang.org/tsconfig)

[tsconfig.json (번역)](https://typescript-kr.github.io/pages/tsconfig.json.html)

대부분의 설정은 기본값을 가지고 있고, 변경할 부분만 작성하면 된다^^

<br/>

<br/>



#### 2. 변수에 타입 작성하기



타입을 작성 두 가지 방법 : 타입 알리아스, 인터페이스



타입 추론, 타입 가드

