---
title: "DateTimeConverter"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于在视图时间轴层级中将日期转换为字符串的转换器。"
type: docs
weight: 70
url: /zh/java/com.aspose.tasks/datetimeconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class DateTimeConverter extends System.MulticastDelegate
```

表示用于在视图时间轴层级中将日期转换为字符串的转换器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DateTimeConverter()](#DateTimeConverter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [invoke(Date date)](#invoke-java.util.Date-) | 表示一种转换方法，用于在视图时间尺度层级中将日期转换为字符串。 |
### DateTimeConverter() {#DateTimeConverter--}
```
public DateTimeConverter()
```


### invoke(Date date) {#invoke-java.util.Date-}
```
public abstract String invoke(Date date)
```


表示一种转换方法，用于在视图时间尺度层级中将日期转换为字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | java.util.Date | 用于转换为字符串的 `java.util.Date` 类实例。 |

**Returns:**
java.lang.String - 指定日期的字符串表示。
