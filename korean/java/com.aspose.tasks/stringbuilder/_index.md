---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API Reference"
description: "변경 가능한 문자열을 나타냅니다."
type: docs
weight: 281
url: /ko/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

문자열을 변경할 수 있는 가변 문자열을 나타냅니다. 확장할 수 없습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | 지정된 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | 지정된 용량으로 시작하고 지정된 최대값까지 확장할 수 있는 StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | 지정된 문자열을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | 지정된 문자열과 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | 지정된 하위 문자열과 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [append(boolean value)](#append-boolean-) | 지정된 부울 값의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(byte value)](#append-byte-) | 지정된 바이트의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(char value)](#append-char-) | 지정된 유니코드 문자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(char value, int repeatCount)](#append-char-int-) | 유니코드 문자의 문자열 표현을 지정된 횟수만큼 복사하여 이 인스턴스에 추가합니다. |
| [append(char[] value)](#append-char---) | 지정된 배열에 있는 유니코드 문자들의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | 지정된 유니코드 문자 서브배열의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(double value)](#append-double-) | 지정된 double 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(float value)](#append-float-) | 지정된 float 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(int value)](#append-int-) | 지정된 int 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(Object value)](#append-java.lang.Object-) | 지정된 객체의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(String value)](#append-java.lang.String-) | 지정된 문자열의 복사본을 이 인스턴스에 추가합니다. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | 지정된 하위 문자열의 복사본을 이 인스턴스에 추가합니다. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | 지정된 BigDecimal 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(long value)](#append-long-) | 지정된 long 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [append(short value)](#append-short-) | 지정된 short 숫자의 문자열 표현을 이 인스턴스에 추가합니다. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | 0개 이상의 형식 항목을 포함하는 복합 형식 문자열을 처리하여 반환된 문자열을 이 인스턴스에 추가합니다. |
| [appendLine()](#appendLine--) | 현재 StringBuilder 객체의 끝에 기본 줄 구분자를 추가합니다. |
| [appendLine(String value)](#appendLine-java.lang.String-) | 지정된 문자열의 복사본과 기본 줄 구분자를 이어서 현재 StringBuilder 객체의 끝에 추가합니다. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | 이 인스턴스의 지정된 구간에서 문자들을 복사하여 대상 Char 배열의 지정된 구간에 넣습니다. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | StringBuilder 이 인스턴스의 용량이 최소한 지정된 값 이상이 되도록 보장합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getCapacity()](#getCapacity--) | 현재 인스턴스가 할당한 메모리에서 포함될 수 있는 최대 문자 수를 가져옵니다. |
| [getLength()](#getLength--) | 현재 StringBuilder 객체의 길이를 가져옵니다. |
| [getMaxCapacity()](#getMaxCapacity--) | 이 인스턴스의 최대 용량을 가져옵니다. |
| [hashCode()](#hashCode--) | 이 StringBuilder에 대한 해시 코드를 반환합니다. |
| [insert(int index, boolean value)](#insert-int-boolean-) | 지정된 문자 위치에 boolean 값의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, byte value)](#insert-int-byte-) | 지정된 문자 위치에 byte 값의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, char value)](#insert-int-char-) | 지정된 문자 위치에 지정된 Unicode 문자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, char[] value)](#insert-int-char---) | 지정된 문자 위치에 지정된 Unicode 문자 배열의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | 지정된 문자 위치에 지정된 Unicode 문자 하위 배열의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, double value)](#insert-int-double-) | 지정된 문자 위치에 double 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, float value)](#insert-int-float-) | 지정된 문자 위치에 float 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, int value)](#insert-int-int-) | 지정된 문자 위치에 int 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | 지정된 문자 위치에 객체의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | 지정된 문자 위치에 문자열을 이 인스턴스에 삽입합니다. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | 지정된 문자 위치에 지정된 문자열의 하나 이상 복사본을 이 인스턴스에 삽입합니다. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | 지정된 문자 위치에 decimal 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, long value)](#insert-int-long-) | 지정된 문자 위치에 long 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [insert(int index, short value)](#insert-int-short-) | 지정된 문자 위치에 short 숫자의 문자열 표현을 이 인스턴스에 삽입합니다. |
| [remove(int startIndex, int length)](#remove-int-int-) | 이 인스턴스에서 지정된 문자 범위를 제거합니다. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | 이 인스턴스에서 지정된 문자의 모든 발생을 다른 지정된 문자로 교체합니다. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | 이 인스턴스의 하위 문자열 내에서 지정된 문자의 모든 발생을 다른 지정된 문자로 교체합니다. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 이 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | 이 인스턴스의 하위 문자열 내에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다. |
| [setCapacity(int value)](#setCapacity-int-) | 현재 인스턴스가 할당한 메모리에 포함될 수 있는 최대 문자 수를 설정합니다. |
| [setLength(int value)](#setLength-int-) | 현재 StringBuilder 객체의 길이를 설정합니다. |
| [toString()](#toString--) | 이 인스턴스의 값을 String으로 변환합니다. |
| [toString(int startIndex, int length)](#toString-int-int-) | 이 인스턴스의 하위 문자열 값을 String으로 변환합니다. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


StringBuilder 클래스의 새 인스턴스를 초기화합니다.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


지정된 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 용량 | int | 이 인스턴스의 권장 시작 크기입니다. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


지정된 용량으로 시작하고 지정된 최대값까지 확장할 수 있는 StringBuilder 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 용량 | int | StringBuilder의 권장 시작 크기입니다. |
| maxCapacity | int | 현재 문자열이 포함할 수 있는 최대 문자 수입니다. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


지정된 문자열을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 인스턴스 값을 초기화하는 데 사용되는 문자열입니다. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


지정된 문자열과 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 인스턴스 값을 초기화하는 데 사용되는 문자열입니다. |
| 용량 | int | StringBuilder의 권장 시작 크기입니다. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


지정된 하위 문자열과 용량을 사용하여 StringBuilder 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 이 인스턴스 값을 초기화하는 데 사용되는 하위 문자열을 포함하는 문자열입니다. |
| 시작인덱스 | int | 값 내에서 하위 문자열이 시작되는 위치입니다. |
| 길이 | int | 하위 문자열의 문자 수입니다. |
| 용량 | int | StringBuilder의 권장 시작 크기입니다. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


지정된 부울 값의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 추가할 부울 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


지정된 바이트의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 바이트 | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


지정된 유니코드 문자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 문자 | 추가할 Unicode 문자입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


유니코드 문자의 문자열 표현을 지정된 횟수만큼 복사하여 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 문자 | 추가할 문자. |
| repeatCount | int | 값을 추가할 횟수. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


지정된 배열에 있는 유니코드 문자들의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | char[] | 추가할 문자 배열. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


지정된 유니코드 문자 서브배열의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | char[] | 문자 배열. |
| 시작인덱스 | int | 값의 시작 위치. |
| charCount | int | 추가할 문자 수. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


지정된 double 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


지정된 float 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | float | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


지정된 int 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


지정된 객체의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Object | 추가할 객체. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


지정된 문자열의 복사본을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가할 문자열. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


지정된 하위 문자열의 복사본을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가할 하위 문자열을 포함하는 문자열. |
| 시작인덱스 | int | 값 내 하위 문자열의 시작 위치. |
| count | int | 값에서 추가할 문자 수. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


지정된 BigDecimal 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


지정된 long 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | long | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


지정된 short 숫자의 문자열 표현을 이 인스턴스에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | short | 추가할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


복합 형식 문자열을 처리하여 반환된 문자열을 이 인스턴스에 추가합니다. 복합 형식 문자열은 0개 이상의 형식 항목을 포함할 수 있습니다. 각 형식 항목은 매개변수 배열의 해당 인수의 문자열 표현으로 대체됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| format | java.lang.String | 복합 형식 문자열. |
| args | java.lang.Object[] | 형식을 지정할 객체 배열. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


현재 StringBuilder 객체의 끝에 기본 줄 구분자를 추가합니다.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


지정된 문자열의 복사본과 기본 줄 구분자를 이어서 현재 StringBuilder 객체의 끝에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가할 문자열. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


이 인스턴스의 지정된 구간에서 문자들을 복사하여 대상 Char 배열의 지정된 구간에 넣습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceIndex | int | 이 인스턴스에서 문자를 복사할 시작 위치입니다. 인덱스는 0부터 시작합니다. |
| 대상 | char[] | 문자를 복사할 배열입니다. |
| 대상인덱스 | int | 문자를 복사할 대상의 시작 위치입니다. 인덱스는 0부터 시작합니다. |
| count | int | 복사할 문자 수입니다. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


StringBuilder 이 인스턴스의 용량이 최소한 지정된 값 이상이 되도록 보장합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 용량 | int | 보장해야 할 최소 용량입니다. |

**Returns:**
int - 이 인스턴스의 새로운 용량입니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체, 또는 null입니다. |

**Returns:**
boolean - 이 인스턴스와 sb가 문자열, Capacity, MaxCapacity 값이 동일하면 true, 그렇지 않으면 false입니다.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


현재 인스턴스가 할당한 메모리에서 포함될 수 있는 최대 문자 수를 가져옵니다.

**Returns:**
int - 현재 인스턴스가 할당한 메모리에 포함될 수 있는 최대 문자 수입니다.
### getLength() {#getLength--}
```
public int getLength()
```


현재 StringBuilder 객체의 길이를 가져옵니다.

**Returns:**
int - 이 인스턴스의 길이입니다.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


이 인스턴스의 최대 용량을 가져옵니다.

**Returns:**
int - 이 인스턴스가 보유할 수 있는 최대 문자 수입니다.
### hashCode() {#hashCode--}
```
public int hashCode()
```


이 StringBuilder에 대한 해시 코드를 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


지정된 문자 위치에 boolean 값의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | boolean | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


지정된 문자 위치에 byte 값의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | 바이트 | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


지정된 문자 위치에 지정된 Unicode 문자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | 문자 | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


지정된 문자 위치에 지정된 Unicode 문자 배열의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | char[] | 삽입할 문자 배열입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


지정된 문자 위치에 지정된 Unicode 문자 하위 배열의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | char[] | 문자 배열. |
| 시작인덱스 | int | 값 내 시작 인덱스입니다. |
| charCount | int | 삽입할 문자 수입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


지정된 문자 위치에 double 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | double | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


지정된 문자 위치에 float 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | float | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


지정된 문자 위치에 int 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | int | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


지정된 문자 위치에 객체의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | java.lang.Object | 삽입할 객체, 또는 null입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


지정된 문자 위치에 문자열을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | java.lang.String | 삽입할 문자열입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


지정된 문자 위치에 지정된 문자열의 하나 이상 복사본을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | java.lang.String | 삽입할 문자열입니다. |
| count | int | 값을 삽입할 횟수입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


지정된 문자 위치에 decimal 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | java.math.BigDecimal | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


지정된 문자 위치에 long 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | long | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


지정된 문자 위치에 short 숫자의 문자열 표현을 이 인스턴스에 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입이 시작되는 이 인스턴스 내 위치입니다. |
| 값 | short | 삽입할 값입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


이 인스턴스에서 지정된 문자 범위를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작인덱스 | int | 제거가 시작되는 이 인스턴스 내 0 기반 위치입니다. |
| 길이 | int | 제거할 문자 수입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


이 인스턴스에서 지정된 문자의 모든 발생을 다른 지정된 문자로 교체합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| oldChar | 문자 | 교체할 문자입니다. |
| newChar | 문자 | oldChar를 교체하는 문자입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


이 인스턴스의 하위 문자열 내에서 지정된 문자의 모든 발생을 다른 지정된 문자로 교체합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| oldValue | 문자 | 교체할 문자입니다. |
| newValue | 문자 | oldChar를 교체하는 문자입니다. |
| 시작인덱스 | int | 이 인스턴스에서 부분 문자열이 시작되는 위치입니다. |
| count | int | 부분 문자열의 길이입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


이 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| oldValue | java.lang.String | 교체할 문자열입니다. |
| newValue | java.lang.String | oldValue를 교체하는 문자열이거나 null입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


이 인스턴스의 하위 문자열 내에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| oldValue | java.lang.String | 교체할 문자열입니다. |
| newValue | java.lang.String | oldValue를 교체하는 문자열이거나 null입니다. |
| 시작인덱스 | int | 이 인스턴스에서 부분 문자열이 시작되는 위치입니다. |
| count | int | 부분 문자열의 길이입니다. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


현재 인스턴스가 할당한 메모리에 포함될 수 있는 최대 문자 수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 현재 인스턴스에 할당된 메모리에 포함될 수 있는 최대 문자 수입니다. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


현재 StringBuilder 객체의 길이를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 이 인스턴스의 길이입니다. |

### toString() {#toString--}
```
public String toString()
```


이 인스턴스의 값을 String으로 변환합니다.

**Returns:**
java.lang.String - 이 인스턴스와 값이 동일한 문자열입니다.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


이 인스턴스의 하위 문자열 값을 String으로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작인덱스 | int | 이 인스턴스에서 부분 문자열의 시작 위치입니다. |
| 길이 | int | 부분 문자열의 길이입니다. |

**Returns:**
java.lang.String - 이 인스턴스의 지정된 부분 문자열과 값이 동일한 문자열입니다.
