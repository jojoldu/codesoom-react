# 3. 코드숨 리액트 - 3주차

왜 `getByRole`은 있는데 `getById` 혹은 `getByName`이 없나하고 한참 시간을 보내다가 아래 [Stackoverflow 답변](https://stackoverflow.com/questions/53003594/find-element-by-id-in-react-testing-library) 을 보고 이해하게 됐다.

![so1](./images/so1.png)

프론트엔드에서는 `id`와 `name` 같은 속성이 **세부 구현 사항이기 때문에** 테스트 검증에 사용되어서는 안된다는 것이다.  

좋은 테스트는 세부 구현 사항을 검증하는 것이 아니라, 명세를 검증해야 한다.  

* [테스트 코드에서 내부 구현 검증 피하기](https://jojoldu.tistory.com/614)

나는 프론트엔드의 세부 구현 사항이 **속성이 될거라곤 생각을 못했다**.  

getByRole에서 얘기하는 Role 은 aria를 따른다는 것도 몰랐다.

* [html-aria](https://www.w3.org/TR/html-aria/#docconformance)

그래서 테스트를 작성할때마다 이 문서를 계속 보고 하곤 하는데, IDE에서 자동지원 안되나 하는 생각도 들었다.  

과제의 아쉬운 점은 아무래도 **컴포넌트의 모든 이벤트가 App에서 넘겨준 함수를 실행**하는 것 밖에 없다보니 검증할만한게 없다는 것이 아쉬웠다.  

예를 들어 `Input` 컴포넌트의 기능을 검증하려고 하면, `onClick` 과 `onChange`를 검증하고 싶은데, 이게 어차피 호출자에서 넘겨준 함수를 실행하는것에 그치기 때문에 **실행되나 검증**만 할 뿐이다.  
아마 과정이 계속 진행되면서 컴포넌트의 이벤트들도 다 App에서 분리되지 않을까 예상해본다.
