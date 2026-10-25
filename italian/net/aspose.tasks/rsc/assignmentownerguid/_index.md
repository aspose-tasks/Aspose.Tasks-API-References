---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il GUID del proprietario di un'assegnazione"
type: docs
weight: 110
url: /it/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

Il GUID del proprietario dell'assegnazione.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


