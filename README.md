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
