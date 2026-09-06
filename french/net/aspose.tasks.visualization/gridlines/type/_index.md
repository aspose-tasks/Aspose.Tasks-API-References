---
title: "Gridlines.Type"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Gridlines. Obtient ou définit le type de ligne de grille"
type: docs
weight: 70
url: /fr/net/aspose.tasks.visualization/gridlines/type/
---
## Gridlines.Type property

Obtient ou définit le type de quadrillage.

```csharp
public GridlineType Type { get; set; }
```

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

* enum [GridlineType](../../gridlinetype/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


