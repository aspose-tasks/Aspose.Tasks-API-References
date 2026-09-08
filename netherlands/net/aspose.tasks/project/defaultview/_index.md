---
title: "Project.DefaultView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project eigenschap. Haalt een standaardweergave van het project op of stelt deze in"
type: docs
weight: 360
url: /nl/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Haalt de standaardweergave van het project op of stelt deze in.

```csharp
public View DefaultView { get; set; }
```

## Voorbeelden

Toont hoe te werken met de standaardweergave van een project.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Haal standaardweergave op
UsageView view = (TaskUsageView)project.DefaultView;

// Details-kopkolom wordt niet weergegeven
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Geef details-kopkolom weer
view.DisplayDetailsHeaderColumn = true;

// Herhaal details-kop op alle toewijzingsrijen
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Toont hoe te werken met de weergave van Project en een kolom toe te voegen aan de standaardweergave (die wordt weergegeven wanneer een MPP‑bestand wordt geopend in MS Project).

```csharp
// maak een leeg project zonder weergaven
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Wijzig de standaardweergave (het is een Gantt‑diagramweergave).
// Of je kunt de weergave selecteren op naam of via het View‑scherm met behulp van de project.View‑collectie.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// De WriteViewData‑vlag moet worden gebruikt om wijzigingen in de eigenschappen van de weergave te behouden.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### Zie ook

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


