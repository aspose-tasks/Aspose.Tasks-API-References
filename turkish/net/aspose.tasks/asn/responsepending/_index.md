---
title: "Asn.ResponsePending"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. TeamAssign mesajı için yanıtın alınıp alınmadığını belirler"
type: docs
weight: 480
url: /tr/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

TeamAssign mesajı için yanıtın alınıp alınmadığını belirler.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Örnekler

Asn.ResponsePending özelliğinin nasıl okunup yazılacağını gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


