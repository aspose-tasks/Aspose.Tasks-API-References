---
title: "Asn.ResponsePending"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, получен ли ответ на сообщение TeamAssign"
type: docs
weight: 480
url: /ru/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

Определяет, получен ли ответ на сообщение TeamAssign.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Примеры

Показывает, как читать/записывать свойство Asn.ResponsePending.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


