---
title: "Asn.VAC"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La differenza tra il costo di base e il costo totale"
type: docs
weight: 590
url: /it/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

La differenza tra il costo di baseline e il costo totale.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Esempi

Mostra come leggere la proprietà Asn.VAC.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


