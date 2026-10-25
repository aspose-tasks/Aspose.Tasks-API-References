---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 내 반복 작업의 세부 정보를 나타냅니다."
type: docs
weight: 244
url: /ko/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

프로젝트 내 반복 작업의 세부 정보를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | 일일 반복 패턴에 대한 반복 횟수를 가져옵니다. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | 일일 반복 패턴에 작업일을 사용할지 여부를 나타내는 값을 가져옵니다. |
| [getDuration()](#getDuration--) | 반복 작업의 한 발생에 대한 기간을 가져옵니다. |
| [getEndDate()](#getEndDate--) | 발생이 종료되는 날짜를 가져옵니다. |
| [getMonthlyDay()](#getMonthlyDay--) | 월별 반복 패턴의 일 수를 가져옵니다. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | 서수일을 사용할 때 월별 반복 패턴의 요일을 가져옵니다. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | 월별 반복 패턴의 서수 번호를 가져옵니다. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | 서수일을 사용할 때 월별 반복 패턴의 반복 횟수를 가져옵니다. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | 월별 반복 패턴의 반복 횟수를 가져옵니다. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | 월별 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 가져옵니다. |
| [getOccurrences()](#getOccurrences--) | 반복 작업의 발생 횟수를 가져옵니다. |
| [getRecurrencePattern()](#getRecurrencePattern--) | 반복 작업의 반복 패턴을 가져옵니다. |
| [getStartDate()](#getStartDate--) | 발생이 시작되는 날짜를 가져옵니다. |
| [getTask()](#getTask--) | 이 인스턴스의 상위 작업을 가져옵니다. [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) 클래스. |
| [getUseEndDate()](#getUseEndDate--) | 반복 작업에 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값을 가져옵니다. |
| [getWeeklyDays()](#getWeeklyDays--) | 주별 반복 패턴에 사용되는 요일 컬렉션을 가져옵니다. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | 주별 반복 패턴의 반복 횟수를 가져옵니다. |
| [getYearlyDate()](#getYearlyDate--) | 연간 반복 패턴의 날짜를 가져옵니다. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | 서수일을 사용할 때 연간 반복 패턴의 요일을 가져옵니다. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | 서수일을 사용할 때 연간 반복 패턴의 월을 가져옵니다. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | 연간 반복 패턴의 서수 번호를 가져옵니다. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | 연간 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 가져옵니다. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | 일별 반복 패턴의 반복 횟수를 설정합니다. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | 일별 반복 패턴에 작업일을 사용할지 여부를 나타내는 값을 설정합니다. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 반복 작업의 한 발생에 대한 기간을 설정합니다. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | 발생이 종료되는 날짜를 설정합니다. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | 월별 반복 패턴의 일 수를 설정합니다. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | 서수일을 사용할 때 월 반복 패턴의 날짜를 설정합니다. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | 월 반복 패턴의 서수 번호를 설정합니다. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | 서수일을 사용할 때 월 반복 패턴의 반복 횟수를 설정합니다. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | 월 반복 패턴의 반복 횟수를 설정합니다. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | 월 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 설정합니다. |
| [setOccurrences(int value)](#setOccurrences-int-) | 반복 작업의 발생 횟수를 설정합니다. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | 반복 작업의 반복 패턴을 설정합니다. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 발생이 시작되는 날짜를 설정합니다. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | 반복 작업에 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값을 설정합니다. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | 주간 반복 패턴에 사용되는 요일 컬렉션을 설정합니다. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | 주간 반복 패턴의 반복 횟수를 설정합니다. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | 연간 반복 패턴의 날짜를 설정합니다. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | 서수일을 사용할 때 연간 반복 패턴의 요일을 설정합니다. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | 서수일을 사용할 때 연간 반복 패턴의 월을 설정합니다. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | 연간 반복 패턴의 서수 번호를 설정합니다. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | 연간 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 설정합니다. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


일일 반복 패턴에 대한 반복 횟수를 가져옵니다.

**Returns:**
int - 일일 반복 패턴의 반복 횟수.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


일일 반복 패턴에 작업일을 사용할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 일일 반복 패턴에 근무일을 사용할지 여부를 나타내는 값.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


반복 작업의 한 발생에 대한 기간을 가져옵니다.

--------------------

`Duration` 인스턴스([getDuration()](../../com.aspose/tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) 클래스.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


발생이 종료되는 날짜를 가져옵니다.

**Returns:**
java.util.Date - 발생이 종료되는 날짜.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


월별 반복 패턴의 일 수를 가져옵니다.

**Returns:**
int - 월 반복 패턴의 일 수.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


서수일을 사용할 때 월별 반복 패턴의 요일을 가져옵니다.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 서수일을 사용할 때 월 반복 패턴의 일.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


월별 반복 패턴의 서수 번호를 가져옵니다.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 월 반복 패턴의 서수 번호.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


서수일을 사용할 때 월별 반복 패턴의 반복 횟수를 가져옵니다.

**Returns:**
int - 순서형 일자를 사용할 때 월별 반복 패턴의 반복 횟수.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


월별 반복 패턴의 반복 횟수를 가져옵니다.

**Returns:**
int - 월별 반복 패턴의 반복 횟수.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


월별 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 월별 반복 패턴에 순서형 일자를 사용할지 여부를 나타내는 값.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


반복 작업의 발생 횟수를 가져옵니다.

**Returns:**
int - 반복 작업의 발생 횟수.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


반복 작업의 반복 패턴을 가져옵니다.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 반복 작업의 반복 패턴.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


발생이 시작되는 날짜를 가져옵니다.

**Returns:**
java.util.Date - 발생이 시작되는 날짜.
### getTask() {#getTask--}
```
public final Task getTask()
```


이 인스턴스의 상위 작업을 가져옵니다. [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) 클래스.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


반복 작업에 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 반복 작업에 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


주별 반복 패턴에 사용되는 요일 컬렉션을 가져옵니다.

--------------------

**Returns:**
int - 주간 반복 패턴에 사용되는 요일 컬렉션.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


주별 반복 패턴의 반복 횟수를 가져옵니다.

**Returns:**
int - 주간 반복 패턴의 반복 횟수.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


연간 반복 패턴의 날짜를 가져옵니다.

**Returns:**
java.util.Date - 연간 반복 패턴의 날짜.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


서수일을 사용할 때 연간 반복 패턴의 요일을 가져옵니다.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 순서형 일자를 사용할 때 연간 반복 패턴의 요일.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


서수일을 사용할 때 연간 반복 패턴의 월을 가져옵니다.

--------------------

[Month](../../com.aspose/tasks/month) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 순서형 일자를 사용할 때 연간 반복 패턴의 월.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


연간 반복 패턴의 서수 번호를 가져옵니다.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 열거형 값 중 하나일 수 있습니다.

**Returns:**
int - 연간 반복 패턴의 순서 번호.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


연간 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 연간 반복 패턴에 순서형 일자를 사용할지 여부를 나타내는 값.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


일별 반복 패턴의 반복 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 일일 반복 패턴의 반복 횟수. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


일별 반복 패턴에 작업일을 사용할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 일일 반복 패턴에 근무일을 사용할지 여부를 나타내는 값. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


반복 작업의 한 발생에 대한 기간을 설정합니다.

--------------------

`Duration` 인스턴스([getDuration()](../../com.aspose/tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 반복 작업 하나의 발생 지속 시간. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


발생이 종료되는 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 발생이 종료되는 날짜. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


월별 반복 패턴의 일 수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 월별 반복 패턴의 일 수. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


서수일을 사용할 때 월 반복 패턴의 날짜를 설정합니다.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 순서형 일자를 사용할 때 월별 반복 패턴의 일. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


월 반복 패턴의 서수 번호를 설정합니다.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 월별 반복 패턴의 순서 번호. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


서수일을 사용할 때 월 반복 패턴의 반복 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 순서형 일자를 사용할 때 월별 반복 패턴의 반복 횟수. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


월 반복 패턴의 반복 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 월별 반복 패턴의 반복 횟수. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


월 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 월별 반복 패턴에 서수일을 사용할지 여부를 나타내는 값입니다. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


반복 작업의 발생 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 반복 작업의 발생 횟수입니다. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


반복 작업의 반복 패턴을 설정합니다.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 반복 작업의 반복 패턴입니다. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


발생이 시작되는 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 발생이 시작되는 날짜입니다. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


반복 작업에 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 반복 작업에 대해 종료 날짜를 사용할지 발생 횟수를 사용할지 여부를 나타내는 값입니다. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


주간 반복 패턴에 사용되는 요일 컬렉션을 설정합니다.

--------------------

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 주간 반복 패턴에 사용되는 요일 컬렉션입니다. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


주간 반복 패턴의 반복 횟수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 주간 반복 패턴의 반복 횟수입니다. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


연간 반복 패턴의 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 연간 반복 패턴의 날짜입니다. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


서수일을 사용할 때 연간 반복 패턴의 요일을 설정합니다.

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 서수일을 사용할 때 연간 반복 패턴의 요일입니다. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


서수일을 사용할 때 연간 반복 패턴의 월을 설정합니다.

--------------------

[Month](../../com.aspose/tasks/month) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 서수일을 사용할 때 연간 반복 패턴의 월입니다. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


연간 반복 패턴의 서수 번호를 설정합니다.

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) 열거형 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 연간 반복 패턴의 서수 번호입니다. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


연간 반복 패턴에 서수일을 사용할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 연간 반복 패턴에 서수일을 사용할지 여부를 나타내는 값입니다. |

