---
title: "ResourceAssignment.Set"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Отображает указанное свойство на указанное значение в этом контейнере"
type: docs
weight: 750
url: /ru/net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

Сопоставляет указанное свойство с указанным значением в этом контейнере.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| Параметр | Описание |
| --- | --- |
| T | тип сопоставленного значения. |
| key | указанный ключ свойства. [`Asn`](../../asn/) для получения ключа свойства. |
| значение | значение. |

## Примеры

Показывает, как создать назначение и получить/установить общие свойства назначения.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


