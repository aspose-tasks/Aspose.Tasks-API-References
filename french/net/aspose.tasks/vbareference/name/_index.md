---
title: "VbaReference.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaReference. Obtient ou définit le nom de la référence VBA"
type: docs
weight: 30
url: /fr/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Obtient ou définit le nom de la référence VBA.

```csharp
public string Name { get; set; }
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


