---
title: "类 CalendarCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalendarCollection 类。表示 Calendar 对象的集合"
type: docs
weight: 240
url: /zh/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

表示一个 [`Calendar`](../calendar/) 对象的集合。

```csharp
public class CalendarCollection : IList<Calendar>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | 获取此 `CalendarCollection` 对象中包含的对象数量。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | 向此 CalendarCollection 对象添加一个新的基础日历并返回添加的日历。 |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | 向此 CalendarCollection 对象添加一个具有指定基础日历的新日历并返回添加的日历。 |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | 返回具有指定名称的日历。 |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | 返回具有指定 UID 的日历。 |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | 从项目 CalendarCollection 中移除日历。 |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | 将 CalendarCollection 对象转换为 [`Calendar`](../calendar/) 对象的列表。 |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


