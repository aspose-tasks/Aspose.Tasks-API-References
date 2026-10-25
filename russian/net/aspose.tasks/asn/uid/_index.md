---
title: "Asn.Uid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Уникальный идентификатор назначения"
type: docs
weight: 560
url: /ru/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

Уникальный идентификатор назначения.

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## Примеры

Показывает, как читать/записывать свойство Asn.Uid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


