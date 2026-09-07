---
title: "Rsc.AssignmentOwner"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il nome di un proprietario dell'assegnazione"
type: docs
weight: 100
url: /it/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Il nome del proprietario dell'assegnazione.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


