---
title: "Tsk.DisplayAsSummary"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, должна ли задача отображаться как сводная задача. Чтение поддерживается только для формата XML"
type: docs
weight: 280
url: /ru/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Определяет, должна ли задача отображаться как сводная задача. Чтение поддерживается только для формата XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


