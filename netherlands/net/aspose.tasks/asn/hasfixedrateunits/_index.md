---
title: "Asn.HasFixedRateUnits"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of de eenheden een vaste tarief hebben"
type: docs
weight: 270
url: /nl/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Bepaalt of de eenheden een vaste tarief hebben.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Voorbeelden

Toont hoe de eigenschap Asn.HasFixedRateUnits te lezen/schrijven.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


