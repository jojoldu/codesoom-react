# 4. 코드숨 리액트 - 4주차

## 1. 학습 내용

Redux 를 배우기 시작했다

### Flux Architecture

* Action
* Dispatcher
* Store
* View

Flux는 MVC와 다르게 단방향으로 데이터가 흐른다.
React view에서 사용자가 상호작용을 할 때, 그 view는 중앙의 dispatcher를 통해 action을 전파하게 된다.  
어플리케이션의 데이터와 비지니스 로직을 가지고 있는 store는 action이 전파되면 이 action에 영향이 있는 모든 view를 갱신한다.  
이 방식은 특히 React의 선언형 프로그래밍 스타일 즉, **view가 어떤 방식으로 갱신해야 되는지 일일이 작성하지 않고서도 데이터를 변경**할 수 있는 형태에서 편리하다.

### Redux

* Store
* Reducer
  * 상태를 다른 상태로 변경하는데 사용되는 것
  * 최초 상태를 같이 넣어주는 경우가 많다

아샬님의 강의가 React가 생전 처음인 사람에겐 어렵다고 생각할 수도 있을것 같았다.  
그런분들에겐 생활코딩 이고잉님의 Redux 강좌를 추가적으로 듣는 것도 좋은 방법이라고 생각했다.

* [생활코딩 - Redux](https://www.inflearn.com/course/redux-%EC%83%9D%ED%99%9C%EC%BD%94%EB%94%A9/dashboard)


## 2. 과제 & 코드리뷰



## 3. 회고
