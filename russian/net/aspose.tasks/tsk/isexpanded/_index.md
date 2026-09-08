---
title: "Tsk.IsExpanded"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, развернута ли сводная задача в представлении GanttChart"
type: docs
weight: 590
url: /ru/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Определяет, развернута ли сводная задача в представлении GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


