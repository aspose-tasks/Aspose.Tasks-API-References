---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectView. Inclut les colonnes de tâche id, indicateurs, nom, durée, début et fin"
type: docs
weight: 30
url: /fr/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Inclut les colonnes id, indicateurs, nom, durée, début et fin de tâche.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Valeur de retour

une vue qui contient une liste de [`GanttChartColumn`](../../ganttchartcolumn/).

## Exemples

Montre comment enregistrer un projet avec la vue du diagramme de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Voir aussi

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


