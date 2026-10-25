---
title: "Gridline.Pattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Gridline. Obtient ou définit le LinePattern d'une ligne de grille"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

Obtient ou définit le [`LinePattern`](../../linepattern/) d'une ligne de grille.

```csharp
public LinePattern Pattern { get; set; }
```

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

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


