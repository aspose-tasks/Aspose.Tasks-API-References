---
title: "Délégué TaskBarTextConverter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Convertisseur personnalisé des données de tâches en texte de barre"
type: docs
weight: 3380
url: /fr/net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

Convertisseur personnalisé des données de tâche en texte de barre.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | Tâche pour laquelle le texte de la barre de tâche sera rendu. |

### Valeur de retour

Texte à rendre pour une barre correspondant à la tâche spécifiée.

## Exemples

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


