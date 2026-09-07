---
title: "Asn.RegularWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La quantità di lavoro non straordinario programmato per un'assegnazione"
type: docs
weight: 420
url: /it/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

La quantità di lavoro non straordinario programmato per un'assegnazione.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Asn.RegularWork.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


