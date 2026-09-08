---
title: "Klasse TimelineView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TimelineView klasse. Vertegenwoordigt een tijdlijnweergave van een project"
type: docs
weight: 2580
url: /nl/net/aspose.tasks/timelineview/
---
## TimelineView class

Stelt een tijdlijnweergave van een project voor.

```csharp
public class TimelineView : View
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TimelineView](timelineview/)() | Initialiseert een nieuwe instantie van de `TimelineView` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft hoe datums op de tijdlijnweergave worden opgemaakt. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of overlappende taken op meerdere rijen worden weergegeven. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Haalt op of stelt een filter in dat wordt gebruikt in een enkele weergave. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Haalt op of stelt een groep van de enkele weergave in. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project het filter voor een enkele weergave markeert. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Haalt op of stelt de naam van een View-object in. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Haalt een instantie van de [`PageInfo`](../view/pageinfo/) klasse op. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in het mpp-bestandsformaat. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Haalt de bovenliggende van het View-object op. Alleen-lezen [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Haalt het schermtype voor de enkele weergave op. Alleen-lezen [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Haalt een waarde op die aangeeft of datums worden weergegeven. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Andere weergaven‑keuzelijsten in het lint. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of pan- en zoombesturing worden weergegeven. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of de tijdschaal wordt weergegeven. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of een lijn die vandaag representeert, wordt weergegeven. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Haalt op of stelt een tabel van de enkele weergave in. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft hoeveel lijnen worden gebruikt om taken in een tijdlijn weer te geven. |
| [Type](../../aspose.tasks/view/type/) { get; } | Haalt het type item in de enkele weergave op, zoals taken of resources. Alleen-lezen [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Haalt de unieke identifier van een weergave op. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Haalt een collectie objecten op die de plaatsing en weergave van [`OleObject`](../oleobject/) in de weergave vertegenwoordigen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Vergelijkt de huidige instantie met een ander object van hetzelfde type en retourneert een geheel getal dat aangeeft of de huidige instantie voorafgaat, volgt of zich op dezelfde positie in de sorteervolgorde bevindt als het andere object. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Retourneert een hashcode‑waarde voor de instantie van de [`Resource`](../resource/) klasse. |

## Voorbeelden

Toont hoe te werken met &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// initialiseer een tijdlijnweergave
var view = new TimelineView();

// stel een waarde in die aangeeft hoe datums op de tijdlijnweergave worden opgemaakt.
view.DateFormat = DateFormat.DateDddDd;
// stel een waarde in die aangeeft of overlappende taken op meerdere rijen worden weergegeven.
view.DisplayOverlapped = true;
// stel een waarde in die aangeeft of pan- en zoombesturing worden weergegeven.
view.ShowPanZoom = true;
// stel een waarde in die aangeeft of de tijdschaal wordt weergegeven.
view.ShowTimescale = true;
// stel een waarde in die aangeeft of een lijn die vandaag representeert, wordt weergegeven.
view.ShowToday = true;
// stel een waarde in die aangeeft hoeveel lijnen worden gebruikt om taken in een tijdlijn weer te geven.
view.TextLinesCount = 2;

// haalt een waarde op die aangeeft of overlappende taken op meerdere rijen worden weergegeven.
Console.WriteLine("Show Dates: " + view.ShowDates);

// voeg de weergave toe aan het project
project.Views.Add(view);

// voeg wat testgegevens toe aan het project
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


