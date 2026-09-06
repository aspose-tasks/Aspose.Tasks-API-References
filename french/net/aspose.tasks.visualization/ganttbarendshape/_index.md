---
title: "Enum GanttBarEndShape"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Représente la forme de fin dans les barres et les points de progression dans les lignes de progression."
type: docs
weight: 3030
url: /fr/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Représente la forme de fin dans les barres et les points de progression dans les lignes de progression.

```csharp
public enum GanttBarEndShape
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| ArrowDown | `14` | Indique la forme de fin de barre Gantt flèche pointant vers le bas. |
| ArrowUp | `8` | Indique la forme de fin de barre Gantt flèche pointant vers le haut. |
| CaretDownTop | `9` | Indique la forme de fin de barre Gantt caret pointant vers le bas sur la moitié supérieure de la barre. |
| CaretUpBottom | `10` | Indique la forme de fin de barre Gantt caret pointant vers le haut sur la moitié inférieure de la barre. |
| Circle | `19` | Indique la forme de fin de barre Gantt cercle. |
| CircleArrowDown | `18` | Indique la forme de fin de barre Gantt flèche entourée pointant vers le bas. |
| CircleArrowUp | `17` | Indique la forme de fin de barre Gantt flèche entourée pointant vers le haut. |
| CircleDiamond | `13` | Indique la forme de fin de barre Gantt losange entouré. |
| CircleTriangleDown | `16` | Indique la forme de fin de barre Gantt triangle entouré pointant vers le bas. |
| CircleTriangleUp | `15` | Indique la forme de fin de barre Gantt triangle entouré pointant vers le haut. |
| Diamond | `3` | Indique la forme de fin de barre Gantt losange. |
| HouseDown | `2` | Indique la forme de fin de barre Gantt maison à l'envers. |
| HouseUp | `1` | Indique la forme de fin de barre Gantt maison. |
| LeftBracket | `21` | Indique la forme de fin de barre Gantt crochet gauche. |
| LeftFade | `23` | Indique la forme de fin de barre Gantt fondu gauche. |
| LineShape | `11` | Indique la forme de fin de barre Gantt ligne. |
| NoBarEndShape | `0` | Indique aucune forme de fin de barre Gantt. |
| RightBracket | `22` | Indique la forme de fin de barre Gantt crochet droit. |
| RightFade | `24` | Indique la forme de fin de barre Gantt fondu droit. |
| Square | `12` | Indique la forme de fin de barre Gantt carré. |
| Star | `20` | Indique la forme de fin de barre Gantt étoile. |
| TriangleDown | `5` | Indique la forme de fin de barre Gantt triangle pointant vers le bas. |
| TriangleLeft | `7` | Indique la forme de fin de barre Gantt en triangle pointant vers la gauche. |
| TriangleRight | `6` | Indique la forme de fin de barre Gantt en triangle pointant vers la droite. |
| TriangleUp | `4` | Indique la forme de fin de barre Gantt triangle entouré pointant vers le haut. |

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


