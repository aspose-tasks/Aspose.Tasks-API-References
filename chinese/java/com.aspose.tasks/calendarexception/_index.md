---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示日历中的例外时间段。"
type: docs
weight: 43
url: /zh/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

表示日历中的例外时间段。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CalendarException()](#CalendarException--) | 初始化 [CalendarException](../../com.aspose.tasks/calendarexception) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | 如果指定的 java.util.Date 结构实例是例外日，则返回 true。 |
| [delete()](#delete--) | 从父日历 CalendarExceptionCollection 对象中删除 Exception 实例。 |
| [getDayWorking()](#getDayWorking--) | 获取指示指定日期或天类型是否为工作日的值。 |
| [getDaysOfWeek()](#getDaysOfWeek--) | 获取此对象的 DayTypeCollection。 |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | 获取一个值，指示是否通过输入出现次数来定义重复范围。 |
| [getExceptionDates()](#getExceptionDates--) | 返回日历异常适用的日期。 |
| [getFromDate()](#getFromDate--) | 获取异常时间的开始。 |
| [getMonth()](#getMonth--) | 获取安排异常重复的月份。 |
| [getMonthDay()](#getMonthDay--) | 获取安排异常重复的月份中的日期。 |
| [getMonthItem()](#getMonthItem--) | 获取安排异常重复的月份项。 |
| [getMonthPosition()](#getMonthPosition--) | 获取月份项在月份中的位置。 |
| [getName()](#getName--) | 获取异常的名称。 |
| [getOccurrences()](#getOccurrences--) | 获取日历异常有效的出现次数。 |
| [getParentCalendar()](#getParentCalendar--) | 获取此对象的父日历。 |
| [getPeriod()](#getPeriod--) | 获取异常的重复周期。 |
| [getToDate()](#getToDate--) | 获取异常时间的结束。 |
| [getType()](#getType--) | 获取异常类型。 |
| [getWorkingTime()](#getWorkingTime--) | 返回日历异常的工作时间。 |
| [getWorkingTimes()](#getWorkingTimes--) | 获取 WorkingTimeCollection 对象。 |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 设置一个值，指示指定的日期或日期类型是否为工作日。 |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | 设置一个值，指示是否通过输入出现次数来定义重复范围。 |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 设置异常时间的开始。 |
| [setMonth(int value)](#setMonth-int-) | 设置安排异常重复的月份。 |
| [setMonthDay(int value)](#setMonthDay-int-) | 设置安排异常重复的月份中的日期。 |
| [setMonthItem(int value)](#setMonthItem-int-) | 设置安排异常重复的月份项。 |
| [setMonthPosition(int value)](#setMonthPosition-int-) | 设置月份项在月份中的位置。 |
| [setName(String value)](#setName-java.lang.String-) | 设置异常的名称。 |
| [setOccurrences(int value)](#setOccurrences-int-) | 设置日历异常有效的出现次数。 |
| [setPeriod(int value)](#setPeriod-int-) | 设置异常的重复周期。 |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 设置异常时间的结束。 |
| [setType(int value)](#setType-int-) | 设置异常类型。 |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | 设置 WorkingTimeCollection 对象。 |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


初始化 [CalendarException](../../com.aspose.tasks/calendarexception) 类的新实例。

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


如果指定的 java.util.Date 结构实例是例外日，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | java.util.Date | 指定的 java.util.Date 实例。 |

**Returns:**
boolean - 如果 java.util.Date 值是异常日则返回 true；否则返回 false。
### delete() {#delete--}
```
public final void delete()
```


从父日历 CalendarExceptionCollection 对象中删除 Exception 实例。

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


获取指示指定日期或天类型是否为工作日的值。

**Returns:**
boolean - 指示指定的日期或日期类型是否为工作日的值。
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


获取此对象的 DayTypeCollection。异常有效的星期几。

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


获取一个值，指示是否通过输入出现次数来定义重复范围。False 表示重复范围是通过输入结束日期来定义的。

**Returns:**
boolean - 一个值，指示是否通过输入出现次数来定义重复范围。
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


返回日历异常适用的日期。

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - 日历异常适用的日期。
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


获取异常时间的开始。

**Returns:**
java.util.Date - 异常时间的开始。
### getMonth() {#getMonth--}
```
public final int getMonth()
```


获取安排异常重复的月份。

**Returns:**
int - 安排异常重复的月份。
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


获取安排异常重复的月份中的日期。

**Returns:**
int - 安排异常重复的月份中的日期。
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


获取安排异常重复的月份项。

**Returns:**
int - 安排异常重复的月份项。
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


获取月份项在月份中的位置。

**Returns:**
int - 月份项在月份中的位置。
### getName() {#getName--}
```
public final String getName()
```


获取异常的名称。

**Returns:**
java.lang.String - 异常的名称。
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


获取日历异常有效的出现次数。

**Returns:**
int - 日历异常有效的出现次数。
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


获取此对象的父日历。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


获取异常的重复周期。

**Returns:**
int - 异常的重复周期。
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


获取异常时间的结束。

**Returns:**
java.util.Date - 异常时间的结束。
### getType() {#getType--}
```
public final int getType()
```


获取异常类型。

**Returns:**
int - 异常类型。
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


返回日历异常的工作时间。

**Returns:**
double - 返回此日历异常的工作时间。
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


获取 WorkingTimeCollection 对象。定义工作日工作时间的工作时间集合。

--------------------

至少必须存在一个工作时间，且不能超过五个。

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


设置一个值，指示指定的日期或日期类型是否为工作日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示指定的日期或日期类型是否为工作日的值。 |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


设置一个值，指示是否通过输入出现次数来定义重复范围。False 表示重复范围是通过输入结束日期来定义的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否通过输入出现次数来定义重复范围。 |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


设置异常时间的开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 异常时间的开始。 |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


设置安排异常重复的月份。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 安排异常重复的月份。 |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


设置安排异常重复的月份中的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 计划异常重复的月份中的日期。 |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


设置安排异常重复的月份项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 计划异常重复的月份项。 |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


设置月份项在月份中的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 月份项在月份中的位置。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置异常的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 异常的名称。 |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


设置日历异常有效的出现次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 日历异常有效的出现次数。 |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


设置异常的重复周期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 异常的重复周期。 |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


设置异常时间的结束。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 异常时间的结束。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


设置异常类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 异常类型。 |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


设置 WorkingTimeCollection 对象。定义工作日工作时间的工作时间集合。

--------------------

至少必须存在一个工作时间，且不能超过五个。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection 对象。 |

