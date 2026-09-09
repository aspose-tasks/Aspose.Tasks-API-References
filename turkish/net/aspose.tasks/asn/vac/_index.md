---
title: "Asn.VAC"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Temel maliyet ile toplam maliyet arasındaki fark"
type: docs
weight: 590
url: /tr/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

Temel maliyet ile toplam maliyet arasındaki fark.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Örnekler

Asn.VAC özelliğini okuma nasıl gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


