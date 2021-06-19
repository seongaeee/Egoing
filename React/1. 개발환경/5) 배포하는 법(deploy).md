# 배포하는 법(deploy)

<br>

#### 기존 방식

리액트 페이지를 로드하면 아래와 같이 1.7MB 용량이 다운받아진다.

이는 `npm run start`를 통해 개발환경에서 리액트를 실행시켰기 때문이다.

<img src="https://user-images.githubusercontent.com/62600984/122643607-a1aaa680-d14b-11eb-8485-eab6a6d2ee6e.png" width=700>

<br>

#### build

아래의 명령어를 입력해보자.

```
npm run build
```

그 후에 `build`라는 폴더가 생긴다. 해당 폴더에 있는 파일은 불필요한 것을 제거시켜서 용량이 줄어든다.

실제로 서비스할때는 build의 파일을 쓴다.

<br>

#### build 파일 실행

build를 실행시키기 위해 다음과 같은 명령어를 입력하면 된다.

```
npx serve -s build
```

리액트 페이지를 로드하면 아래와 같이 147kB 용량이 다운받아진다. 기존 개발환경에서 실행시켰을때보다 훨씬 줄어든 용량이다.

<img src="https://user-images.githubusercontent.com/62600984/122643615-acfdd200-d14b-11eb-89b0-0adf227fdf0c.png" width=700>
