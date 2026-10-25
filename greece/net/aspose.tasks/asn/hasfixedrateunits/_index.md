---
title: "Asn.HasFixedRateUnits"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Καθορίζει αν οι Μονάδες έχουν Σταθερό Ρυθμό"
type: docs
weight: 270
url: /el/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Καθορίζει εάν οι Μονάδες έχουν Σταθερό Ρυθμό.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.HasFixedRateUnits.

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

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


