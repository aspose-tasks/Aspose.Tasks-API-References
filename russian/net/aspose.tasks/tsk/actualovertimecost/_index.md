---
title: "Tsk.ActualOvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Затраты, понесённые за сверхурочную работу, уже выполненную над задачами назначенными ресурсами"
type: docs
weight: 50
url: /ru/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Затраты, возникшие в результате уже выполненной сверхурочной работы над задачами назначенными ресурсами.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


