---
title: "Énumération GanttBarFillPattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Visualization.GanttBarFillPattern. Un motif de remplissage de forme"
type: docs
weight: 3040
url: /fr/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Le motif de remplissage d'une forme.

```csharp
public enum GanttBarFillPattern
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Hollow | `0` | Motif creux. |
| SolidFill | `1` | Motif de remplissage plein. |
| LightFill | `2` | Motif de remplissage clair. |
| MediumFill | `3` | Motif de remplissage moyen. |
| DarkFill | `4` | Motif de remplissage sombre. |
| DiagonalLeft | `5` | Motif diagonal gauche (du coin supérieur gauche au coin inférieur droit). |
| DiagonalRight | `6` | Motif diagonal droit (du coin supérieur droit au coin inférieur gauche). |
| DiagonalCross | `7` | Motif diagonal en croix. |
| LineVertical | `8` | Motif de ligne verticale. |
| LineHorizontal | `9` | Motif de ligne horizontale. |
| LineCross | `10` | Motif de ligne croisée. |
| SolidFillWithDashedBorder | `11` | Motif plein avec bordure pointillée. |

## Exemples

Montre comment définir les styles de barre personnalisés de la vue de projet du diagramme de Gantt.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Ajoutez le style de barre personnalisé à la collection de barres personnalisées de la vue du projet
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


