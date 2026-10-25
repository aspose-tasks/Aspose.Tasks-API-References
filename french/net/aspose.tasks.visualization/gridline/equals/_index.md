---
title: "Gridline.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Gridline. Retourne un indicateur indiquant si cette instance est égale à l'objet spécifié"
type: docs
weight: 50
url: /fr/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | l'objet spécifié à comparer à cette instance. |

### Valeur de retour

un indicateur indiquant si cette instance est égale à l'objet spécifié.

## Exemples

Montre comment vérifier l'égalité de lignes de grille.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// l'égalité des lignes de grille est vérifiée par rapport au type de ligne de grille.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// modifier le type
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Voir aussi

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


