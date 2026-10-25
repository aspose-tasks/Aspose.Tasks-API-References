---
title: "Klasse ProjectView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.ProjectView class. Projectweergaveklasse"
type: docs
weight: 3300
url: /nl/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Klasse van projectweergave

```csharp
public class ProjectView
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Initialiseert een nieuw exemplaar van de `ProjectView`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Haalt de projectweergavekolommen op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Bevat Uid-, taaknaam-, resource-naam-, werk- en duurtoewijzingskolommen. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Bevat id-, indicatoren-, naam-, duur-, start- en eindtaakkolommen. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Bevat Uid-, resource-naam-, type-, materiaallabel-, initialen-, groep-, max eenheden-, standaardtarief-, overurenttarief-, kosten per gebruik-, opbouw bij-, basisagenda- en code-resourcekolommen. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Bevat Uid, naam, start, eind en werkresourcekolommen. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Bevat id, indicatoren, naam, duur, start, eind, voorgangers en resource-namen taakkolommen. |

## Voorbeelden

Toont hoe een project op te slaan met de toewijzingsweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


