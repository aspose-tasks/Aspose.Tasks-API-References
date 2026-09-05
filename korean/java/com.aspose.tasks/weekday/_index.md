---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API Reference"
description: "주중 요일을 나타내며, 이는 주의 일반 요일 또는 캘린더의 예외 요일을 정의합니다."
type: docs
weight: 352
url: /ko/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

주중 요일을 나타내며, 이는 주의 일반 요일 또는 캘린더의 예외 요일을 정의합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | 지정된 요일 유형으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | 지정된 요일 유형 및 작업 시간 기간 목록으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | 지정된 요일 유형 및 작업 시간 기간으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay()](#WeekDay--) | [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | .Net의 [DayOfWeek](../../com.aspose.tasks/dayofweek)을 `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))으로 변환합니다. |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | 기본 작업 요일을 생성합니다. |
| [deepClone()](#deepClone--) | 주 요일의 깊은 복사본을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getDayType()](#getDayType--) | 날의 유형을 가져옵니다. |
| [getDayWorking()](#getDayWorking--) | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 가져옵니다. |
| [getFromDate()](#getFromDate--) | 예외 시간의 시작을 가져옵니다. |
| [getToDate()](#getToDate--) | 예외 시간의 끝을 가져옵니다. |
| [getWorkingTime()](#getWorkingTime--) | 주 요일에 대한 작업 시간을 반환합니다. |
| [getWorkingTimes()](#getWorkingTimes--) | 이 WeekDay 인스턴스에 대한 WorkingTimeCollection을 가져옵니다. |
| [hashCode()](#hashCode--) | 해당 [WeekDay](../../com.aspose.tasks/weekday) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 설정합니다. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | 지정된 요일에 대한 기본 시간 기간을 설정합니다. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 예외 시간의 시작을 설정합니다. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 예외 시간의 종료를 설정합니다. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


지정된 요일 유형으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dayType | int | 지정된 요일 유형. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


지정된 요일 유형 및 작업 시간 기간 목록으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dayType | int | 지정된 요일 유형. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | 작업 시간 기간 목록. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


지정된 요일 유형 및 작업 시간 기간으로 [WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dayType | int | 지정된 요일 유형. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | 작업 시간 기간 배열. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


[WeekDay](../../com.aspose.tasks/weekday) 클래스의 새 인스턴스를 초기화합니다.

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


.Net의 [DayOfWeek](../../com.aspose.tasks/dayofweek)을 `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))으로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dw | int | 캐스팅할 요일. |

**Returns:**
int - 캐스팅된 요일 유형.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


기본 작업 요일을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dayType | int | 기본 작업 요일을 생성할 요일 유형. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


주 요일의 깊은 복사본을 반환합니다.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
boolean - 지정된 객체가 이 인스턴스와 동일한 FromDate, ToDate 값 및 WorkingTimes를 가진 WeekDay인 경우 **True**; 그렇지 않으면 **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


날의 유형을 가져옵니다.

**Returns:**
int - 요일 유형.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


예외 시간의 시작을 가져옵니다.

**Returns:**
java.util.Date - 예외 시간의 시작.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


예외 시간의 끝을 가져옵니다.

**Returns:**
java.util.Date - 예외 시간의 종료.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


주 요일에 대한 작업 시간을 반환합니다.

**Returns:**
double - 작업 시간.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


이 WeekDay 인스턴스에 대한 WorkingTimeCollection을 가져옵니다. 요일에 작업된 시간을 정의하는 작업 시간 컬렉션입니다.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


해당 [WeekDay](../../com.aspose.tasks/weekday) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


지정된 요일에 대한 기본 시간 기간을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | 기본 작업 요일을 설정할 요일. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


예외 시간의 시작을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 예외 시간의 시작. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


예외 시간의 종료를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 예외 시간의 끝. |

