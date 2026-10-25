---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API Reference"
description: "두 타임스탬프 사이의 차이를 나타냅니다."
type: docs
weight: 317
url: /ko/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

두 타임스탬프 사이의 차이를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | 지정된 시간, 분 및 초 수로 TimeDelta의 새 인스턴스를 초기화합니다. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | 지정된 일, 시간, 분, 초 및 밀리초 수로 TimeDelta의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | 이 인스턴스와 다른 인스턴스의 합계인 값을 갖는 새 TimeDelta 객체를 반환합니다. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 두 TimeDelta 값을 비교하고 첫 번째 값이 두 번째 값보다 짧은지, 같은지, 긴지를 나타내는 정수를 반환합니다. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | 이 인스턴스를 지정된 TimeDelta 객체와 비교하고 이 인스턴스가 TimeSpan 객체보다 짧은지, 같은지, 긴지를 나타내는 정수를 반환합니다. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | `other` 시간 간격이 이와 같은지 여부를 나타냅니다. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 두 인스턴스가 같은지 확인합니다. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | 지정된 일 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다. |
| [fromHours(double value)](#fromHours-double-) | 지정된 시간 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다. |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | 지정된 밀리초 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다. |
| [fromMinutes(double value)](#fromMinutes-double-) | 지정된 분 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다. |
| [fromSeconds(double value)](#fromSeconds-double-) | 지정된 초 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다. |
| [getDays()](#getDays--) | 이 인스턴스가 나타내는 시간 간격의 일 구성 요소를 반환합니다. |
| [getHours()](#getHours--) | 이 인스턴스가 나타내는 시간 간격의 시간 구성 요소를 반환합니다. |
| [getMilliseconds()](#getMilliseconds--) | 이 인스턴스가 나타내는 시간 간격의 밀리초 구성 요소를 반환합니다. |
| [getMinutes()](#getMinutes--) | 이 인스턴스가 나타내는 시간 간격의 분 구성 요소를 반환합니다. |
| [getSeconds()](#getSeconds--) | 이 인스턴스가 나타내는 시간 간격의 초 구성 요소를 반환합니다. |
| [getTotalDays()](#getTotalDays--) | 현재 인스턴스의 값을 전체 및 소수 일 단위로 반환합니다. |
| [getTotalHours()](#getTotalHours--) | 현재 인스턴스의 값을 전체 및 소수 시간 단위로 반환합니다. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | 현재 인스턴스의 값을 전체 및 소수 밀리초 단위로 반환합니다. |
| [getTotalMinutes()](#getTotalMinutes--) | 현재 인스턴스의 값을 전체 및 소수 분 단위로 반환합니다. |
| [getTotalSeconds()](#getTotalSeconds--) | 현재 인스턴스의 값을 전체 및 소수 초 단위로 반환합니다. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | 이 인스턴스의 값을 부정한 값을 갖는 새로운 `TimeDelta`를 반환합니다. |
| [parse(String s)](#parse-java.lang.String-) | 시간 간격의 문자열 표현을 해당 `TimeDelta` 등가물로 변환합니다. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | 이 인스턴스와 `other` 인스턴스 사이의 차이를 값으로 갖는 새로운 TimeDelta 객체를 반환합니다. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | 시간 간격의 문자열 표현을 해당 TimeDelta 등가물로 변환하고 변환이 성공했는지 여부를 나타내는 값을 반환합니다. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


지정된 시간, 분 및 초 수로 TimeDelta의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시간 | int | 시간 수. |
| 분 | int | 분 수. |
| 초 | int | 초 수. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


지정된 일, 시간, 분, 초 및 밀리초 수로 TimeDelta의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 일 | int | 일 수. |
| 시간 | int | 시간 수. |
| 분 | int | 분 수. |
| 초 | int | 초 수. |
| 밀리초 | int | 밀리초 수. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


이 인스턴스와 다른 인스턴스의 합계인 값을 갖는 새 TimeDelta 객체를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 합산할 인스턴스. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


두 TimeDelta 값을 비교하고 첫 번째 값이 두 번째 값보다 짧은지, 같은지, 긴지를 나타내는 정수를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 비교할 첫 번째 시간 간격. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 비교할 두 번째 시간 간격. |

**Returns:**
int - \-1 if `t1`이 `t2`보다 짧고, `t1`이 `t2`와 같으면 0, `t1`이 `t2`보다 길면 1.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


이 인스턴스를 지정된 TimeDelta 객체와 비교하고 이 인스턴스가 TimeSpan 객체보다 짧은지, 같은지, 긴지를 나타내는 정수를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 비교할 인스턴스. |

**Returns:**
int - \\-1은 이 인스턴스가 `other`보다 짧을 때, 0은 이 인스턴스가 `other`와 같을 때, 1은 이 인스턴스가 `other`보다 길 때를 의미합니다.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


`other` 시간 간격이 이와 같은지 여부를 나타냅니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 비교할 시간 간격. |

**Returns:**
boolean - 구간이 같으면 `true`; 그렇지 않으면 `false`.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


두 인스턴스가 같은지 확인합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 첫 번째 인스턴스. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 두 번째 인스턴스. |

**Returns:**
boolean - 인스턴스가 같으면 `true`; 그렇지 않으면 `false`.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


지정된 일 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 일 수. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


지정된 시간 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 시간 수. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


지정된 밀리초 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 밀리초 수. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


지정된 분 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 분 수. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


지정된 초 수(가장 가까운 밀리초로 반올림)를 나타내는 TimeDelta를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 초 수. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


이 인스턴스가 나타내는 시간 간격의 일 구성 요소를 반환합니다.

**Returns:**
int - 시간 간격의 일 구성 요소. 양수 또는 음수일 수 있습니다.
### getHours() {#getHours--}
```
public int getHours()
```


이 인스턴스가 나타내는 시간 간격의 시간 구성 요소를 반환합니다.

**Returns:**
int - -23부터 23까지 범위의 시간 간격의 시간 구성 요소.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


이 인스턴스가 나타내는 시간 간격의 밀리초 구성 요소를 반환합니다.

**Returns:**
int - -999부터 999까지 범위의 시간 간격의 밀리초 구성 요소.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


이 인스턴스가 나타내는 시간 간격의 분 구성 요소를 반환합니다.

**Returns:**
int - -59부터 59까지 범위의 시간 간격의 분 구성 요소.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


이 인스턴스가 나타내는 시간 간격의 초 구성 요소를 반환합니다.

**Returns:**
int - -59부터 59까지 범위의 시간 간격의 초 구성 요소.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


현재 인스턴스의 값을 전체 및 소수 일 단위로 반환합니다.

**Returns:**
double - 이 인스턴스가 나타내는 전체 일 수.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


현재 인스턴스의 값을 전체 및 소수 시간 단위로 반환합니다.

**Returns:**
double - 이 인스턴스가 나타내는 전체 시간 수.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


현재 인스턴스의 값을 전체 및 소수 밀리초 단위로 반환합니다.

**Returns:**
double - 이 인스턴스가 나타내는 전체 밀리초 수.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


현재 인스턴스의 값을 전체 및 소수 분 단위로 반환합니다.

**Returns:**
double - 이 인스턴스가 나타내는 전체 분 수.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


현재 인스턴스의 값을 전체 및 소수 초 단위로 반환합니다.

**Returns:**
double - 이 인스턴스가 나타내는 전체 초 수.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


이 인스턴스의 값을 부정한 값을 갖는 새로운 `TimeDelta`를 반환합니다.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


시간 간격의 문자열 표현을 해당 `TimeDelta` 등가물로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| s | java.lang.String | 변환할 시간 간격을 지정하는 문자열. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


이 인스턴스와 `other` 인스턴스 사이의 차이를 값으로 갖는 새로운 TimeDelta 객체를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 빼기 위한 인스턴스. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


시간 간격의 문자열 표현을 해당 TimeDelta 등가물로 변환하고 변환이 성공했는지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| s | java.lang.String | 변환할 시간 간격을 지정하는 문자열. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | 이 배열은 최소 하나의 요소를 포함해야 합니다. 이 메서드가 반환될 때, `result[0]`은 `s`에 의해 지정된 시간 간격을 나타내는 객체를 포함하거나, 변환에 실패한 경우 길이가 0인 시간 간격을 포함합니다. |

**Returns:**
boolean - 변환에 성공하면 `true`; 그렇지 않으면 `false`.
