---
title: "Klasse UsageView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.UsageView klasse. Vertegenwoordigt een usage view in een project"
type: docs
weight: 2650
url: /nl/net/aspose.tasks/usageview/
---
## UsageView class

Stelt een gebruiksweergave in een project voor.

```csharp
public abstract class UsageView : View
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Krijgt of stelt de uitlijning van detailgegevens in. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Krijgt of stelt de instellingen van de onderste timescale-tier van de weergave in. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Krijgt of stelt een waarde in die aangeeft of de details-kopkolom in de weergave moet worden weergegeven of niet. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of korte detailkopnamen al dan niet worden weergegeven. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Haalt op of stelt een filter in dat wordt gebruikt in een enkele weergave. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Haalt op of stelt een groep van de enkele weergave in. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project het filter voor een enkele weergave markeert. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Haalt op of stelt instellingen van de middelste tijdschaallaag van de weergave in. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Haalt op of stelt de naam van een View-object in. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Haalt een instantie van de [`PageInfo`](../view/pageinfo/) klasse op. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in het mpp-bestandsformaat. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Haalt de bovenliggende van het View-object op. Alleen-lezen [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de detailkop op alle toewijzingsrijen moet worden herhaald of niet. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Haalt het schermtype voor de enkele weergave op. Alleen-lezen [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Andere weergaven‑keuzelijsten in het lint. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Haalt op of stelt een tabel van de enkele weergave in. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Haalt op of stelt instellingen van de bovenste tijdschaallaag van de weergave in. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

Toont hoe een taakgebruikweergave met details te renderen.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// haal de weergave op
UsageView view = (TaskUsageView)project.DefaultView;

// detailkopkolom wordt niet weergegeven
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// toon detailkopkolom
view.DisplayDetailsHeaderColumn = true;

// herhaal detailkop op alle toewijzingsrijen
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


