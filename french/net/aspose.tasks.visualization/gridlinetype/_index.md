---
title: "Énumération GridlineType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Visualization.GridlineType. Type de ligne de grille"
type: docs
weight: 3110
url: /fr/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Type de ligne de grille.

```csharp
public enum GridlineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| GanttRow | `0` | Indique le type de ligne de grille d'une ligne de Gantt. |
| TopTierColumn | `1` | Indique le type de ligne de grille d'une colonne de niveau supérieur. |
| BottomTierColumn | `2` | Indique le type de ligne de grille d'une colonne de niveau inférieur. |
| SheetRow | `3` | Indique le type de ligne de grille d'une ligne de feuille. |
| SheetColumn | `4` | Indique le type de ligne de grille d'une colonne de feuille. |
| UsageRow | `5` | Indique le type de ligne de grille d'une ligne d'utilisation. |
| UsageColumn | `6` | Indique le type de ligne de grille d'une colonne d'utilisation. |
| GanttTitleVertical | `7` | Indique le type de ligne de grille verticale du titre Gantt. |
| GanttTitleHorizontal | `8` | Indique le type de ligne de grille horizontale du titre Gantt. |
| BarRows | `9` | Indique le type de ligne de grille des lignes de barre. |
| GanttProjectStart | `10` | Indique le type de ligne de grille du début du projet Gantt. |
| GanttProjectFinish | `11` | Indique le type de ligne de grille de la fin du projet Gantt. |
| GanttStatusDate | `12` | Indique le type de ligne de grille de la date d'état du Gantt. |
| GanttCurrentDate | `13` | Indique le type de ligne de grille de la date actuelle du Gantt. |
| GanttPageBreaks | `14` | Indique le type de ligne de grille des sauts de page du Gantt. |
| MiddleTierColumn | `15` | Indique le type de ligne de grille de la colonne du niveau intermédiaire. |

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


