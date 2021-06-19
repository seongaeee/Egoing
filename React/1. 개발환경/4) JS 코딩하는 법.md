# JS 코딩하는 법

<br>

## 폴더 구조

#### public 폴더

`component`들은 index.html의 `<div id="root"></div>`안에 들어간다.

<br>

#### src 폴더

`component`들을 만들고 수정한 파일이 있는 폴더이다. 개발 작업의 대부분은 파일은 src폴더에 넣는다.  

<br>

- index.js

`document.getElementById('root')`을 보면 위에서 설명한 것처럼 id가 root인 부분에 들어가게 되는것을 알수있다.

`<App />`부분이 컴포넌트가 들어갈 자리이고, ./App,js파일에 컴포넌트 내용이 있다.

- App.js

다음과 같이 클래스 타입으로 변경하자.

코드는 하나의 태그(`<div className="App"></div>`)로 감싸져야한다.

<img src="https://user-images.githubusercontent.com/62600984/122643511-21844100-d14b-11eb-97f2-9e9c338a8f31.png" width=700>
