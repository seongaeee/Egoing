## Component 파일로 분리하기

<br>

하나의 App.js에 모든 컴포넌트들을 넣으면 관리와 재활용성이 떨어진다. 이를 해결하기 위해 파일로 분리하자.

1. src 폴더안에 component 폴더를 만들기

2. 컴포넌트 파일 만들기

```java
import { Component } from "react";

class Content extends Component {
  render() {
    return ();
  }
}

export default Content;
```

3. App.js에 컴포넌트 import

```java
import Content from "./component/Content";
```
