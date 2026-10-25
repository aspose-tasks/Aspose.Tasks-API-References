---
title: "Tsk.PhysicalPercentComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Значение процента завершения, которое может использоваться как альтернатива для расчёта бюджетных затрат выполненных работ (BCWP)"
type: docs
weight: 900
url: /ru/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Значение процента завершения, которое может использоваться как альтернатива для расчёта бюджетной стоимости выполненных работ (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


