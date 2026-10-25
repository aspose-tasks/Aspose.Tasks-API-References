---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le GUID d'un propriétaire d'affectation"
type: docs
weight: 110
url: /fr/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

Le GUID d'un propriétaire d'affectation.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


