---
title: "Rsc.AssignmentOwner"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le nom d’un propriétaire d’affectation"
type: docs
weight: 100
url: /fr/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Le nom d'un propriétaire d'affectation.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


