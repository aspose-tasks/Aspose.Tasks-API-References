---
title: "Asn.UpdateNeeded"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se la risorsa assegnata a un'attività deve essere aggiornata rispetto allo stato dell'attività"
type: docs
weight: 580
url: /it/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Determina se la risorsa assegnata a un'attività deve essere aggiornata rispetto allo stato dell'attività.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Esempi

Mostra come leggere/scrivere la proprietà Asn.UpdateNeeded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


