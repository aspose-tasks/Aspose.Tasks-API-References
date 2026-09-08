---
title: "View.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "View-eigenschap. Haalt de naam van een View-object op of stelt deze in."
type: docs
weight: 50
url: /nl/net/aspose.tasks/view/name/
---
## View.Name property

Haalt op of stelt de naam van een View-object in.

```csharp
public string Name { get; set; }
```

## Voorbeelden

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


