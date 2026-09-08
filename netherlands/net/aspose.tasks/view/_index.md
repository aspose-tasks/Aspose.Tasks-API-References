---
title: "Klasse View"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.View klasse. Vertegenwoordigt een weergave in Project"
type: docs
weight: 2890
url: /nl/net/aspose.tasks/view/
---
## View class

Stelt een weergave in Project voor.

```csharp
public class View : IComparable<View>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [View](view/#constructor)() | Initialiseert een nieuw exemplaar van de `View` klasse. |
| [View](view/#constructor_1)(ViewScreen) | Initialiseert een nieuw exemplaar van de `View` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Haalt op of stelt een filter in dat wordt gebruikt in een enkele weergave. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Haalt op of stelt een groep van de enkele weergave in. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project het filter voor een enkele weergave markeert. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Haalt op of stelt de naam van een View-object in. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Haalt een exemplaar op van de [`PageInfo`](./pageinfo/) klasse. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in het mpp-bestandsformaat. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Haalt de bovenliggende van het View-object op. Alleen-lezen [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Haalt het schermtype voor de enkele weergave op. Alleen-lezen [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Andere weergaven‑keuzelijsten in het lint. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Haalt op of stelt een tabel van de enkele weergave in. |
| [Type](../../aspose.tasks/view/type/) { get; } | Haalt het type item in de enkele weergave op, zoals taken of resources. Alleen-lezen [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Haalt de unieke identifier van een weergave op. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Haalt een collectie objecten op die de plaatsing en weergave van [`OleObject`](../oleobject/) in de weergave vertegenwoordigen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Vergelijkt de huidige instantie met een ander object van hetzelfde type en retourneert een geheel getal dat aangeeft of de huidige instantie voorafgaat, volgt of zich op dezelfde positie in de sorteervolgorde bevindt als het andere object. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Retourneert een hashcode‑waarde voor de instantie van de [`Resource`](../resource/) klasse. |
| [operator ==](../../aspose.tasks/view/op_equality/) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


