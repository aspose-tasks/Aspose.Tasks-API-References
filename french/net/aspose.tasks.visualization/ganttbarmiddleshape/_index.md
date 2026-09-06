---
title: "Enum GanttBarMiddleShape"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Spécifie la forme centrale d'une barre"
type: docs
weight: 3050
url: /fr/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Spécifie la forme centrale d'une barre.

```csharp
public enum GanttBarMiddleShape
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LineBottom | `7` | Indique la forme de ligne alignée en bas. |
| LineMiddle | `6` | Indique la forme de ligne alignée au centre. |
| LineTop | `5` | Indique la forme de ligne alignée en haut. |
| None | `0` | Indique une forme vide. |
| RectangleBar | `1` | Indique une forme de barre rectangulaire pleine hauteur. |
| RectangleBottom | `4` | Indique une forme de barre rectangulaire à mi-hauteur alignée en bas. |
| RectangleMiddle | `3` | Indique une forme de barre rectangulaire à 1/3 de hauteur alignée au centre. |
| RectangleTop | `2` | Indique la forme de barre rectangle demi‑hauteur alignée en haut. |

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

Montre comment utiliser les styles de barre personnalisés de la vue du diagramme de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Les styles de barre peuvent être spécifiques à une tâche (situés dans GanttChartView.CustomBarStyles)
// ou spécifiques à une catégorie (situés dans GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // À des fins de démonstration, nous modifions le style de la tâche avec l'ID unique = 4
    // Ici, nous définissons le champ (TaskName) pour qu'il s'affiche à gauche de la barre de tâche.
    ganttBarStyle.LeftField = Field.TaskName;
    // Ici, nous définissons un convertisseur personnalisé pour contrôler le texte à afficher à l'intérieur de la barre de tâche.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // À des fins de démonstration, nous modifions les styles applicables aux tâches jalon.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


