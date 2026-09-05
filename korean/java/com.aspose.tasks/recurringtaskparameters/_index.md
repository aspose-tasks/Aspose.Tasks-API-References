---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트에서 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다."
type: docs
weight: 245
url: /ko/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

프로젝트에서 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | 새 인스턴스를 초기화합니다 [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDuration()](#getDuration--) | 반복 작업의 한 발생에 대한 기간을 가져옵니다. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | 리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값을 가져옵니다. |
| [getRecurrencePattern()](#getRecurrencePattern--) | 반복 작업의 반복 패턴을 가져옵니다. |
| [getTaskName()](#getTaskName--) | 반복 작업의 이름을 가져옵니다. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | 반복 작업에 대한 캘린더를 설정합니다. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 반복 작업의 한 발생에 대한 기간을 설정합니다. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | 리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값을 설정합니다. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | 반복 작업의 반복 패턴을 설정합니다. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | 반복 작업의 이름을 설정합니다. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


새 인스턴스를 초기화합니다 [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) 클래스.

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


반복 작업의 한 발생에 대한 기간을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


반복 작업의 반복 패턴을 가져옵니다.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 열거형의 값 중 하나일 수 있습니다.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


반복 작업의 이름을 가져옵니다.

**Returns:**
java.lang.String - 반복 작업의 이름.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


반복 작업에 대한 캘린더를 설정합니다. 캘린더는 프로젝트 캘린더 컬렉션에서 선택됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 캘린더 컬렉션이 포함된 프로젝트. |
| calendarName | java.lang.String | 캘린더의 이름. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


반복 작업의 한 발생에 대한 기간을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) 클래스의 인스턴스입니다. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 리소스가 사용 가능할 때 작업이 발생하지 않더라도 반복 작업을 예약할지 여부를 나타내는 값. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


반복 작업의 반복 패턴을 설정합니다.

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 열거형의 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | 반복 작업의 반복 패턴. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


반복 작업의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 반복 작업의 이름. |

