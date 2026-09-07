---
title: "Asn.FixedMaterial"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se il consumo di una risorsa materiale assegnata avviene in un unico importo fisso"
type: docs
weight: 260
url: /it/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Determina se il consumo di una risorsa materiale assegnata avviene in un unico importo fisso.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Esempi

Mostra come leggere/scrivere la proprietà Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


