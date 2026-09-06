---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。向此 CalendarCollection 对象添加一个新的基础日历并返回已添加的日历"
type: docs
weight: 20
url: /zh/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

向此 CalendarCollection 对象添加一个新的基础日历并返回添加的日历。

```csharp
public Calendar Add(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 日历名称。 |

### 返回值

已添加 [`Calendar`](../../calendar/) 对象。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当日历名称为 null 时抛出。 |

## 示例

展示如何创建标准日历。

```csharp
var project = new Project();

// 定义一个日历并将其设为标准
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### 另见

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

向此 CalendarCollection 对象添加一个具有指定基础日历的新日历并返回添加的日历。

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 指定的名称。 |
| baseCalendar | 日历 | 指定的基础日历。 |

### 返回值

已添加 [`Calendar`](../../calendar/) 对象。

## 示例

展示如何添加新日历。

```csharp
var project = new Project();

// 可以通过使用集合的 Add 重载向项目的日历集合添加新日历。
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 另见

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


