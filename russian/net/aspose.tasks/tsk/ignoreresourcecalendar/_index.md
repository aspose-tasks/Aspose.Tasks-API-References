---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, учитывается ли в планировании задачи календарь ресурсов, назначенных на задачу"
type: docs
weight: 530
url: /ru/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Определяет, учитывается ли при планировании задачи календарь назначенных ей ресурсов.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


