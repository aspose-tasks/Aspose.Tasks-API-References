---
title: "Asn.Milestone"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se l'assegnazione è un traguardo"
type: docs
weight: 330
url: /it/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Determina se l'assegnazione è una pietra miliare.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Esempi

Mostra come leggere la proprietà Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


