---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir göreve atanan kaynağın, görevin durumu açısından güncellenmesi gerekip gerekmediğini belirler"
type: docs
weight: 580
url: /tr/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Bir göreve atanan kaynağın, görevin durumu hakkında güncellenmesi gerekip gerekmediğini belirler.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Örnekler

Asn.UpdateNeeded özelliğinin nasıl okunup/yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


