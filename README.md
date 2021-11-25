# JavaScript

<br><br>

## 자료형

---

### 자료형이란?

<br>

- 어떤 종류의 데이터를 사용하는 것인지 컴퓨터에게 알려주는 것
- 자료형마다 사용 가능한 연산자(Operator)를 따로 가지고 있습니다.
- **자료형이 같아야 연산을 할 수 있습니다.**
  <br><br>

#### 자료형의 종류

```js
Number;
String;
Boolean;
Null;
Undefined;
```

<br>
그리고 하나 더 객체가 있습니다.
<br><br>

```js
Object;
```

---

#### Number Type

<br>
정수와 실수 모두 Number 타입입니다.

```js
5;
3.0;
-4.8;
```

<br>

#### 숫자의 연산자

<br>
사칙연산, 괄호, 나머지 등이 있습니다.

```js
 +, -, /, *, ( ), %
```

<br>

#### 문자열

<br>

```js
"I am String";
"Hello" + "World";
```

<br>
문자열에도 +가 됩니다. (참고로 문자열은 "Immutable" 특징을 가집니다.)
<br>
<br>

#### typeof 연산자

<br>
데이터 유형을 알려주는 중요한 연산자
<br><br>

```js
typeof 5;
("number");
typeof -4.8;
("number");
typeof "5";
("string");
```

<br>

#### Boolean

<br>

```js
true;
false;
5 > 3;
false;
5 == 5;
true;
5 > 5;
false;
```

<br>

#### 논리 연산자

<br>
논리 연산자에는 &&, ||, ! 등이 있습니다.
<br><br>

```js
true;
!true;
true && false;
false;
true || false;
true;
```

<br>

---

## 변수

<br>

### 변수란?

<br>

**데이터(값)를 담을 수 있는 그릇**입니다.
데이터들은 컴퓨터의 메모리의 어딘가에 저장되는데 그 **값들을 구별짓고 재사용하기 위해서** 변수를 씁니다.
<br>
<br>

### 변수 선언하기

<br>
변수를 사용하기 위해서는 먼저 선언이 필요합니다.
<br><br>

```js
var a;
```

---

### 변수와 대입 연산자

<br>
변수에 값을 넣고 싶을 때 `=` 연산자를 사용합니다. `=`은 수학에서의 같다가 아니라 변수에 값을 할당할 때 사용하는 대입 연산자입니다. 같다는 `===` 를 주로 사용합니다.
<br><br>

### 변수 사용하기

<br>
여러가지 방식이 있습니다.
<br><br>

```js
var a = 7;
var b = 10;
var c = a + b; //17
```

<br>

### 변수 이름 잘 짓기

<br>
변수의 이름은 매우 중요합니다. 일반적으로 소문자로 시작해, 영어, 숫자 `_`를 주로 사용합니다. 카멜 케이스나 스네이크 표기법을 사용합니다.
<br><br>

#### 카멜 케이스

<br>

> numPeople

<br>

#### 스네이크 케이스

<br>

> num_people

---

<br>

## 연산자 및 기타

<br>

### 증감 연산자

<br>

```js
var a;
a++;
a = 0;
a++;
1;
a--;
0;
```

<br>

### 비교 연산자

<br>
비교 연산자를 수행한 결과값은 Boolean입니다. 비교 연산자에는 `>, <, >=, <=, ===, !=` 등이 있습니다.
<br><br>

```js
var a = 3;
var b = 5;
var c = "5";
a > b;
false;
a < b;
true;
b === c;
false;
```

<br>

### 문자열의 길이 구하기

<br>

```js
var a = "hello";
a.length;

5;
```

<br>
`.`연산자는 객체의 속성을 가져올 때 사용하는 연산자입니다.

<br><br>

### 문자열 간단히 조작하기

<br>

```js
var a = "KheLLo";
a[0];
("K");
a[1] = "H"; //안 됨
a.slice(1, 4);
("heL");
a.toUpperCase();
("KHELLO");
a.toLowerCase();
("khello");
```

<br>

### undefined, null, NaN

<br>

- undefined : 값이 정의되지 않았다.
- null : 값이 비어있다.
- NaN(Not a Number) : 값이 아니다. === 계산 불가능

### console.log()

<br>
개발자 콘솔에 뭔가를 찍어주는 메소드입니다.
<br><br>

```js
var a = 1;
var b = "더하기";
var c = 2;
console.log(a + " " + b + " " + c + " = " + a + c);
1 더하기 2 = 12
```

<br>

### alert()와 prompt() 사용해 보기

<br>

```js
var ans = prompt("How are you?");
alert(ans);
```

---

## 조건문

<br>
조건에 따라 다른 행동을 취해야 할 때, `if`문과 조건부 연산자 `?`를 사용하면 됩니다.
<br><br>

### 'if'문

<br>

```js
if (조건식) {
  //조건식이 참일 경우 실행될 구문
}
```

- `{}`는 생략할 수 있지만 꼭 쓰는게 좋습니다.
- indent(들여쓰기)를 해야 합니다.
  <br><br>

### if + else 문

<br>

```js
if (조건식) {
  //조건식이 참일 경우 실행될 구문
} else {
  //조건식이 거짓일 경우 실행
}
```

<br>

### if + else if + else

<br>

```js
if (조건식1) {
  //조건식이 참일 경우 실행
} else if (조건식2) {
  //조건식1은 거짓이고 2는 참일 경우
} else {
  //거짓일 경우 실행
}
```

<br>

## While 반복문

<br>
반복문은 비슷한 일을 반복적으로 처리하기 위한 명령문입니다.
<br><br>

```js
while (조건) {
  console.log("참일때 실행됨");
}
```

---

```js
var n = 1;
while (n <= 100) {
  console.log("Hi" + n);
  n++;
}
```

---

<br>

### 그래서 for가 등장함

<br>

```js
for (var i = 0; i <= 100; i++) {
  console.log(i);
}
```

### 추가 설명

<br>
반복문은 자주 사용하는 형태가 있습니다.
<br><br>

1. n 회 코드 실행
2. 특정 조건을 만족시킬 때까지 코드 실행
3. 배열 안의 원소들 각각에 대해 코드 실행
   <br><br>

## break 와 continue

<br>

<b>break는 반복문을 중간에 빠져나갈 때 사용합니다.</b> <br><br>

```js
var str;
while (true) {
  str = prompt("아무거나 입력하세요");
  document.write(str + "<br>");
  if (str == "q") {
    break;
  }
}
document.write("Bye~");
```

<br>

<b> continue는 반복문의 처음으로 돌아갑니다. </b> <br><br>

- while : 조건식 (i<10)으로 이동
- for : 증감식 (i++)으로 이동
  <br><br>

```js
for (var i = 0; i < 10; i++) {
  if (i == 5) {
    continue;
  }
  console.log(i);
}
```

<br>

## 이중 루프

<br>
반복문 안에 반복문이 있는 걸 이중 루프라고 합니다. 종종 사용합니다.
3중, 4중도 가능하지만 잘 사용하지 않습니다.
<br><br>

```js
for (var i = 0; i < 2; i++) {
  for (var j = 0; j < 3; j++) {
    console.log(i + ", " + j);
  }
}
```

<br><br>

---

<br><br>

# Switch case 문법

변수에 저장된 값에 따라 각각 다른 코드를 실행하는 분기문입니다. 상황에 따라 `if`와 `else if`를 반복적으로 써야 하는 상황을 피하게 해줍니다.

## 문법

```js
var value;
switch (value) {
  case 값1:
    //value == 값1일 경우 실행할 코드
    break;
  case 값2:
    //value == 값2일 경우 실행할 코드
    break;
  //...
  default:
  //위쪽에 해당되지 않는 경우 실행할 코드
}
```

## 예제

점수가 10점이면 A, 9점이면 B, 그 외에는 C를 출력하는 코드를 작성하세요.

### if로 구현

```js
var score = prompt("점수를 입력하세요");
if (score === 10) {
  console.log("A");
} else if (score == 9) {
  console.log("B");
} else {
  console.log("C");
}
```

### switch-case 로 구현

```js
var score = prompt('점수를 입력하세요');
switch (score) {
    case 10:
    console.log('A);
    break;
    case 9:
    console.log('B');
    break;
    default:
    console.log('C');
}
```

<br>

---

<br>

# 배열과 문자열

## 배열 (Array)

<br>
자바 스크립트에서 가장 많이 사용하는 <b>자료구조</b>의 하나로 <br>
주로 같은 종류의 값 여러 개를 묶어서 저장하고 관리하기 위해 사용합니다. <br>
참고로 자바스크립트의 배열은 객체입니다.
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array

## 배열 만들기

```js
var scores = [50, 60, 70];
console.log(scores);
console.log(scores.length);
```

## 인덱스를 이용해서 배열의 원소 읽기

```js
scores[0];
scores[3];
```

## 배열에 값 쓰기

```js
scores[0] = 100;
scores[9] = 50;
```

## 배열의 타입 알아보기

```js
typeof scores;
typeof scores[0];
```

## 배열 만들기 2

```js
var a = [];
a[0] = 2;
a[1] = 4;
```

## 배열의 길이 구하기

```js
scores.length;
```

## 배열의 마지막 원소 읽어오기

```js
scores[scores.length - 1];
```

## 문자열과 배열

- 문자열과 배열은 비슷한 성질을 많이 가지고 있습니다.
- 문자열: Immutable
- 배열: Mutable

## 배열의 메소드들

<b> push(), pop() </b>

- `push(value)` : 배열의 뒤 쪽에 새로운 원소를 삽입합니다.
- `pop()`: 배열의 마지막 원소를 빼서 변수에 넣어 줍니다. 이 때 변수의 길이는 1 감소합니다.
- 스택처럼 동작하는데 사용합니다.

<b> shift(), unshift() </b>

- `push`, `pop`과 반대로 동작합니다.
- `unshift(v)` : 배열의 맨 앞에 새로운 값을 추가합니다.
- `shift()` : 배열의 앞에서 값을 빼서 변수에 넣어 줍니다.

<br><br>

---

<br><br>

# 함수의 기초

## 함수란

수학의 함수와 상당히 유사합니다. 매개변수 -> (처리) -> 리턴값의 형태를 가집니다.

```js
f(x) = 2x + 3
f(2) = 7
f(3) = 9

var foo = function(x) {
  return 2 * x + 3;
}

var y = foo(2);
y = foo(3);
```

## 함수 만들기 1

매개 변수도 없고, 리턴값도 없는 가장 단순한 형태의 함수를 만들어 봅시다. 출력과 리턴은 전혀 다르다는 걸 기억하세요.

```js
var foo = function () {
  console.log("I am function");
};
```

## 함수 호출

함수를 사용하는 것을 함수 호출(call)이라고 합니다. <b?>함수 이름 + 괄호</b>가 필요합니다.

```js
foo();
```

## 매개변수가 있는 함수 정의하기

```js
var foo2 = function (name) {
  console.log("hello" + name);
};
```

## 매개변수가 있는 함수 사용해 보기

```js
foo2("honux");
```

# 함수와 리턴 값

## 리턴 값이 있는 함수 정의하기

리턴 값이 있을 경우 함수를 호출해서 변수에 값을 넣을 수 있습니다.

```js
var five = function () {
  return 5;
};

var n = five();
console.log(n);
//5
```

## 리턴이 없는 함수를 변수에 할당하면?

```js
var foo = function () {
  console.log(5);
};
var n = foo();
console.log(n);
//undefined
```

## 아무 값도 없는 리턴 사용하기

`return`으로 함수를 종료하는데 사용할 수 있다.

```js
var test1 = function (text) {
  if (text === "exit") {
    return;
  }
  console.log("보이나요?");
};

test1("hoho");
test1("exit");

//undefined
```

## 함수를 사용하면

- 가독성이 좋아짐
- 유지보수를 잘하게 됨
  <br><br>

## 함수 어떻게 만들까?

- 매개 변수와 리턴을 적극적으로 활용하자.
- 줄 수가 지나치게 길어지면 함수로 빼자. (10줄 정도)
- 인덴트가 지나치게 깊어져도 함수로 빼자.
- 함수는 반드시 한 가지 일만 하도록 하자.
  <br><br>

## 2중 루프를 한 번에 빠져 나가기

- `break` 명령은 한 번에 한 루프만 빠져나갑니다.
- 함수의 `return` 을 이용하면 2중 루프를 한 번에 종료할 수 있습니다.
  <br><br>

---

<br><br>

# 객체의 기초

## 객체란 무엇인가?

- 현실의 물체에 대응되는 개념입니다.
- 객체를 사용하면 변수와 함수를 묶어서 관리하게 됩니다.
- 객체는 속성과 메소드를 가집니다.
  <br><br>

## 객체 만들기

```
p1 = {};
```

## 속성

객체에 속한 변수

```js
p1.name = "Kim Hyeong Kyeom";
console.log(p1.name); //"Kim Hyeong Kyeom"
```

## 메소드

객체에 속한 함수

```js
p1.eat = function (food) {
  console.log(this.name + " ate delicious " + food + "...");
};

p1.eat("Beef");
// "Kim Hyeong Kyeom ate delicious Beef..."
```

## 메소드 대신에 일반 함수를 썼다면?

```js
eat(p1, "Beef");
```

의미가 모호해진다. <br><br>

## 객체 지향 프로그래밍

- 유지보수가 쉬워진다.
- 가독성이 높아진다.
- 대형 프로그램을 짜기 쉬워진다.
- 객체와 객체가 협력해서 일을 한다.
- 객체는 일에 책임을 진다.
- 객체는 객체에 메시지를 보낸다.
- 객체는 자율적으로 일을 한다.
  <br><br>

## this 키워드

메소드 안에서 사용시 함수를 소유한 객체를 가르킨다.

```js
var p2 = {};
p2.name = "crong";
p2.weight = 80;
p2.say = function (word) {
  console.log(this.name + " says, " + word);
};
// this = p2
```

## 객체 만들기 2

JSON 표기법을 이용해서 객체를 만들 수도 있습니다. 생성자 함수를 이용하는 방법도 있지만 다음에 다루겠습니다.

```js
var m1 = {
  name: "Honux",
  hp: 100,
  power: 10,
  attack: function (target) {
    target.hp -= this.power;
  },
};

var c1 = {
  type: "Coffee",
  energy: 10,
};

//m1.eat(c1);
```

## 배열의 메소드 더 살펴보기

### concat()

concat: 배열 합치기, 문자열도 가능

### join

배열을 문자열로 바꿀 때 사용합니다.

### indexOf(), lastIndexOf()

배열이나 문자열안의 원소를 가지고 인덱스를 찾을 수 있음

```js
var a = [10, 20, 30, 40, 10, 50];
a.indexOf(10); //0
a.indexOf(65535); //-1
a.lastIndexOf(10); //4
```

### slice()

사용법 : `slice(startIndex, endIndex)` 기존 배열을 잘라서 새로운 배열을 만듭니다. 기존 배열은 변하지 않습니다. starIndex 위치부터 endIndex 직전의 위치까지 자릅니다. endIndex의 원소는 포함되지 않습니다.

```js
a = [1, 2, 3, 4, 5];
a.slice(2, 4); //[3,4]
a; // [1, 2, 3, 4, 5]
```

### 문자열의 split()

문자열을 문자의 배열로 나누고 싶을 때 사용하는 메소드입니다.

```js
var s = "hello, world a-b-co, ltd";

s.split("");
//["h", "e", "l", "l", "o", ",", " ", "w", "o", "r", "l", "d", " ", "a", "-", "b", "-", "c", "o", ",", " ", "l", "t", "d"]

s.split(","); //["hello", " world a-b-co", " ltd"]

s.split("-"); //["hello, world a", "b", "co, ltd"]
```

<br>

---

<br><br>

# 객체의 생성자 살펴보기

### 생성자로 여러 객체를 쉽게 만들기

비슷한 객체를 여러 개 만들 때는 객체를 생성하는 함수를 이용합니다. 이 때 객체를 생성하는 함수를 생성자라고 합니다. 생성자는 관례상 대문자로 시작하는 경우가 많습니다.

```js
//휴면 클래스를 정의하는 함수 = 생성자
var Human = function (name, hp, power) {
  this.name = name;
  this.hp = hp;
  this.power = power;
  this.attack = function (target) {
    target.hp -= this.power;
  };
  this.show = function () {
    console.log("%s %d %d %d", this.name, this.hp, this.mp, this.power);
  };
};
```

## 생성자를 이용해서 객체 만들기

생성자를 이용해서 객체를 만들 때는 `new` 키워드를 사용합니다.

```js
var m1 = new Human("Honux", 100, 10);
var m2 = new Human("Crong", 999, 1);
m1.attack(m2);
m2.attack(m1);
m1.show();
m2.show();
```

위 코드에서 m1은 객체 또는 인스턴스라고 합니다. m1은 그리고 참조 변수입니다. 참조 변수에 대해서는 다음에 다시 설명합니다. <br><br>

## 생성자를 사용하는 이유

- 객체를 하나만 만들 때는 간단히 json 표기법으로 만듭니다.
- 여러 객체를 만들 때는 생성자를 통해서 만듭니다.

<br><br>

---

<br><br>

# 값에 의한 전달 이해하기

<br>

## 참조 변수와 일반 변수

<br>
객체를 변수에 할당하면 참조 변수가 되고, 기본 타입을 변수에 할당하면 일반 변수가 됩니다.
<br><br>

## 일반 변수에서 값 복사 및 바꾸기

<br>
일반 변수는 <b>값만</b> 저장하고 다른 변수에 언제나 독립적으로 존재합니다.
<br><br>

```js
var a = 5;
var b = a;
a === b; //true
b = 10;
a === b; //false
```

<br>
위 코드에서 a와 b는 처음에 값은 같지만 사실은 다른 변수입니다.
<br><br>

## 참조 변수의 동작 방식 이해햐기

<br>
참조 변수라는 것은 객체에 대한 별명 같은 것입니다. 같은 사람을 이름으로도 부르고, 별명으로도 부르고, 다양한 호칭으로 부르는 것과 조금 비슷합니다. 우리가 객체를 만들면 객체가 생기고 변수에는 그 객체의 참조를 할당하는 것입니다. 무슨 말인지 잘 모르겠죠? 이상하게 들리겠지만 아래 코드를 먼저 실행해 보세요.
<br><br>

```js
var m1 = { name: "honux", age: 25 };
var m2 = m1;
m1 === m2; // true
m2.name = "crong";
m1; // {name: "crong", age: 25}
m1 === m2; // true
```

<br>
일반 변수와는 전혀 다른 결과가 나왔죠? 왜 그런지는 나중에 저절로 알게 됩니다. 일단 이게 참조 변수구나하고 기억해 둡시다.
<br><br>

## 함수 호출시의 변수

<br>
두 코드의 동작 차이를 봅시다.
<br><br>

### 값 전달

<br>

```js
var foo_v = function (v) {
  v = v * 2;
  console.log(v);
};

var a = 10;
foo_v(a); // 20
console.log(a); // 10
```

<br>

### 참조 전달

<br>

```js
var foo_r = function (ref) {
  ref.v = ref.v * 2;
  console.log(ref);
};

var p = { name: "Dora", v: 99 };
foo_r(p); // {name: "Dora", v: 198}
console.log(p); // {name: "Dora", v: 198}
```

<br>

### 요약

<br>

- 값 전달 변수는 함수 내부에서 값을 바꿔도 외부에서는 그대로 입니다.
- 참조 전달 변수는 함수 내부에서 값을 바꾸면 외부의 객체도 값이 바뀝니다.

<br>

---

<br><br>

# Prototype

<br>
생성자로 만든 객체는 프로토타입이라는 속성을 가집니다. 자바스크립트로 객체 지향 프로그래밍을 하기 위해서는 프로토타입을 잘 이해해야 합니다. 일단 우리는 프로토타입을 이용해서 메소드를 생성하려 합니다. 이렇게 하면 메모리를 절약하고 효율적으로 객체의 메소드를 생성할 수 있습니다. 
<br><br>

[프로토타입 MDN 참조 링크](https://developer.mozilla.org/ko/docs/Learn/JavaScript/Objects/Object_prototypes)
<br><br>

```js
function Human(name, hp, mp, power) {
  this.name = name; //m1.name = name;
  this.hp = hp;
  this.mp = mp;
  this.power = power;
}

Human.prototype.attack = function (target) {
  target.hp -= this.power;
};
```

<br>

## 배열과 객체

<br>
객체의 속성값이 배열이 될 수 있습니다. 배열 안에 값들이 객체가 될 수 있습니다.
<br><br>

```js
var m1 = { no: 1, scores: [100, 99] };
var m2 = { no: 2, scores: [100, 99] };
var arr1 = [m1, m2];
```

<br>

## 배열, 객체와 참조변수

<br>
객체를 변수에 할당하면 그 변수는 참조 변수가 됩니다. 배열도 객체이므로 배열을 변수에 할당하면 역시 참조 변수가 됩니다. <b>함수 호출 시 참조 변수를 매개 변수로 전달하면 함수 내부에서 변경한 값이 외부에서도 변경된다는 것</b> 꼭 기억하세요.
<br><br>

---

<br>

# DOM과 HTML

<br>

## HTML

<br>

- HyperText Markup Language
- WWW의 3 요소 중 하나
- 팀 버너스리에 의해 만들어 졌다.
  <br><br>

## 엘리먼트(Element)

<br>

- 여는 태그와 닫는 태그로 이루어짐
- 태그 사이에 콘텐츠를 가짐
- 태그 안에 속성과 속성의 값을 가짐
- 닫는 태그가 없는 태그도 있다. (img, br, input)
  <br><br>

## 속성 (Attributes)

<br>
객체의 속성과 비슷하게 엘리먼트도 속성을 가질 수 있습니다.

```html
<a href="http://codesquad.kr" title="코드스쿼드"></a>
```

<br>

## 블록 엘리먼트

<br>

`p, h1, div` 처럼 줄이 바뀌는 엘리먼트
<br><br>

## 인라인 엘리먼트

<br>

`span, img, input, button, a` 처럼 줄바뀜이 없는 엘리먼트
<br><br>

---

<br>

# DOM(Document Object Model)

<br>

- 문서를 객체를 이용해서 계층 구조로 표현함
- 표준 : W3CDOM
- 구현체 : Gecko, Webkit 등
  <br><br>

## html 객체

<br>
HTML 문서도 객체로 간주된다.
<br><Br>

- window : 최상위 객체
- document : DOM의 최상위 객체면서 window의 하위 객체
  <br><br>

```
var list = document.getElementsByTagName('h1');
list[0].innerHTML;
list[0].innerHTML = "Hello";
```

<br>

```
var list = document.getElementById('main');
main.innerHTML = "Hello";
```

<br>

## JS로 DOM 제어하기

<br>
모든 HTML 엘리먼트는 객체이므로 다른 객체와 마찬가지로 JS로 제어가 가능합니다.
<br><br>

### DOM 객체의 값 바꾸기

<br>

```js
var element = document.getElementById("id");
element.innerHTML = "값";
```

<br>

```html
<h2>My First Page</h2>
<p id="test"></p>

<script>
  var p = document.getElementById("test");
  p.innerHTML = "Hello World!";
</script>
```

<br>

---

<br>

# 변수의 Scope

## Scope란?

<br>

- 변수의 유효 범위
  <br>
  <br>

## 전역 변수

<br>
함수 외부에서 선언된 변수. 많이 쓰면 좋지 않습니다. 가급적이면 사용하지 않는 게 좋습니다.
<br><br>

## 지역 변수

<br>
함수 안에서 선언된 변수 외부에서 사용할 수 없다.
<br><br>

## 자동 전역 변수

<br>
함수 안에서 var 없이 선언하면 자동 전역 변수가 된다. 절대로 이렇게 하면 안 됩니다!
<br><Br>

## 매개 변수의 스코프

<br>
함수의 매개 변수는 자동으로 지역 변수 취급
<br><br>

## for 문 안에서 사용된 변수의 스코프

<br>
언어마다 다른데 자바스크립트에서는 그냥 for 문 바깥에서 선언된 것과 동일한 효과입니다.
<br><Br>

## const와 let

<br>
ES6의 새로 등장한 문법으로 var와는 조금 다르게 동작합니다. 일반적으로 연습할 때는 const와 let을 쓰는 걸 권장합니다. let을 블록 범위 스코프를 가지고 있습니다. <br><Br>

> 일단 변수 선언은 무조건 const로 하자. const로 안되는 상황이 발생시에 let을 쓰자.
> <br><br>

---

<br>

# 재귀의 기초

<br>

## 재귀란?

<br>
함수가 함수 안에서 자신을 다시 호출하는 것
<br><br>

```js
var foo = function () {
  foo();
};
```

<br>

# 카운트 다운 재귀로 구현하기

<br>

## 카운트 다운 일반 버전

<br>

```js
var countdown = function (n) {
  for (var i = n; i >= 0; i--) {
    console.log(i);
  }
};

countdown(10);
```

<br>

## 재귀로 구현하기 1

<br>

```js
var countdown2 = function (n) {
  console.log(n);
  countdown2(n - 1);
};
```

<br>
위 코드는 종료 조건이 빠져 있기 때문에 무한 루프처럼 종료가 되지 않습니다! <br><br>

> 재귀 함수는 반드시 종료 조건이 필요합니다!
> <br><Br>

## 재귀 함수에 종료 조건 추가

<br>

```js
var countdown2 = function (n) {
  //termination condition
  console.log(n);
  if (n <= 0) {
    return;
  }

  countdown2(n - 1);
};
```

<br>
재귀에는 반드시 종료조건이 필요하다.
<br><br>

## 왜 재귀를 사용하나?

<br>

- 재귀를 사용하면 쉽게 풀리는 문제들이 많이 존재하기 때문입니다.
- 예를 들어, 알고리즘의 리스트, 트리, 그래프 순회 문제는 재귀로 푸는 게 편합니다.
  <br><br>

## 재귀 vs 일반

<br>

- 일반 함수가 재귀 함수보다 높은 성능을 보인다.
- 모든 재귀 알고리즘은 일반 알고리즘으로 바꿀 수 있다.

그러나, 재귀 없이 구현하면 성능이 좋아지고 재귀를 사용하면 프로그래머의 능력이 좋아집니다.
<br><br>

## 재귀로 구현하기 연습

<br>

- a부터 b까지 정수를 더해서 리턴해 주는 함수
  <br><Br>

```js
var rsum = function (a, b) {
  if (a == b) {
    return a;
  }
  return b + rsum(a, b - 1);
};

var x = rsum(1, 10);
console.log(x);
```

<br>

## 재귀로 팩토리얼 구현하기

<br>

```js
fact(3) = 3 * 2 * 1

  var fact = function(n) {
    //implement
  };
```

<br>

## 점화식

<br>
재귀나 다이나믹 프로그래밍이라는 걸로 문제를 풀 때 유용하게 사용할 수 있는 수학 공식입니다.
<br><br>

## 재귀로 피보나치 수열 구현하기

<br>
피보나치 수열이란 오래 된 수학 문제 중 하나입니다. 무인도 토끼 문제로도 알려져 있습니다.
<br><br>

### 피보나치 수열의 점화식

<br>

> f(0) = 0 f(1) = 1 f(n) = f(n-1) + f(n-2) f(0) = 0, f(1) = 1, f(2) = f(1) + f(0) = 1 + 0 = 1 f(3) = f(2) + f(1) = 1 + 1 = 2 f(4) = f(3) + f(2) 2 + 1 = 3
> <br><br>

## 재귀로 피보나치 수열을 구현하기

<br>

### 첫 번째 방법

<br>

```js
function fibo(n) {
  if (n <= 0) {
    return 0;
  }
  if (n == 1) {
    return 1;
  }
  return fibo(n - 1) + fibo(n - 2);
}
```

<br>

### 두 번째 방법 (옵션)

<br>

```js
var arr = [0, 1];

function fibo_d(n) {
  if (arr[n] == undefined) {
    arr[n] = fibo_d(n - 1) + fibo_d(n - 2);
  }
  return arr[n];
}
```

<br>
이런 방법을 다이나믹 프로그래밍(또는 memoization) 기법이라고 합니다.

Javascript에서 사용되는 변수 선언 방식인 `var`, `let`, `const`의 차이점에 대해 알아보자.

# 재선언, 재할당

> #### 재선언, 재할당이란?
>
> 자바스크립트(Javascript)는 매니지드 언어(managed language)이기 때문에 개발자가 직접 메모리를 제어하지 못한다. 따라서 개발자가 직접 메모리 주소를 통해 값을 저장하고 참조할 필요가 없고 변수를 통해 안전하게 값에 접근이 가능하다. <br><br> 여기서 `var`, `let`, `const` 키워드를 사용하여 변수명을 자바스크립트 엔진에 알리는 것을 선언(declaration) 이라고 한다. 자바스크립트에서의 변수 선언은 `선언 -> 초기화` 단계를 거쳐서 수행된다. <br><br> 할당이란, 변수에 값을 저장하는 것으로 변수에 값을 할당할 때에는 할당 연산자(=)를 사용한다.

```js
var name; //선언
var name = "kyeom"; //할당
var name = "hangkem"; //재선언
name = "hangkemi"; //재할당
```

### var

```js
var name = "kyeom";
console.log(name); // kyeom

var name = "hangkem";
console.log(name); // hangkem

name = "hangkemi";
console.log(name); // hangkemi
```

var의 경우에는 변수의 재선언, 재할당을 했음에도 에러없이 정상적으로 각각 다른 결과값이 출력된다.

### let

```js
let name = "kyeom";
console.log(name); // kyeom

let name = "hangkem";
console.log(name);
// Uncaught SyntaxError: Identifier 'name' has already been declared

name = "hangkem";
console.log(name); // hangkem
```

let은 재선언은 불가능하지만, 변수에 재할당이 가능하다.

### const

```js
const name = "kyeom";
console.log(name); // kyeom

const name = "hangkem";
console.log(name);
// Uncaught SyntaxError: Identifier 'name' has already been declared

name = "hangkem";
console.log(name);
//Uncaught TypeError: Assignment to constant variable.
```

const는 변수 재선언, 변수 재할당 모두 불가능하다. 여기서 `let`과 `const`의 차이점은 `immtuable`, 즉 `let`은 변경이 가능한 값이지만, `const`는 변경이 불가능한 값이라는 점을 알 수 있다.

# Hoisting?🤔

호이스팅(Hoisting)이란, 자바스크립트 코드를 인터프리터가 로드할 때, 변수의 정의가 그 범위에 따라 선언과 할당으로 분리되어 변수의 선언을 항상 컨텍스트 내의 최상위로 끌어올리는 것을 의미한다. 이는 오로지 변수에만 해당되는 것은 아니고 함수도 가능하며, 자바스크립트에서 함수의 호출을 첫 줄에서 하고 마지막 줄에 함수를 정의해도 문제없이 작동되도록 하는 유용한 특성이다. 하지만, 이 `호이스팅` 때문에 `var`에서 치명적인 오류가 발생하는 경우가 있다.

```js
a = "kyeom";
var a;
```

가령, 이러한 코드가 있다고 하면 `var`에서는 선언 단계와 초기화 단계가 한번에 이루어지기 때문에 오류가 발생하지 않게 된다.

```js
a = "kyeom";
let a; // Uncaught ReferenceError: Cannot access 'a' before initialization
```

하지만, `let`으로 선언된 변수를 선언문 이전에 참조하게 되면, `var`로 선언된 변수와는 다르게 ReferenceError(참조 에러)가 발생하게 된다. 이는 `let`으로 선언된 변수가 스코프의 시작에서 변수의 선언까지 TDZ(temporal dead zone)에 빠지기 때문이다. ![](https://images.velog.io/images/hang_kem_0531/post/d2cbe390-976f-47d7-91c0-815b37912864/image.png)

`const`는 더 엄격한데, `let`은 선언을 먼저하고 나중에 변수에 값을 할당하는 것이 가능하지만, `const`는 선언과 동시에 변수에 값을 할당 해야한다.

# 결론

ES6 이후로는 실제 현업에서 `var`로 변수를 선언하는 것은 거의 사용되지 않고 있다. 그렇다면 남은 것은 `let`과 `const`인데, 앞서 말한 것 처럼 둘 사이의 차이점은 `immutable`이라고 할 수 있다. 그렇기 때문에, 변수 선언에는 대부분 `const`를 사용하고, 재할당이 필요한 경우에만 `let` 을 사용해 변수를 선언하는 것이 좋다.

그리고 객체를 재할당하는 경우는 생각보다 흔하지 않다. `const` 를 사용하면 의도치 않은 재할당을 방지해 주기 때문에 보다 안전하다.

---

### 참조문서

https://gist.github.com/LeoHeo/7c2a2a6dbcf80becaaa1e61e90091e5d
https://velog.io/@bathingape/JavaScript-var-let-const-%EC%B0%A8%EC%9D%B4%EC%A0%90
https://developer.mozilla.org/ko/docs/Glossary/Hoisting
https://ui.toast.com/weekly-pick/ko_20191014

# return이란?

우리가 자바스크립트를 사용하여 함수를 작성할 때, `return`이라는 예약어를 자주 사용하고는 한다. 이렇게 자주 사용되는 예약어임에도 불구하고, `return`이라는 예약어가 무엇이고 어떤 역할을 하는지 잘 모르는체로 사용하는 경우가 많다. `return`의 역할이 무엇이고 어느 때에 사용하는지 알아보자.

### <center><q>return이 하는 일</center>

return이 하는 역할 중에 가장 중요한 일은 함수를 사용시에 반환값을 얻는 일이다. 여기서 반환값이란, 말 그대로 함수가 완료되었을 때 함수가 반환하는 값을 뜻한다. 즉, 함수에서 `return`을 사용하게 되면, 그 함수의 결과를 함수에서 얻을 수 있게 되는 것이다.

또한, `return`은 현재 진행중인 함수를 중지시킬 수 있는 역할도 한다. 아직 실행해야 할 함수들이 남은 상황에서도 `return`을 사용하면 뒤에 위치한 코드들은 자동적으로 중지되게 된다.

> 1. 함수의 반환값을 얻을 때 사용한다.
> 2. 현재 진행 중인 함수를 중지(탈출)시킬때 사용한다.

그럼, 예제를 통해 어떻게 사용되는지 알아보자.

## 반환값

```js
const foo = () => {
  const x = 100;
};

foo(); //결과값이 나타나지 않음.
```

위와 같은 코드를 실행하게 되면, `foo()`에 대한 결과값은 나타나지 않는다. 왜 그럴까? `return`을 통해, 반환할 값이 선언되지 않았기 때문이다. 만약 x의 값을 얻고 싶다면 다음과 같이 구현하면 된다.

```js
const foo = () => {
  const x = 100;
  return x;
};

foo(); //100
```

## 함수 중지

`return`은 함수를 중지시키는 기능 역시 수행한다고 했다. 예제를 통해 알아보자.

```js
const foo = () => {
   const x = 100;
   if (x == 100) {
      return x;
   }
   x = x + 1;
   (...)
}

foo(); //100
```

위와 같이, `return` 밑에 더 많은 코드들이 있지만, 함수의 반환값은 결국 `return` 값인 100이 나오게 된다. 이 처럼, `return`은 현재 구문을 중지하고 빠져나오는(escape) 방법으로 사용이 가능하다.

> #### 자동 세미콜론 삽입
>
> `return` 명령문은, 자동 세미콜론 삽입(ASI)의 영향을 받는다. return 키워드와 표현식 사이에는 줄바꿈 문자가 올 수 없다.

```js
return;
a + b;
```

이 코드는 ASI에 의해 아래처럼 처리된다.

```js
return;
a + b;
```

그렇기 때문에, 문제를 해결하려면 괄호를 사용해 ASI를 방지해야 한다.

```js
return a + b;
```

# About ES6

# Introduction

ECMASCript(ES)란, Ecma International이 ECMA-262 기술 규격에 따라 정의하고 있는 표준화된 스크립트 프로그래밍 언어를 말한다. 자바스크립트를 표준화하기 위해 만들어졌다. 현재 2021년 11월 기준, 2019년 6월에 출판된 ES2019까지의 ECMASCript가 나와있지만 오늘 알아볼 ECMASCript는 바로 2015년 6월에 출판된 ECMASCript의 5판, **ES6**이다.

## 왜 ES6인가?

ES10 까지 나온 현재, 왜 우리는 ES6에 주목해야 할까? 그것은 바로 ES6가 새로운 언어 기능이 포함된 주요 업데이트였으며, 2009년도에 표준화된 ES5 이후로 언어 기능에 대한 첫 업데이트였기 때문이다. 그렇기 때문에 ES6에서는 ES5 이하 명세에서 문제가 되었던 부분들이 해결되었고, 이는 가독성 및 유지보수성 향상으로 이어졌다. React나 Vue와 같은 유명 라이브러리들도 이에 맞춰 개발 환경을 ES6로 바꾸게 되었다. 그럼 지금부터, 대표적인 ES6 문법들에 대하여 알아보자.

## ES6 문법

### const and let

`const`와 `let`은, 앞서 작성했던 문서인 [var, let, const의 차이점](https://velog.io/@hang_kem_0531/JS-var-let-const%EC%9D%98-%EC%B0%A8%EC%9D%B4%EC%A0%90)에서 알아볼 수 있듯이, 변수 선언을 위한 ES6의 새로운 문법이다. 이 둘은 모두 블럭 범위이며, `var`과 다르게 재선언을 할 수 없다는 차이점이 있다.

다만, `let`은 재할당이 가능하지만, `const`는 재할당이 불가능하다는 차이점 역시 존재한다. ES6에서 `const`와 `let`이 등장한 이후로, `var`을 변수를 선언할 때 거의 사용되지 않게 되었다.

### Arrow functions(화살표 함수)

ES6에서는 복잡하고 조금은 깨끗하지 않게 느껴졌던 전통적인 함수표현 (`function(){}`)에 대한 대안으로 Arrow Function을 도입하였다. 다만 이것인 전통적인 함수표현의 대안이라고 해도 몇가지의 제한점이 있으며 모든 상황에 사용할 수는 없다.

- this나 super에 대한 바인딩이 없고, methods 로 사용될 수 없다.
- new.target 키워드가 없다.
- 일반적으로 스코프를 지정할 때 사용하는 call, apply, bind methods를 이용할 수 없다.
- 생성자(Constructor)로 사용할 수 없다.
- yield를 화살표 함수 내부에서 사용할 수 없다.

> #### this 바인딩
>
> 화살표 함수가 기존의 function을 대체할 수 없는 이유 중 대표적인 예시가 서로 가리키고 있는 this 값이 다르다는 것이다. 다음의 예를 살펴보자.

```js
function BlackDog() {
  this.name = "흰둥이";
  return {
    name: "검둥이",
    bark: function () {
      console.log(this.name + ": 멍멍!");
    },
  };
}
const blackDog = new BlackDog();
blackDog.bark(); //검둥이: 멍멍!
```

```js
function WhiteDog() {
  this.name = "흰둥이";
  return {
    name: "검둥이",
    bark: () => {
      console.log(this.name + ": 멍멍!");
    },
  };
}
const whiteDog = new WhiteDog();
whiteDog.bark(); //흰둥이: 멍멍!
```

이와 같이 function()을 사용했을 때는 검둥이가 나타나고, 화살표 함수를 사용했을 때는 흰둥이가 나타나게 된다. 일반 함수는 자신이 종속된 객체를 this로 가리키며, 화살표 함수는 자신이 종속된 인스턴스를 가리키게 된다.

### 템플릿 리터럴 (Template Literal)

우리는 이전까지 문자열을 연결하기 위해 더하기(+) 연산자를 사용해왔다. 하지만 ES6 부터는 그럴 필요 없이 백틱을 사용하여 문자열을 연결하고 문자열 내에서 변수를 사용할 수 있게 되었다.

```js
const foo = (name, age) => {
  return `안녕하세요, 저는 ${name}이고, 나이는 ${age} 살 입니다.`;
};

console.log(foo("김형겸", 25));
// 안녕하세요, 저는 김형겸이고, 나이는 25살입니다.
```

### 비구조화 (Destructing)

ES6에서는 비구조화를 통해 배열과 객체의 값을 변수에 더욱 쉽게 할당할 수 있다.

```js
//ES5
const kyeom = {
	FirstName: '김',
	SecondName: '형겸',
	age: 25
  	major: '경영정보학과',
};

let FirstName = kyeom.FirstName;
let SecondName = kyeom.SecondName;
let myAge = kyeom.age;
let myMajor = kyeom.major;

console.log(FirstName);
console.log(SecondName);
console.log(age);

//ES6
const kyeom = {
	FirstName: '김',
	SecondName: '형겸',
	age: 25
  	major: '경영정보학과',
};

let { FirstName, SecondName, age, major } = kyeom;
```

배열 역시 객체와 동일한 구문을 사용한다.

```js
const fruit = ["사과", "배", "귤", "수박"];

let [value1, value2, value3] = fruit;
```

### 클래스(Class)

ES6 이전에는 자바스크립트에서 클래스를 선언하려면 다음과 같이 `function` 구문을 이용하거나 프로토타입 표현식을 이용해서 선언했어야만 했다.

```js
function User(id, name, email) {
  this.id = id;
  this.name = name;
  this.email = email;
}

Person.prototype.id = function () {
  return id;
};

Person.prototype.name = function () {
  return "[name: " + this.name + ", email: " + this.email + "]";
};
```

하지만 ES6부터는 클래스를 사용하는 구문이 추가되어 Java의 문법과 흡사한 형태로 더욱 가독성이 좋은 클래스 구문을 사용할 수 있게 되었다.

```js
class User {
    constructor(id, name, email) {
        this.id = id;
        this.name = name;
        this.email = email;
    }

    id() {
        return id;
    }

    name() {
        return name;
    }

    info() {
        return "[name: " + this.name +
            ", email: " + this.email + "]";
    }
```

### 모듈(Module)

스크립트의 크기가 커지고 복잡해지기 시작하면서, 개발자들은 '모듈(Module)'이라는 각각의 파일로 클래스나 함수를 분리할 필요성을 느꼈다. 모듈은 단지 스크립트 파일 하나에 불과하며, 이를 `export`와 `import`와 같은 특수한 지시자를 통해 다른 모듈을 불러오거나 공유하여 모듈에 있는 함수를 호출하는 등의 기능 공유가 가능해졌다.

- `export` : 변수나 함수 앞에 붙이면 외부 모듈에서 해당 변수나 함수에 접근할 수 있다(모듈 내보내기).
- `import` : 외부 모듈의 기능을 가져올 수 있다(모듈 가져오기).

사용법은 다음과 같다.

```js
// 📁 Hello.js
export function Hello(User) {
  console.log(`Hello, ${User}!`);
}

// 📁 App.js
import { Hello } from "./Hello.js";

console.log(Hello); // 함수
Hello("Kyeom"); // Hello, Kyeom!
```

둘 이상의 모듈을 가져올 경우에는, 중괄호에 해당 모듈을 넣기만 하면 된다.

### 프로미스(Promise)

`Promise` 객체는 비동기 작업의 완료 또는 실패와 그 결과 값을 나타낸다. 예를 들어 API에서 데이터를 가져오거나 실행하는데 시간이 걸리는 함수를 가지고 있을 때 사용할 수 있다. `Promise`는 다음 중 하나의 상태를 가진다.

- 대기(pending): 이행하거나 거부되지 않은 초기 상태.
- 이행(fulfilled): 연산이 성공적으로 완료됨.
- 거부(rejected): 연산이 실패함.

프로미스 구문은 다음과 같이 사용할 수 있다.

```js
const myPromise = (param) => {
  return new Promise((resolve, reject) => {
    if (param) {
      resolve("성공!");
    } else {
      reject("실패!");
    }
  });
};

myPromise(true).then(
  function (result) {
    console.log(result); //'성공!'
  },
  function (err) {
    console.log(err); //'실패!'
  }
);
```

​

## preventDefaults와 stopPropagation의 차이

JS에서 이벤트 전파를 막는 메서드 중에는 `preventDefaults` 말고도 `stopPropagation` 이라는 메서드가 존재한다. 여기서 `preventDefaults` 와 `stopPropagation` 의 차이는 바로 `stopPropagation`은 이벤트 버블링을 중단시킬 수 있다는 것이다.
​

> #### 이벤트 버블링(Event Bubbling)이란?
>
> 이벤트 버블링은 특정 화면 요소에서 이벤트가 발생했을 때 해당 이벤트가 더 상위의 화면 요소들로 전달되어 가는 특성을 의미한다.

```html
<body>
  <div class="one">
    <div class="two">
      <div class="three"></div>
    </div>
  </div>
</body>
```

```js
const divs = document.querySelectorAll("div");
divs.forEach(function (div) {
  div.addEventListener("click", logEvent);
});
function logEvent(event) {
  console.log(event.currentTarget.className);
}
```

이렇게 3개의 div 태그에 클릭시 logEvent를 발생시키는 함수를 등록하고 최하위 div 태그를 누르면 다음과 같이 실행된다.
![](https://images.velog.io/images/hang_kem_0531/post/5775c6b6-c40f-439f-9fe9-cf83006529a1/image.png)
div 태그 한 개만 클릭했을 뿐인데 3개의 이벤트가 발생되는 이유는 브라우저가 이벤트를 감지하는 방식 때문이다. 브라우저는 특정 화면 요소에서 이벤트가 발생했을 때 그 이벤트를 최상위에 있는 화면 요소까지 이벤트를 전파시킨다. 이와 같은 하위에서 상위 요소로의 이벤트 전파 방식을 이벤트 버블링이라고 한다.
![](https://images.velog.io/images/hang_kem_0531/post/1c3e7d62-0eed-4d40-8cf9-2aab7fca4c8e/image.png)
​
이와 같이 `event.preventDefault()`는 단순히 html에서 표준으로 제공하는 태그의 기본 이벤트 발생을 막는 메서드라면, `event.stopPropagation()`은 말 그대로 상위 엘리먼트로의 이벤트 전파, 즉 이벤트 버블링을 막는다는 차이를 확인할 수 있다. 그렇기 때문에 이벤트가 상위 DOM으로 전파되지 않게 하기 위해서는 `event.stopPropagation`을 사용해야 한다.
​

# DOM이란?

프로그래밍을 공부 하다보면 'DOM에 접근하여', 'DOM이 어쩌구 저쩌구..' 라는 문장을 많이 접해봤을 것이다. 나 역시도 책이나 인터넷 강의들도 리액트와 자바스크립트 공부를 하면서 DOM이라는 단어가 나올때마다 DOM의 정확한 뜻을 몰라 많이 헤메었던 기억이 있다. 그렇기 때문에 오늘 DOM에 대해 정확히 알아보고 넘어가기 위해 이 게시글을 작성하고자 한다.

# DOM의 정의

MDN에서 정의한 DOM의 설명을 한번 보자.

> **문서 객체 모델(The Document Object Model, 이하 DOM)** 은 HTML, XML 문서의 프로그래밍 interface 이다. DOM은 문서의 구조화된 표현(structured representation)을 제공하며 프로그래밍 언어가 DOM 구조에 접근할 수 있는 방법을 제공하여 그들이 문서 구조, 스타일, 내용 등을 변경할 수 있게 돕는다.

나는 처음에 이 문장을 보고도 '이게 대체 뭔소리야...' 하면서 이해가 잘 되지 않았었다. 그럼 문서 객체 모델이라는 단어를 한번 분석해보자. 문서 객체란, `<html>`이나 `<body>` 같은 html문서의 태그들을 JavaScript가 이용할 수 있는 객체(object)로 만들면 그것을 문서 객체라고 한다. 모델(Model)은 해당 단어에서는 '인식하는 방식'으로 해석된다. 즉 이 해석만 본다면, DOM이라는 것은 웹 브라우저가 HTML을 인식하는 방식, 혹은 document 객체와 관련된 객체의 집합을 의미한다고 볼 수 있다.

## 웹 페이지가 만들어지는 과정

![](https://images.velog.io/images/hang_kem_0531/post/0bf5fbbe-a5c0-4859-9dc7-e86311c7f632/image.png)
그럼, DOM을 더 자세하게 이해하기 위해 우선 웹 페이지가 만들어지는 과정부터 알아보도록 하자.

웹 페이지는 브라우저가 HTML, CSS, Javascipt를 서버로부터 전달받아 화면에 픽셀화하여 만들어지게 되는데 이때의 과정을 중요 렌더링 경로(Critical Rendering Path), CRP라고 한다. 총 6가지의 단계가 있지만, 간단하게 두 가지로 나누게 되면 브라우저가 읽어들인 문서를 파싱하여 최종적으로 어떤 내용을 페이지에 렌더링 할지 결정하는 단계와, 브라우저가 렌더링을 수행하는 단계로 나눌 수 있다.

이때, 첫번째 단계에서 렌더 트리(Render Tree)가 생성되는데, 이 렌더 트리는 웹 페이지에 표시될 HTML 요소들과 이와 관련된 스타일 요소들로 구성이 되어 있다. 이때 렌더 트리를 생성하기 위해 브라우저가 필요한 2가지 요소가 바로 CSSOM과 DOM 이다. 바로 이때, DOM이 생성된다.

> **CSSOM (Cascading Style Sheet Object Model)** - 요소들과 관련된 스타일 정보의 구조화 표현
> **DOM (Document Object Model)** - HTML 요소들의 구조화 표현

## 트리(Tree) 구조

![](https://images.velog.io/images/hang_kem_0531/post/5601086f-9805-4e2e-901a-d14fd2b93a0a/image.png)
(HTML 문서 내의 DOM 계층의 예)

DOM을 제대로 이해하기 위해서는 트리 구조에 대해서 이해할 필요가 있다. **트리(Tree)는 노드(Node)라고 불리는 개체로 이루어진 자료 구조**이다. 여기서 노드(Node)란, HTML을 예로 들때 HTML 문서의 모든 것을 노드라고 할 수 있다.

| 노드                      | 설명                                                                                                                                         |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| 문서 노드(document node)  | HTML 문서 전체를 나타내는 노드임.                                                                                                            |
| 요소 노드(element node)   | 모든 HTML 요소는 요소 노드이며, 속성 노드를 가질 수 있는 유일한 노드임.                                                                      |
| 속성 노드(attribute node) | 모든 HTML 요소의 속성은 속성 노드이며, 요소 노드에 관한 정보를 가지고 있음. 하지만 해당 요소 노드의 자식 노드(child node)에는 포함되지 않음. |
| 텍스트 노드(text node)    | HTML 문서의 모든 텍스트는 텍스트 노드임.                                                                                                     |
| 주석 노드(comment node)   | HTML 문서의 모든 주석은 주석 노드임.                                                                                                         |

트리와 노드에 관한 설명은 다음과 같다.

**1. 트리는 하나의 루트 노드를 갖는다.
**
**2. 루트 노드는 0개 이상의 자식 노드를 갖고 있다.
**
**3. 그 자식 노드 또한 0개 이상의 자식 노드를 갖고 있고, 이는 반복적으로 정의된다.
**

이와 같이 DOM은 트리(Tree) 구조의 자료 형태를 가지고 있다.

## DOM에 대해 알아두어야 할 것

### 1. DOM != HTML

DOM이 HTML 문서로부터 생성되는 것은 맞지만, DOM이 HTML과 같다고 볼수는 없다. DOM이 원본 HTML 소스와 다를 수 있는 두 가지 케이스가 존재한다.

1. 작성된 HTML이 유효하지 않을 때
   DOM은 유효한 HTML 문서의 인터페이스다. DOM을 생성하는 동안, 브라우저는 유효하지 않은 HTML 코드를 올바르게 교정하게 된다. 예시를 살펴보자.

![](https://images.velog.io/images/hang_kem_0531/post/2a60e49e-0751-4e51-a769-0f05549d12d8/image.png)

![](https://images.velog.io/images/hang_kem_0531/post/9cae8134-d665-445d-8b91-927def066757/image.png)

위와 같이, HTML 규칙의 필수 사항인 `<head>`와 `<body>` 태그가 빠져있지만, DOM 트리에서는 올바르게 교정되어 나타나게 된다.

2. DOM이 자바스크립트에 의해 수정될 경우
   DOM은 HTML 문서를 볼 수 있는 인터페이스 역할을 함과 동시에, 동적으로 변경될 수 있다. 예를 들어, 자바스크립트가 DOM에 새로운 노드를 추가할 수 있다.

![](https://images.velog.io/images/hang_kem_0531/post/fb03de31-1410-4558-8e35-b8a9e66d3656/image.png)
하지만 이 코드는 DOM을 업데이트 할 뿐이지, HTML 문서를 변경하진 않는다.

### 2. DOM은 브라우저에서 보이는 것이 아니다.

앞서 설명한 것처럼, 브라우저 뷰 포트에서 보이는 것은 렌더 트리로, CSSOM과 DOM의 결합체이다. 렌더 트리는 오직 화면에 그려지는 것만으로 구성되어 있기 때문에, 시각적으로 보이지 않는 요소는 제외하게 된다. 예를 들어, `<p>` 태그에 `display:none` 스타일 속성을 추가한다면, DOM에서는 `<p>`요소를 포함하지만, 브라우저 뷰 포트에서는 이것이 나타나지 않는다.

### 3. DOM은 devTools에서 보이는 것이 아니다.

개발 도구의 요소 검사기는 DOM과 가장 가까운 근사치를 제공하지만, DOM에 없는 추가적인 정보를 포함하기도 한다. 가장 좋은 예가 CSS의 가상 요소이다. `::before` 과 `::after` 선택자를 사용하여 생성된 가상 요소는 CSSOM과 렌더 트리의 일부를 구성한다. 하지만, 이는 기술적으로 DOM의 일부는 아니다. DOM은 오직 원본 HTML 문서로부터 빌드 되고, 요소에 적용되는 스타일을 포함하지 않기 때문이다.

![](https://images.velog.io/images/hang_kem_0531/post/17209e2e-45af-4eeb-a12f-d41c30eb576d/image.png)
개발 도구에서는 가상 요소가 DOM의 일부가 아님에도 나타나게 된다. 이러한 이유로 가상 요소는 DOM의 일부가 아니기 때문에 자바스크립트로 수정할 수 없다.

## DOM에 접근하는 방법

자바스크립트로 웹을 다루기 위해서는 DOM 요소에 접근해야 하는데, 다음과 같은 메소드를 이용하여 웹 페이지에서 특정 요소를 찾을 수 있다.

| 메서드                                           | 설명                                                                       |
| ------------------------------------------------ | -------------------------------------------------------------------------- |
| document.getElementById("id명")                  | 해당 id명을 가진 요소 하나를 반환한다.                                     |
| document.querySelector("선택자")                 | 해당 선택자를 만족하는 요소 하나를 반환한다.                               |
| document.getElementsByClassName("class명")[순서] | 해당 class명을 가진 요소들을 배열에 담아 인덱스에 맞는 요소를 반환한다.    |
| document.getElementsByTagName("태그명")[순서]    | 해당 태그명을 가진 요소들을 배열에 담아 인덱스에 맞는 요소를 반환한다.     |
| document.querySelectorAll("선택자명")[순서]      | 해당 선택자를 만족하는 모든 요소들을 배열에 인덱스에 맞는 요소를 반환한다. |

## 요약 정리

요약해서 정리해 보자면, DOM은 넓은 의미로는 웹 브라우저가 HTML을 인식하는 방법, 좁은 의미로는 document 객체의 집합이라고 볼 수 있으며 DOM은 중요 렌더링 경로의 렌더 트리에서 생성되는데, 노드의 집합인 트리 구조로 이루어져 있다고 말할 수 있다. 또한 DOM은 HTML 그 자체가 아니며, 브라우저와 devTools에서 보이는 것이 아니고 특정 메서드를 통해 자바스크립트에서 DOM에 접근할 수 있다.
