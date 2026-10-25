---
title: "Prj.BaselineForEarnedValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La ligne de base spécifique utilisée pour calculer les valeurs de variance"
type: docs
weight: 80
url: /fr/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

La ligne de base spécifique utilisée pour calculer les valeurs de variance.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Exemples

Montre comment lire/écrire la propriété Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


