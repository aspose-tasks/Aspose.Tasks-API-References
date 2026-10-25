---
title: "View.Table"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "View-eigenschap. Haalt een tabel op of stelt deze in van de enkele weergave"
type: docs
weight: 100
url: /nl/net/aspose.tasks/view/table/
---
## View.Table property

Haalt op of stelt een tabel van de enkele weergave in.

```csharp
public Table Table { get; set; }
```

## Voorbeelden

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

Toont hoe te werken met MS Project weergaven.

```csharp
// maak een leeg project zonder weergaven
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// maak een standaard Gantt-diagramweergave
View view = new GanttChartView();

// stel enkele weergave-eigenschappen in
// stel een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Andere Weergaven vervolgkeuzelijsten in het lint
view.ShowInMenu = true;
// stel een waarde in die aangeeft of Microsoft Project het filter voor een enkele weergave markeert
view.HighlightFilter = true;

// het schrijven van de volgende eigenschappen wordt niet ondersteund
// stelt het filter in dat wordt gebruikt in een enkele weergave
view.Filter = null;
// stelt de groep van de enkele weergave in
view.Group = null;
// stelt de tabel van de enkele weergave in
view.Table = null;

// laten we enkele weergave-instellingen afstemmen
// stel het aantal eerste kolommen in dat op alle pagina's moet worden afgedrukt
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// stel een waarde in die aangeeft of een opgegeven aantal eerste kolommen op alle pagina's moet worden afgedrukt
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// voeg de weergave toe aan ons project
project.Views.Add(view);

// WriteViewData flag moet worden gebruikt om wijzigingen in project.Views te behouden.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// laten we enkele eigenschappen van de nieuw toegevoegde weergave controleren
// druk de unieke identifier van een weergave af
Console.WriteLine("View Uid: " + view.Uid);
// druk het schermtype voor de enkele weergave af
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Zie ook

* class [Table](../../table/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


