---
title: "Asn.Confirmed"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir kaynağın tüm atamalarını kabul edip etmediğini belirler"
type: docs
weight: 170
url: /tr/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Bir kaynağın tüm atamalarını kabul edip etmediğini belirler.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Örnekler

Asn.Confirmed özelliğinin nasıl okunup/yazılacağını gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


