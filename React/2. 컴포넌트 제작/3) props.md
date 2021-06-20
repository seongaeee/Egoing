## props

<br>

> `props`란 부모 컴포넌트가 자식 컴포넌트에게 주는 값

> 자식 컴포넌트는 받아온 props를 직접 수정할 수 없다.

우리는 props를 써서 리팩토링(결과 변화 없이, 가독성이나 유지보수 높임)을 할 수 있다.

쉽게 말하면, 하나의 컴포넌트를 다양하게 쓸 수 있게 되어 재활용성이 높아졌다.

다음의 예시로 이해해보자.

```java
class Subject extends Component {
  render() {
    return (
      <header>
        <h1>{this.props.title}</h1>
        {this.props.sub}
      </header>
    );
  }
}
```

```java
class App extends Component {
  render() {
    return (
      <div className="App">
        <Subject title="WEB" sub="world wide web!"></Subject>
        <Subject title="React" sub="For UI"></Subject>
      </div>
    );
  }
}
```
