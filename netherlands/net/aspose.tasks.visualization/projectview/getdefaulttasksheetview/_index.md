---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-methode. Bevat id-indicatoren naam duur start eind voorgangers en resource-namen taakkolommen"
type: docs
weight: 60
url: /nl/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Bevat id, indicatoren, naam, duur, start, eind, voorgangers en resource-namen taakkolommen.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Retourwaarde

een weergave die een lijst bevat van [`GanttChartColumn`](../../ganttchartcolumn/).

## Voorbeelden

Toont hoe een project op te slaan met taakbladweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Zie ook

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


