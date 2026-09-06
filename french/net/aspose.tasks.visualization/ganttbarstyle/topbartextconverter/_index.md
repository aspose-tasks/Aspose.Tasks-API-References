---
title: "GanttBarStyle.TopBarTextConverter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttBarStyle. Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre des tâches. Remplace la valeur de la propriété TopField."
type: docs
weight: 260
url: /fr/net/aspose.tasks.visualization/ganttbarstyle/topbartextconverter/
---
## GanttBarStyle.TopBarTextConverter property

Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. Remplace la valeur de la propriété [`TopField`](../topfield/).

```csharp
public TaskBarTextConverter TopBarTextConverter { get; set; }
```

## Remarques

N’est pas enregistré au format MPP.

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

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


