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
