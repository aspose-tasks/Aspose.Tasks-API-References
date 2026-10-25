---
title: "Asn.VAC"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Разница между базовой стоимостью и общей стоимостью"
type: docs
weight: 590
url: /ru/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

Разница между базовой стоимостью и общей стоимостью.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Примеры

Показывает, как читать свойство Asn.VAC.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


