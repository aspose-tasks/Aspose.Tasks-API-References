---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaModuleAttribute. Retourne une valeur de code de hachage pour cet VbaModuleAttribute"
type: docs
weight: 40
url: /fr/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Retourne une valeur de code de hachage pour ce [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

Renvoie une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'un attribut de module VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// imprimer les codes de hachage d'un attribut de module VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Voir aussi

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


