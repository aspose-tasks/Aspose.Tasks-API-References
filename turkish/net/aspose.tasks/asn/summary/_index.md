---
title: "Asn.Summary"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Görevin bir özet görev olup olmadığını belirler"
type: docs
weight: 530
url: /tr/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

Görevin bir özet görev olup olmadığını belirler.

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## Örnekler

Asn.Summary özelliğini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


