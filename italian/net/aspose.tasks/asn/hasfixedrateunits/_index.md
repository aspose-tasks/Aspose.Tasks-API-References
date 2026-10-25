---
title: "Asn.HasFixedRateUnits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se le Units hanno un tasso fisso"
type: docs
weight: 270
url: /it/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Determina se le unità hanno un tasso fisso.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Esempi

Mostra come leggere/scrivere la proprietà Asn.HasFixedRateUnits.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


