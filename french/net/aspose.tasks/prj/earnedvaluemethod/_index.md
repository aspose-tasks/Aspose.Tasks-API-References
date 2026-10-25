---
title: "Prj.EarnedValueMethod"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La méthode par défaut pour calculer la valeur acquise"
type: docs
weight: 310
url: /fr/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

La méthode par défaut de calcul de la valeur acquise.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Exemples

Montre comment lire/écrire la propriété Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


