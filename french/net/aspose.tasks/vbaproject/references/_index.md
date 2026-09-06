---
title: "VbaProject.References"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaProject. Obtient une collection de VbaReferenceCollection"
type: docs
weight: 70
url: /fr/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Obtient une collection de [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Exemples

Montre comment lire les informations de référence du projet VBA.

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


