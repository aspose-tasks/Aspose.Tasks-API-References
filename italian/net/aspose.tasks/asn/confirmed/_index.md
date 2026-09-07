---
title: "Asn.Confirmed"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se una risorsa ha accettato tutte le sue assegnazioni"
type: docs
weight: 170
url: /it/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Determina se una risorsa ha accettato tutte le sue assegnazioni.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Esempi

Mostra come leggere/scrivere la proprietà Asn.Confirmed.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


