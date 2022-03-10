# Parameter Passing Techniques in java

## 1. Caller 와 Callee function

파라미터는 함수에  데이터가 들어가고 출력되는 것에 따라 다양한 방법이 존재하는데, 아래처럼 함수 B가 함수 A에 의해서 호출되는 상황이 있을 수 있다.
이때, `함수 A를 caller function(호출자 함수)`, `함수 B를 callee function(피호출자 함수)`라고 할 수 있다

```java
public void A(B()){
~~~
}
```

### 1-1. Types of parameters(파라미터의 유형)

파라미터의 형태는 어떻게 전달되는지 그 형태도 상이할 수 있다
이 부분은 그 유형 중 일부가 마치 `1`에서 언급된 내용과 겹쳐질 수 있기 때문에 소분류로 분류하였다

차이점은 `변수` 가 파라미터로 제공되었는지,  `함수`가 파라미터로 제공되었는지가 가장 큰 가시적인 차이점일 것이다

1️⃣ Formal Parameter

-  `파라미터의 타입`과 `파라미터의 변수명` 이 가시적으로 보이는 형태의 파라미터

```java
eat(Food food);
```

2️⃣ Actual Parameter

- `함수의 파라미터로 함수가 제공되는 형태`

```java
eat(getFoodName());
```


## 2. Parameter Passing(메서드의 파라미터 전달 방식)

1️⃣ Pass By Value(Call By Value)

- 함수의 파라미터에 값만 전달하는 방식


2️⃣ Call By Reference(Aliasing)

- 자바의 참조형 변수(문자열, 객체)에 해당되는 방식
- 주소값을 참조해서 값이 전달되는 방식
