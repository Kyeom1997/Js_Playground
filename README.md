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

```
Number
String
Boolean
Null
Undefined
```

<br>
그리고 하나 더 객체가 있습니다.
<br><br>

```
Object
```

---

#### Number Type

<br>
정수와 실수 모두 Number 타입입니다.

```
5;
3.0;
-4.8;
```

<br>

#### 숫자의 연산자

<br>
사칙연산, 괄호, 나머지 등이 있습니다.

```
 +, -, /, *, ( ), %
```

<br>

#### 문자열

<br>

```
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

```typeof 5;
"number"
typeof -4.8;
"number"
typeof "5";
"string"
```

<br>

#### Boolean

<br>

```
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

```
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

```
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

```
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

```
var a;
a++;
a = 0;
a++;
1
a--;
0
```

<br>

### 비교 연산자

<br>
비교 연산자를 수행한 결과값은 Boolean입니다. 비교 연산자에는 `>, <, >=, <=, ===, !=` 등이 있습니다.
<br><br>

```
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

```
var a = "hello";
a.length;

5
```

<br>
`.`연산자는 객체의 속성을 가져올 때 사용하는 연산자입니다.

<br><br>

### 문자열 간단히 조작하기

<br>

```
var a = "KheLLo"
a[0];
"K"
a[1] = "H"; //안 됨
a.slice(1,4);
"heL"
a.toUpperCase();
"KHELLO"
a.toLowerCase();
"khello"
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

```
var a = 1;
var b = "더하기";
var c = 2;
console.log(a + " " + b + " " + c + " = " + a + c);
1 더하기 2 = 12
```

<br>

### alert()와 prompt() 사용해 보기

<br>

```
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

```
if (조건식) {
  //조건식이 참일 경우 실행될 구문
}
```

- `{}`는 생략할 수 있지만 꼭 쓰는게 좋습니다.
- indent(들여쓰기)를 해야 합니다.
  <br><br>

### if + else 문

<br>

```
if (조건식) {
  //조건식이 참일 경우 실행될 구문
} else {
  //조건식이 거짓일 경우 실행
}
```

<br>

### if + else if + else

<br>

```
if (조건식1) {
  //조건식이 참일 경우 실행
} else if(조건식2)  {
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

```
while(조건) {
  console.log("참일때 실행됨");
}
```

---

```
var n = 1;
while(n <=100) {
  console.log("Hi" + n);
  n++;
}
```

---

<br>

### 그래서 for가 등장함

<br>

```
for(var i = 0; i <=100; i++) {
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

```
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

```
for(var i = 0;i < 10; i++) {
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

```
for (var i = 0; i < 2; i++) {
    for (var j = 0; j < 3; j++) {
        console.log(i + ", " +j);
    }
}
```

<br><br>

---

<br><br>

# Switch case 문법

변수에 저장된 값에 따라 각각 다른 코드를 실행하는 분기문입니다. 상황에 따라 `if`와 `else if`를 반복적으로 써야 하는 상황을 피하게 해줍니다.

## 문법

```
var value;
switch(value) {
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

```
var score = prompt('점수를 입력하세요');
if (score === 10) {
    console.log('A');
} else if (score == 9) {
    console.log('B');
} else {
    console.log('C');
}
```

### switch-case 로 구현

```
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

```
var scores = [50, 60, 70];
console.log(scores);
console.log(scores.length);
```

## 인덱스를 이용해서 배열의 원소 읽기

```
scores[0];
scores[3];
```

## 배열에 값 쓰기

```
scores[0] = 100;
scores[9] = 50;
```

## 배열의 타입 알아보기

```
typeof scores
typeof scores[0]
```

## 배열 만들기 2

```
var a = [];
a[0] = 2;
a[1] = 4;
```

## 배열의 길이 구하기

```
scores.length;
```

## 배열의 마지막 원소 읽어오기

```
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

```
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

```
var foo = function() {
  console.log("I am function");
}
```

## 함수 호출

함수를 사용하는 것을 함수 호출(call)이라고 합니다. <b?>함수 이름 + 괄호</b>가 필요합니다.

```
foo();
```

## 매개변수가 있는 함수 정의하기

```
var foo2 = function(name) {
  console.log("hello" + name);
}
```

## 매개변수가 있는 함수 사용해 보기

```
foo2("honux");
```

# 함수와 리턴 값

## 리턴 값이 있는 함수 정의하기

리턴 값이 있을 경우 함수를 호출해서 변수에 값을 넣을 수 있습니다.

```
var five = function () {
  return 5;
}

var n = five();
console.log(n);
//5
```

## 리턴이 없는 함수를 변수에 할당하면?

```
var foo = function() {
    console.log(5);
}
var n = foo();
console.log(n);
//undefined
```

## 아무 값도 없는 리턴 사용하기

`return`으로 함수를 종료하는데 사용할 수 있다.

```
var test1 = function(text) {
  if (text === "exit") {
    return;
  }
  console.log("보이나요?");
}

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

```
p1.name = "Kim Hyeong Kyeom"
console.log(p1.name) //"Kim Hyeong Kyeom"
```

## 메소드

객체에 속한 함수

```
p1.eat = function(food) {
    console.log(this.name + " ate delicious " + food +"...");
};

p1.eat("Beef");
// "Kim Hyeong Kyeom ate delicious Beef..."
```

## 메소드 대신에 일반 함수를 썼다면?

```
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

```
var p2 = {};
p2.name = "crong";
p2.weight = 80;
p2.say = function(word) {
    console.log(this.name + " says, " + word);
};
// this = p2
```

## 객체 만들기 2

JSON 표기법을 이용해서 객체를 만들 수도 있습니다. 생성자 함수를 이용하는 방법도 있지만 다음에 다루겠습니다.

```
var m1 = {
  "name": "Honux",
  "hp": 100,
  "power": 10,
  "attack": function(target) {
    target.hp -= this.power;
  }
};

var c1 = {
   type: "Coffee",
   energy: 10
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

```
var a = [10, 20, 30, 40, 10, 50]
a.indexOf(10); //0
a.indexOf(65535); //-1
a.lastIndexOf(10); //4
```

### slice()

사용법 : `slice(startIndex, endIndex)` 기존 배열을 잘라서 새로운 배열을 만듭니다. 기존 배열은 변하지 않습니다. starIndex 위치부터 endIndex 직전의 위치까지 자릅니다. endIndex의 원소는 포함되지 않습니다.

```
a = [1, 2, 3, 4, 5];
a.slice(2,4); //[3,4]
a; // [1, 2, 3, 4, 5]
```

### 문자열의 split()

문자열을 문자의 배열로 나누고 싶을 때 사용하는 메소드입니다.

```
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

```
//휴면 클래스를 정의하는 함수 = 생성자
var Human = function(name, hp, power) {
this.name = name;
this.hp = hp;
this.power = power;
this.attack = function(target) {
target.hp -= this.power;
};
this.show = function() {
console.log("%s %d %d %d",
this.name, this.hp, this.mp, this.power);
};
};
```

## 생성자를 이용해서 객체 만들기

생성자를 이용해서 객체를 만들 때는 `new` 키워드를 사용합니다.

```
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

```
var a = 5;
var b = a;
a === b //true
b = 10
a === b //false
```

<br>
위 코드에서 a와 b는 처음에 값은 같지만 사실은 다른 변수입니다.
<br><br>

## 참조 변수의 동작 방식 이해햐기

<br>
참조 변수라는 것은 객체에 대한 별명 같은 것입니다. 같은 사람을 이름으로도 부르고, 별명으로도 부르고, 다양한 호칭으로 부르는 것과 조금 비슷합니다. 우리가 객체를 만들면 객체가 생기고 변수에는 그 객체의 참조를 할당하는 것입니다. 무슨 말인지 잘 모르겠죠? 이상하게 들리겠지만 아래 코드를 먼저 실행해 보세요.
<br><br>

```
var m1 = {name: "honux", age: 25};
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

```
var foo_v = function(v) {
    v = v * 2;
    console.log(v);
}

var a = 10;
foo_v(a); // 20
console.log(a); // 10
```

<br>

### 참조 전달

<br>

```
var foo_r = function(ref) {
    ref.v = ref.v * 2;
    console.log(ref);
}

var p = {name: "Dora", v: 99};
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

```
function Human(name, hp, mp, power) {
  this.name = name; //m1.name = name;
  this.hp = hp;
  this.mp = mp;
  this.power = power;
}

Human.prototype.attack = function(target) {
    target.hp -= this.power;
};
```

<br>

## 배열과 객체

<br>
객체의 속성값이 배열이 될 수 있습니다. 배열 안에 값들이 객체가 될 수 있습니다.
<br><br>

```
var m1 = {'no': 1, 'scores': [100, 99]};
var m2 = {'no': 2, 'scores': [100, 99]};
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
Hyper
