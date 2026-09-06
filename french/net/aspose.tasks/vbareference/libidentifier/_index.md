---
title: "VbaReference.LibIdentifier"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaReference. Obtient l'identifiant de la bibliothèque"
type: docs
weight: 20
url: /fr/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Obtient l'identifiant de la bibliothèque.

```csharp
public string LibIdentifier { get; }
```

## Exemples

Montre comment lire les références VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Voir aussi

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


