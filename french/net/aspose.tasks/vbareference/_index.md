---
title: "Classe VbaReference"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.VbaReference. Représente une référence du VbaProject"
type: docs
weight: 2870
url: /fr/net/aspose.tasks/vbareference/
---
## VbaReference class

Représente une référence du [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [VbaReference](vbareference/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Obtient l'identifiant de la bibliothèque. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Obtient ou définit le nom de la référence VBA. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à l'objet `VbaReference` spécifié. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Renvoie une valeur indiquant si cette instance est égale à l'objet `VbaReference` spécifié. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Renvoie une valeur de code de hachage pour ce `VbaReference`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


