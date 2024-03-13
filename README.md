# Python

## **Python Syntax**

들여쓰기는 코드 줄 시작 부분의 공백을 나타냅니다.

다른 프로그래밍 언어에서 코드의 들여쓰기는 가독성만을 위한 것이지만 Python의 들여쓰기는 매우 중요합니다.

Python은 들여쓰기를 사용하여 코드 블록을 나타냅니다.

들여쓰기를 건너뛰면 Python에서 오류가 발생합니다.

공백의 수는 프로그래머에게 달려 있으며, 가장 일반적으로 사용되는 것은 4개이지만 적어도 하나는 있어야 합니다.

동일한 코드 블록에서 동일한 수의 공백을 사용해야 합니다. 그렇지 않으면 Python에서 오류가 발생합니다.

```python
pythonCopy code
if 5 > 2:
    print("Five is greater than two!")
```

## **Python Comments**

주석은 Python 코드를 설명하는 데 사용된다.

주석을 사용하면 코드를 더 읽기 쉽게 만들 수 있다.

코드를 테스트할 때 실행을 방지하기 위해 주석을 사용한다.

주석은 a로 시작하며 `#`Python은 이를 무시합니다.

```python
#This is a comment
print("Hello, World!")
```

주석은 줄 끝에 배치할 수 있으며 Python은 줄의 나머지 부분을 무시합니다.

```python
print("Hello, World!") #This is a comment
```

Python은 변수에 할당되지 않은 문자열 리터럴을 무시하므로 코드에 여러 줄 문자열(삼중 따옴표)을 추가하고 그 안에 주석을 넣을 수 있다.

```python
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```

## 변수

변수는 처음 값을 할당하는 순간 생성됩니다.

```python
x = 5
y = "John"
print(x)
print(y)
```

## 출력 변수

Python `print()`함수는 변수를 출력하는 데 자주 사용됩니다.

```python
x = "Python is awesome"
print(x)
```

`+`연산자를 사용하여 여러 변수를 출력 할 수도 있습니다 

```python
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```

## 글로벌 키워드

함수 내에서 전역 변수를 생성하려면 `global`키워드를 사용할 수 있습니다.

키워드를 사용하면 `global`변수는 전역 범위에 속합니다.

```python
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

## **데이터 유형**

프로그래밍에서 데이터 유형은 중요한 개념입니다.

변수는 다양한 유형의 데이터를 저장할 수 있으며, 유형에 따라 다른 작업을 수행할 수 있습니다

| 텍스트 유형: | str |
| --- | --- |
| 숫자 유형: | int, float, complex |
| 시퀀스 유형: | list, tuple, range |
| 매핑 유형: | dict |
| 세트 유형: | set,frozenset |
| 부울 유형: | bool |
| 바이너리 유형: | bytes, bytearray, memoryview |
| 없음 유형: | NoneType |

## 숫자 유형

Python에는 세 가지 숫자 유형이 있습니다.

- `int`
- `float`
- `complex`

숫자 유형의 변수는 값을 할당하면 생성됩니다.

```python
x = 1    # int
y = 2.8  # float
z = 1j   # complex
```

## 문자열

Python의 문자열은 작은따옴표나 큰따옴표로 묶입니다

다음 함수를 사용하여 문자열 리터럴을 표시할 수 있습니다 `print()`.

```python
print("Hello")
print('Hello')
```

슬라이스 구문을 사용하여 다양한 문자를 반환할 수 있습니다.

```python
b = "Hello, World!"
print(b[2:5])
```

`upper()`는 문자열을 대문자로 반환합니다.

```python
a = "Hello, World!"
print(a.upper())
```

`lower()`는 문자열을 소문자로 반환합니다

```python
a = "Hello, World!"
print(a.lower())
```

## 참 또는 거짓

bool 은 두 값 중 하나를 나타냅니다: `True`또는 `False`.

```python
print(10 > 9)
print(10 == 9)
print(10 < 9)
```

if 문에서 조건을 실행하면 Python은 `True`또는 `False` 를 반환합니다

```python
a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
```

## 연산자

연산자는 변수와 값에 대한 연산을 수행하는 데 사용됩니다.

```python
print(10 + 5)
```

## **산술 연산자**

산술 연산자는 숫자 값과 함께 사용되어 일반적인 수학 연산을 수행합니다.

| + | 덧셈 | x + y |
| --- | --- | --- |
| - | 뻴셈 | x - y |
| * | 곱셈 | x * y |
| / | 나눗셈 | x / y |
| % | 나머지 | x % y |
| ** | 제곱 | x ** y |
| // | 정수 나누기 | x // y |

## 할당 연산자

할당 연산자는 변수에 값을 할당하는 데 사용됩니다

| = | 값 할당 | x = 5 |
| --- | --- | --- |
| += | 기존 값에 값을 더하여 할당 | x = x + 3 |
| -= | 기존 값에 값을 빼서 할당 | x = x - 3 |
| *= | 기존 값에 값을 곱하여 할당 | x = x * 3 |
| /= | 기존 값에 값을 나누어 할당 | x = x / 3 |
| %= | 기존 값에 값을 나눈 나머지 값 할당 | x = x % 3 |
| //= | 기존 값에 값을 나눈 값의 가장 가까운 정수 할당 | x = x // 3 |
| **= | 기존 값에 제곱을 할당 | x = x ** 3 |
| &= | 비트 연산 and | x = x & 3 |
| |= | 비트 연산 or | x = x | 3 |
| ^= | 비트 연산 xor | x = x ^ 3 |
| >>= | a 비트를 b번 오른쪽 이동 후 할당 | x = x >> 3 |
| <<= | a 비트를 b번 왼쪽 이동 후 할당 | x = x << 3 |

## **비교 연산자**

비교 연산자는 두 값을 비교하는 데 사용됩니다.

| == | 같음 | x == y |
| --- | --- | --- |
| != | 같지 않음 | x != y |
| > | 초과 | x > y |
| < | 미만 | x < y |
| >= | 이상 | x >= y |
| <= | 이하 | x <= y |

## **논리 연산자**

논리 연산자는 조건문을 결합하는 데 사용됩니다.

| and | 그리고 | x < 5 and  x < 10 |
| --- | --- | --- |
| or | 또는 | x < 5 or x < 4 |
| not | 부정 | not(x < 5 and x < 10) |

## 목록

목록은 단일 변수에 여러 항목을 저장하는 데 사용됩니다.

목록은 대괄호를 사용하여 생성됩니다.

```python
thislist = ["apple", "banana", "cherry"]
print(thislist)
```

## 튜플

튜플은 단일 변수에 여러 항목을 저장하는 데 사용됩니다.

**튜플은 순서가 지정되고 변경할 수 없다 .**

튜플은 둥근 괄호로 작성됩니다.

```python
thistuple = ("apple", "banana", "cherry")
print(thistuple)
```

## 세트

세트는 단일 변수에 여러 항목을 저장하는 데 사용됩니다.

*세트는 순서가 없고* , *변경할 수 없으며* , *색인이 생성되지 않은* 컬렉션입니다 .

```python
thisset = {"apple", "banana", "cherry"}
print(thisset)
```

## 사전

사전은 키:값 쌍으로 데이터 값을 저장하는 데 사용됩니다.

사전은 순서가 지정되고 변경 가능하며 중복이 허용되지 않는 모음입니다.

사전은 중괄호로 작성되며 키와 값을 갖습니다.

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
```

## **If 문**

- 같음:
    
    a == b
    
- 같지 않음:
    
    a != b
    
- 미만:
    
    a < b
    
- 작거나 같음:
    
    a <= b
    
- 보다 큼:
    
    a > b
    
- 이상:
    
    a >= b
    
    "if 문"은 if 키워드를 사용하여 작성됩니다.
    
    ```python
    a = 33
    b = 200
    if b > a:
      print("b is greater than a")
    ```
    
    ## elif
    
    elif 키워드 는 "이전 조건이 true가 아니면 이 조건을 시도하십시오"라고 말하는 Python의 방식입니다.
    
    ```python
    a = 33
    b = 33
    if b > a:
      print("b is greater than a")
    elif a == b:
      print("a and b are equal")
    ```
    
    ## else
    
    else 키워드 는 이전 조건에서 포착되지 않은 모든 항목을 포착합니다.
    
    ```python
    a = 200
    b = 33
    if b > a:
      print("b is greater than a")
    elif a == b:
      print("a and b are equal")
    else:
      print("a is greater than b")
    ```
    
    ## While 루프
    
    while 루프를 사용하면 조건이 참인 한 일련의 명령문을 실행할 수 있습니다.
    
    ```python
    i = 1
    while i < 6:
      print(i)
      i += 1
    ```
    
    break 문을 사용하면 while 조건이 true인 경우에도 루프를 중지할 수 있습니다.
    
    i가 3일 때 루프를 종료합니다.
    
    ```python
    i = 1
    while i < 6:
      print(i)
      if i == 3:
        break
      i += 1
    ```
    
    continue 문을 사용하면 현재 반복을 중지하고 다음을 계속할 수 있습니다.
    
    i가 3이면 다음 반복을 계속합니다.
    
    ```python
    i = 0
    while i < 6:
      i += 1
      if i == 3:
        continue
      print(i)
    ```
    
    ## **For 루프**
    
    for 루프 는 시퀀스(즉, 목록, 튜플, 사전, 집합 또는 문자열)를 반복하는 데 사용됩니다.
