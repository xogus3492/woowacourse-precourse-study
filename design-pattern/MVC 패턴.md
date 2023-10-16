## 등장 배경

MVC 등장 이전에는 프로그래머들이 개발을 하면서 코드가 많아지고 복잡해질수록 점점 유지보수가 힘들어져서 이러한 유지보수가 힘들어지는 문제에 대한 대책으로 MVC라는 패턴을 개발함

## 동작 과정 단순화

<img width="1178" alt="Untitled" src="https://github.com/xogus3492/woowacourse-precourse-study/assets/77439799/6197bd65-670f-4d2f-9d45-074ab54415b2">


 - Model : 데이터와 관련된 부분

 - View : 사용자에게 보여지는 부분

 - Controller : Model과 View의 중개 역할을 하는 부분

## 설계 규칙

1. Model은 View와 Controller에 의존하지 않아야 한다. (Model 내부에 Controller와 View에 관련된 코드가 있으면 안됨)
2. View는 Model에만 의존해야 하고, Comtroller에는 의존하지 않아야 한다. (View 내부에 Model에 관련된 코드만 있어야 하고 Controller에 관련된 코드는 있으면 안됨)
3. View가 Model로부터 데이터를 받을 때는 사용자마다 다르게 보여줘야하는 데이터에 대해서만 받아야 한다. (사용자 모두에게 공통적으로 보여줘야하는 데이터에 대해서는 View가 자체적으로 가지고 있어야 함)
4. Controller는 Model과 View 모두에 의존해도 된다. (Controller 내부에 Model과 View에 관련된 코드를 포함할 수 있음)
5. View가 Model에 대한 데이터를 받을 때 반드시 Controller로부터 받아야 한다.
