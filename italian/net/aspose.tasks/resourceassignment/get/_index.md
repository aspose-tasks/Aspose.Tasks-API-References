---
title: "ResourceAssignment.Get"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ResourceAssignment metodo. Restituisce il valore a cui la proprietà è mappata in questo contenitore"
type: docs
weight: 700
url: /it/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

Restituisce il valore a cui la proprietà è mappata in questo contenitore.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Asn`](../../asn/) per ottenere la chiave della proprietà. |

### Valore di ritorno

il valore a cui la proprietà è mappata in questo contenitore.

## Esempi

Mostra come creare un'assegnazione e ottenere/impostare le proprietà comuni dell'assegnazione.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


