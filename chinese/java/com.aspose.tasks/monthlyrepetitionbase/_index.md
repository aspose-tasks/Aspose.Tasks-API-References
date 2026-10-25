---
title: "MonthlyRepetitionBase"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示月度日期位置的基础模式。"
type: docs
weight: 159
url: /zh/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

表示月度日期位置的基础模式。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | 获取一个月份数，表示两次出现之间的月份间隔。 |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | 设置一个月份数，表示两次出现之间的月份间隔。 |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


获取用于计算重复的计算器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


获取一个月份数，表示两次出现之间的月份间隔。

**Returns:**
int - 一个月份数，表示两次出现之间的月份间隔。
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


获取用于重复模式的验证器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


设置一个月份数，表示两次出现之间的月份间隔。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 一个月份数，表示两次出现之间的月份间隔。 |

