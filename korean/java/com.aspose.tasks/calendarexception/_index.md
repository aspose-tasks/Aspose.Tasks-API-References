---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API Reference"
description: "달력의 예외적인 시간 기간을 나타냅니다."
type: docs
weight: 43
url: /ko/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

달력의 예외적인 시간 기간을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CalendarException()](#CalendarException--) | [CalendarException](../../com.aspose.tasks/calendarexception) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | 지정된 java.util.Date 구조체 인스턴스가 예외일 경우 true를 반환합니다. |
| [delete()](#delete--) | 부모 캘린더 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다. |
| [getDayWorking()](#getDayWorking--) | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 가져옵니다. |
| [getDaysOfWeek()](#getDaysOfWeek--) | 이 객체에 대한 DayTypeCollection을 가져옵니다. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 가져옵니다. |
| [getExceptionDates()](#getExceptionDates--) | 캘린더 예외가 적용되는 날짜를 반환합니다. |
| [getFromDate()](#getFromDate--) | 예외 시간의 시작을 가져옵니다. |
| [getMonth()](#getMonth--) | 예외 반복이 예약된 월을 가져옵니다. |
| [getMonthDay()](#getMonthDay--) | 예외 반복이 예약된 월의 일을 가져옵니다. |
| [getMonthItem()](#getMonthItem--) | 예외 반복이 예약된 월 항목을 가져옵니다. |
| [getMonthPosition()](#getMonthPosition--) | 월 내에서 월 항목의 위치를 가져옵니다. |
| [getName()](#getName--) | 예외의 이름을 가져옵니다. |
| [getOccurrences()](#getOccurrences--) | 캘린더 예외가 유효한 발생 횟수를 가져옵니다. |
| [getParentCalendar()](#getParentCalendar--) | 이 객체의 상위 캘린더를 가져옵니다. |
| [getPeriod()](#getPeriod--) | 예외의 반복 기간을 가져옵니다. |
| [getToDate()](#getToDate--) | 예외 시간의 끝을 가져옵니다. |
| [getType()](#getType--) | 예외 유형을 가져옵니다. |
| [getWorkingTime()](#getWorkingTime--) | 캘린더 예외에 대한 작업 시간을 반환합니다. |
| [getWorkingTimes()](#getWorkingTimes--) | WorkingTimeCollection 객체를 가져옵니다. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 설정합니다. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 설정합니다. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 예외 시간의 시작을 설정합니다. |
| [setMonth(int value)](#setMonth-int-) | 예외 반복이 예약된 월을 설정합니다. |
| [setMonthDay(int value)](#setMonthDay-int-) | 예외 반복이 예약된 월의 일을 설정합니다. |
| [setMonthItem(int value)](#setMonthItem-int-) | 예외 반복이 예약된 월 항목을 설정합니다. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | 월 내에서 월 항목의 위치를 설정합니다. |
| [setName(String value)](#setName-java.lang.String-) | 예외의 이름을 설정합니다. |
| [setOccurrences(int value)](#setOccurrences-int-) | 캘린더 예외가 유효한 발생 횟수를 설정합니다. |
| [setPeriod(int value)](#setPeriod-int-) | 예외의 반복 기간을 설정합니다. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 예외 시간의 끝을 설정합니다. |
| [setType(int value)](#setType-int-) | 예외 유형을 설정합니다. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | WorkingTimeCollection 객체를 설정합니다. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


[CalendarException](../../com.aspose.tasks/calendarexception) 클래스의 새 인스턴스를 초기화합니다.

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


지정된 java.util.Date 구조체 인스턴스가 예외일 경우 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | java.util.Date | 지정된 java.util.Date 구조체 인스턴스. |

**Returns:**
boolean - java.util.Date 값이 예외일인 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### delete() {#delete--}
```
public final void delete()
```


부모 캘린더 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


이 객체에 대한 DayTypeCollection을 가져옵니다. 예외가 유효한 요일입니다.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 가져옵니다. False는 반복 범위가 종료 날짜 입력으로 정의됨을 지정합니다.

**Returns:**
boolean - 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


캘린더 예외가 적용되는 날짜를 반환합니다.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - 캘린더 예외가 적용되는 날짜.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


예외 시간의 시작을 가져옵니다.

**Returns:**
java.util.Date - 예외 시간의 시작.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


예외 반복이 예약된 월을 가져옵니다.

**Returns:**
int - 예외 반복이 예정된 월.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


예외 반복이 예약된 월의 일을 가져옵니다.

**Returns:**
int - 예외 반복이 예정된 월의 일.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


예외 반복이 예약된 월 항목을 가져옵니다.

**Returns:**
int - 예외 반복이 예정된 월 항목.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


월 내에서 월 항목의 위치를 가져옵니다.

**Returns:**
int - 월 내에서 월 항목의 위치.
### getName() {#getName--}
```
public final String getName()
```


예외의 이름을 가져옵니다.

**Returns:**
java.lang.String - 예외의 이름.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


캘린더 예외가 유효한 발생 횟수를 가져옵니다.

**Returns:**
int - 캘린더 예외가 유효한 발생 횟수.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


이 객체의 상위 캘린더를 가져옵니다.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


예외의 반복 기간을 가져옵니다.

**Returns:**
int - 예외의 반복 기간.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


예외 시간의 끝을 가져옵니다.

**Returns:**
java.util.Date - 예외 시간의 종료.
### getType() {#getType--}
```
public final int getType()
```


예외 유형을 가져옵니다.

**Returns:**
int - 예외 유형.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


캘린더 예외에 대한 작업 시간을 반환합니다.

**Returns:**
double - 이 캘린더 예외에 대한 작업 시간을 반환합니다.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


WorkingTimeCollection 객체를 가져옵니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다.

--------------------

작업 시간은 최소 하나 이상 있어야 하며, 다섯 개를 초과할 수 없습니다.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 지정된 날짜 또는 요일 유형이 작업 중인지 여부를 나타내는 값. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 설정합니다. False는 반복 범위가 종료 날짜 입력으로 정의됨을 지정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


예외 시간의 시작을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 예외 시간의 시작. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


예외 반복이 예약된 월을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 예외 반복이 예정된 월. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


예외 반복이 예약된 월의 일을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 예외 반복이 예정된 달의 날짜. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


예외 반복이 예약된 월 항목을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 예외 반복이 예정된 월 항목. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


월 내에서 월 항목의 위치를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 월 내에서 월 항목의 위치. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


예외의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 예외의 이름. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


캘린더 예외가 유효한 발생 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 캘린더 예외가 유효한 발생 횟수. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


예외의 반복 기간을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 예외의 반복 기간. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


예외 시간의 끝을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 예외 시간의 종료. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


예외 유형을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 예외 유형. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


WorkingTimeCollection 객체를 설정합니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다.

--------------------

작업 시간은 최소 하나 이상 있어야 하며, 다섯 개를 초과할 수 없습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection 객체. |

