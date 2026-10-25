---
title: "Tsk.RemainingOvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Оставшиеся запланированные расходы на сверхурочную работу для задачи"
type: docs
weight: 970
url: /ru/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

Оставшиеся запланированные расходы на сверхурочную работу для задачи.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


