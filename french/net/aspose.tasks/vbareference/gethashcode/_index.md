---
title: "VbaReference.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaReference. Retourne une valeur de code de hachage pour ce VbaReference"
type: docs
weight: 50
url: /fr/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Retourne une valeur de code de hachage pour ce [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

Renvoie une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une référence VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Le code de hachage d'une référence est le code de hachage du GUID interne de la référence
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Voir aussi

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


