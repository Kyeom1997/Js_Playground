# JavaScript

## 자료형

---

### 자료형이란?

- 어떤 종류의 데이터를 사용하는 것인지 컴퓨터에게 알려주는 것
- 자료형마다 사용 가능한 연산자(Operator)를 따로 가지고 있습니다.
- **자료형이 같아야 연산을 할 수 있습니다.**
  <br>

#### 자료형의 종류

```
Number
String
Boolean
Null
Undefined
```

그리고 하나 더 객체가 있습니다.

```
Object
```

---

#### Number Type

정수와 실수 모두 Number 타입입니다.

```
5;
3.0;
-4.8;
```

<br>

#### 숫자의 연산자

사칙연산, 괄호, 나머지 등이 있습니다.

```
 +, -, /, *, ( ), %
```

<br>

#### 문자열

```
"I am String";
"Hello" + "World";
```

문자열에도 +가 됩니다. (참고로 문자열은 "Immutable" 특징을 가집니다.)

<br>

#### typeof 연산자

데이터 유형을 알려주는 중요한 연산자

```typeof 5;
"number"
typeof -4.8;
"number"
typeof "5";
"string"
```

<br>

#### Boolean

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

논리 연산자에는 &&, ||, ! 등이 있습니다.

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

### 변수란?

**데이터(값)를 담을 수 있는 그릇**입니다.
데이터들은 컴퓨터의 메모리의 어딘가에 저장되는데 그 **값들을 구별짓고 재사용하기 위해서** 변수를 씁니다.
<br>

### 변수 선언하기

변수를 사용하기 위해서는 먼저 선언이 필요합니다.

```
var a;
```

---

### 변수와 대입 연산자

변수에 값을 넣고 싶을 때 `=` 연산자를 사용합니다. `=`은 수학에서의 같다가 아니라 변수에 값을 할당할 때 사용하는 대입 연산자입니다. 같다는 `===` 를 주로 사용합니다.

<br>

### 변수 사용하기

여러가지 방식이 있습니다.

```
var a = 7;
var b = 10;
var c = a + b; //17
```

<br>

### 변수 이름 잘 짓기

변수의 이름은 매우 중요합니다. 일반적으로 소문자로 시작해, 영어, 숫자 `_`를 주로 사용합니다. 카멜 케이스나 스네이크 표기법을 사용합니다.

#### 카멜 케이스

> numPeople

#### 스네이크 케이스

> num_people

---

<br>

## 연산자 및 기타

### 증감 연산자

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

비교 연산자를 수행한 결과값은 Boolean입니다. 비교 연산자에는 `>, <, >=, <=, ===, !=` 등이 있습니다.

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

```
var a = "hello";
a.length;

5
```

`.`연산자는 객체의 속성을 가져올 때 사용하는 연산자입니다.

<br>

### 문자열 간단히 조작하기

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

undefined : 값이 정의되지 않았다.
null : 값이 비어있다.
NaN(Not a Number) : 값이 아니다. === 계산 불가능

### console.log()

개발자 콘솔에 뭔가를 찍어주는 메소드입니다.

```
var a = 1;
var b = "더하기";
var c = 2;
console.log(a + " " + b + " " + c + " = " + a + c);
1 더하기 2 = 12
```

### alert()와 prompt() 사용해 보기

```
var ans = prompt("How are you?");
alert(ans);
```

---

## 조건문

조건에 따라 다른 행동을 취해야 할 때, `if`문과 조건부 연산자 `?`를 사용하면 됩니다.

<br>

### 'if'문

```
if (조건식) {
  //조건식이 참일 경우 실행될 구문
}
```

- `{}`는 생략할 수 있지만 꼭 쓰는게 좋습니다.
- indent(들여쓰기)를 해야 합니다.

### if + else 문

```
if (조건식) {
  //조건식이 참일 경우 실행될 구문
} else {
  //조건식이 거짓일 경우 실행
}
```

### if + else if + else

```
if (조건식1) {
  //조건식이 참일 경우 실행
} else if(조건식2)  {
  //조건식1은 거짓이고 2는 참일 경우
} else {
  //거짓일 경우 실행
}
```

## While 반복문

반복문은 비슷한 일을 반복적으로 처리하기 위한 명령문입니다.

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

### 그래서 for가 등장함

```
for(var i = 0; i <=100; i++) {
  console.log(i);
}
```

### 추가 설명

반복문은 자주 사용하는 형태가 있습니다.

1. n 회 코드 실행
2. 특정 조건을 만족시킬 때까지 코드 실행
3. 배열 안의 원소들 각각에 대해 코드 실행

## break 와 continue

<b>break는 반복문을 중간에 빠져나갈 때 사용합니다.</b> <br>

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

<b> continue는 반복문의 처음으로 돌아갑니다. </b> <br>

- while : 조건식 (i<10)으로 이동
- for : 증감식 (i++)으로 이동

```
for(var i = 0;i < 10; i++) {
    if (i == 5) {
        continue;
    }
    console.log(i);
}
```

## 이중 루프

반복문 안에 반복문이 있는 걸 이중 루프라고 합니다. 종종 사용합니다.
3중, 4중도 가능하지만 잘 사용하지 않습니다.

```
for (var i = 0; i < 2; i++) {
    for (var j = 0; j < 3; j++) {
        console.log(i + ", " +j);
    }
}
```

<br>
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

<b> push(), pop()
- `push(value)` : 배열의 뒤 쪽에 새로운 원소를 삽입합니다.
- `pop()`: 배열의 마지막 원소를 빼서 변수에 넣어 줍니다. 이 때 변수의 길이는 1 감소합니다.
- 스택처럼 동작하는데 사용합니다.

<b> shift(), unshift()
- `push`, `pop`과 반대로 동작합니다.
- `unshift(v)` : 배열의 맨 앞에 새로운 값을 추가합니다.
- `shift()` : 배열의 앞에서 값을 빼서 변수에 넣어 줍니다.

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