---
title: "Duration"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트에서 기간을 나타냅니다."
type: docs
weight: 76
url: /ko/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

프로젝트에서 기간을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Duration()](#Duration--) | 지정된 TimeSpan 값과 TimeUnitType을 사용하여 [Duration](../../com.aspose.tasks/duration) 구조체의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [Clone()](#Clone--) | 이 인스턴스의 깊은 복사본을 생성하고 반환합니다. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | 인스턴스를 다른 인스턴스로 깊게 복사합니다. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | 지정된 기간을 이 기간에 추가합니다. |
| [add(double val)](#add-double-) | 지정된 double 값을 이 기간에 추가합니다. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Duration 객체를 지정된 시간 단위로 다른 기간으로 변환합니다. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getTimeSpan()](#getTimeSpan--) | 이 Duration 객체의 `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 인스턴스를 가져옵니다. |
| [getTimeUnit()](#getTimeUnit--) | 이 객체의 시간 단위 유형을 가져옵니다. |
| [hashCode()](#hashCode--) | 이 객체에 대한 해시 코드 값을 반환합니다. |
| [isElapsed()](#isElapsed--) | 시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다. |
| [isEstimated()](#isEstimated--) | 시간 단위가 추정인지 여부를 나타내는 값을 가져옵니다. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | 지정된 문자열을 [Duration](../../com.aspose.tasks/duration) 구조체의 인스턴스로 변환합니다. |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | 형식 \"PT--H--M--S--\"의 기간 문자열을 구문 분석합니다. |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | 지정된 기간을 이 기간 인스턴스에서 빼습니다. |
| [subtract(double val)](#subtract-double-) | 지정된 double 값을 이 기간 인스턴스에서 빼습니다. |
| [toDouble()](#toDouble--) | Duration 객체를 `double` 값으로 변환합니다. |
| [toString()](#toString--) | 이 인스턴스의 문자열 표현을 반환합니다. |
### Duration() {#Duration--}
```
public Duration()
```


지정된 TimeSpan 값과 TimeUnitType을 사용하여 [Duration](../../com.aspose.tasks/duration) 구조체의 새 인스턴스를 초기화합니다.

### Clone() {#Clone--}
```
public Duration Clone()
```


이 인스턴스의 깊은 복사본을 생성하고 반환합니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


인스턴스를 다른 인스턴스로 깊게 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | 다른 인스턴스. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


지정된 기간을 이 기간에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | 이 인스턴스에 추가할 지정된 [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


지정된 double 값을 이 기간에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| val | double | 이 인스턴스에 추가할 지정된 `double` 값. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Duration 객체를 지정된 시간 단위로 다른 기간으로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| timeUnitType | 바이트 | 지정된 시간 단위 유형. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - 이 인스턴스와 동일한 TimeSpan 및 TimeUnit 값을 가진 다른 Duration 인스턴스가 있는 경우 **True**를 반환하고, 그렇지 않으면 **false**를 반환합니다.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | 비교할 첫 번째 객체. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | 비교할 두 번째 객체. |

**Returns:**
boolean - 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - 지정된 객체가 이 인스턴스와 동일한 TimeSpan 및 TimeUnit 값을 가진 Duration인 경우 **True**, 그렇지 않으면 **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


이 Duration 객체의 `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 인스턴스를 가져옵니다.

값: 이 Duration 객체의 TimeSpan 인스턴스.

**Returns:**
double - 이 Duration 객체의 `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 인스턴스.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


이 객체의 시간 단위 유형을 가져옵니다.

값: 이 Duration 인스턴스의 시간 단위 유형.

**Returns:**
byte - 이 객체의 시간 단위 유형.
### hashCode() {#hashCode--}
```
public int hashCode()
```


이 객체에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 Duration 인스턴스에 대한 해시 코드 값을 반환합니다.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다.

값: 이 Duration 인스턴스가 경과했는지 여부를 결정하는 플래그.

**Returns:**
boolean - 시간 단위가 경과했는지 여부를 나타내는 값.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


시간 단위가 추정인지 여부를 나타내는 값을 가져옵니다.

값: 이 Duration 인스턴스가 추정된 것인지 여부를 결정하는 플래그.

**Returns:**
boolean - 시간 단위가 추정된 것인지 여부를 나타내는 값.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 첫 번째 기간. |
| b | [Duration](../../com.aspose.tasks/duration) | 두 번째 기간. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 첫 번째 기간. |
| b | [Duration](../../com.aspose.tasks/duration) | 두 번째 기간. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


지정된 문자열을 [Duration](../../com.aspose.tasks/duration) 구조체의 인스턴스로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | 기간을 변환할 지정된 [Project](../../com.aspose.tasks/project) 클래스 인스턴스. |
| 값 | java.lang.String | 변환할 지정된 문자열. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


형식 \"PT--H--M--S--\"의 기간 문자열을 구문 분석합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 구문 분석할 지정된 문자열. |

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 구조체의 구문 분석된 인스턴스를 반환합니다.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


지정된 기간을 이 기간 인스턴스에서 빼습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | 이 인스턴스에서 빼기 위한 지정된 [Duration](../../com.aspose.tasks/duration) 인스턴스. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


지정된 double 값을 이 기간 인스턴스에서 빼습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| val | double | 이 인스턴스에서 빼기 위한 지정된 `double` 값. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Duration 객체를 `double` 값으로 변환합니다.

**Returns:**
double - 변환된 값.
### toString() {#toString--}
```
public String toString()
```


이 인스턴스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 인스턴스의 문자열 표현입니다.
