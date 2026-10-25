---
title: "Asn.Confirmed"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, принял ли ресурс все свои назначения"
type: docs
weight: 170
url: /ru/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Определяет, принял ли ресурс все свои назначения.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Примеры

Показывает, как читать/записывать свойство Asn.Confirmed.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


