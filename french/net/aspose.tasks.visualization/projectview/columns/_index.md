---
title: "ProjectView.Columns"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectView. Obtient les colonnes de la vue du projet"
type: docs
weight: 70
url: /fr/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

Obtient les colonnes de la vue du projet.

```csharp
public List<ViewColumn> Columns { get; }
```

## Exemples

Montre comment enregistrer un projet avec une vue contenant un ensemble personnalisé de colonnes.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// itérer sur les colonnes de la vue
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Voir aussi

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


