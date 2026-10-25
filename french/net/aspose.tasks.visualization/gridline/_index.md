---
title: "Classe Gridline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.Gridline. La ligne horizontale ou verticale qui apparaît dans la vue du projet"
type: docs
weight: 3100
url: /fr/net/aspose.tasks.visualization/gridline/
---
## Gridline class

La ligne horizontale ou verticale qui apparaît dans la vue du projet.

```csharp
public class Gridline
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Gridline](gridline/)() | Initialise une nouvelle instance de la classe `Gridline`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Obtient ou définit le [`Color`](./color/) d'une ligne de grille. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Obtient ou définit le type de ligne de grille ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Obtient ou définit le [`LinePattern`](../linepattern/) d'une ligne de grille. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Renvoie une valeur de code de hachage pour l'instance de la classe `Gridline`. |

## Exemples

Montre comment travailler avec les lignes de grille lors de l'enregistrement dans des formats visuels.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // définit le type de ligne de grille (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // définit le <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> d'une ligne de grille
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


