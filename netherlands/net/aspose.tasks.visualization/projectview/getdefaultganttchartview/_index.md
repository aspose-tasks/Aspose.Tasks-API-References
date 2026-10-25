---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-methode. Bevat id-indicatoren naam duur start en eind taakkolommen"
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Bevat id-, indicatoren-, naam-, duur-, start- en eindtaakkolommen.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Retourwaarde

een weergave die een lijst bevat van [`GanttChartColumn`](../../ganttchartcolumn/).

## Voorbeelden

Toont hoe een project op te slaan met Gantt-diagramweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Zie ook

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


