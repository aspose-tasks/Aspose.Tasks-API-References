---
title: "Class Gridlines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Gridlines class. Représente les lignes de grille qui apparaissent dans une vue GanttChart."
type: docs
weight: 3120
url: /fr/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Représente les lignes de grille qui apparaissent dans une vue GanttChart.

```csharp
public class Gridlines
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Gridlines](gridlines/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Obtient ou définit le nombre de 0 à 99 qui spécifie l'intervalle entre les lignes de grille. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Obtient ou définit la couleur des lignes de grille secondaires. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Obtient ou définit le motif de ligne pour les quadrillages secondaires. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Obtient ou définit la couleur des quadrillages normaux. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Obtient ou définit le motif de ligne pour les quadrillages normaux. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Obtient ou définit le type de quadrillage. |

## Exemples

Montre comment travailler avec les quadrillages.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// Permet d'ajuster le premier quadrillage de la vue
var gridlines = view.Gridlines[0];
// définit le nombre de 0 à 99 qui spécifie l'intervalle entre les quadrillages.
gridlines.Interval = 2;
// définit la couleur des quadrillages secondaires.
gridlines.IntervalColor = Color.Red;
// définit le motif de ligne pour les quadrillages secondaires
gridlines.IntervalPattern = LinePattern.Solid;
// définit la couleur des quadrillages normaux
gridlines.NormalColor = Color.Blue;
// définit le motif de ligne pour les quadrillages normaux
gridlines.NormalPattern = LinePattern.CloseDot;
// définit le type de quadrillage
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


