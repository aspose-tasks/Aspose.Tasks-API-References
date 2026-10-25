---
title: "Asn.HasFixedRateUnits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Birimlerin Sabit Orana sahip olup olmadığını belirler"
type: docs
weight: 270
url: /tr/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Birimlerin sabit oranı olup olmadığını belirler.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Örnekler

Asn.HasFixedRateUnits özelliğinin nasıl okunup/yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


