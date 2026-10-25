---
title: "Asn.Milestone"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, является ли назначение контрольной точкой"
type: docs
weight: 330
url: /ru/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Определяет, является ли назначение контрольной точкой.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Примеры

Показывает, как читать свойство Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


