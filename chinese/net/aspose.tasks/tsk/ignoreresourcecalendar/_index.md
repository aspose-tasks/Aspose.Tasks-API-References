---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务的调度是否考虑分配给任务的资源日历"
type: docs
weight: 530
url: /zh/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

确定任务的调度是否考虑了分配给该任务的资源日历。

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## 示例

展示如何读取/写入 Tsk.IgnoreResourceCalendar 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


