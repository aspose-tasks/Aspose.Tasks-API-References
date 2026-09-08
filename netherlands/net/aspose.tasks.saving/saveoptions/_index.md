---
title: "Klasse SaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.SaveOptions klasse. Dit is een abstracte basisklasse voor klassen die de gebruiker in staat stelt extra opties op te geven bij het opslaan van een project in een bepaald formaat."
type: docs
weight: 2190
url: /nl/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

Dit is een abstracte basisklasse voor klassen die de gebruiker toestaan extra opties op te geven bij het opslaan van een project in een bepaald formaat.

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Haalt op of stelt de lijst van instanties van de [`BarStyle`](../../aspose.tasks.visualization/barstyle/) klasse in die verschijnen in de projectweergave. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Haalt op of stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of niet-werkelijke tijd moet worden getekend (Standaardwaarde is WAAR). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Haalt op of stelt een datum in waarop het renderen moet worden voltooid. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Haalt op of stelt een lijst van [`Gridline`](../../aspose.tasks.visualization/gridline/) in die verschijnen in de projectweergave. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; geeft onwaar terug als de paginarichting landschap is. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Haalt op of stelt een waarde in die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Haalt op of stelt een array van PageLegendItem in die bepaalt welke balken in de paginalegenda moeten worden gerenderd. Indien null, worden de standaarditems gerenderd. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (Standaardwaarde is ONWAAR). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Haalt op of stelt de kleur voor niet-werkelijke tijd in. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Haalt op of stelt het aantal pagina's van het project in. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Haalt op of stelt de grootte van de te renderen pagina in (Standaardwaarde is PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Haalt op of stelt de [`PresentationFormat`](./presentationformat/) in waarin het document wordt opgeslagen. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingstaakbalk opgerolde balken weergeeft. Het Rollup‑veld voor samenvattingstaken moet op Ja staan om subtaken naar hen op te rollen. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Haalt op of stelt de datum in vanaf wanneer gerenderd moet worden. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Haalt op of stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Haalt op of stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Haalt op of stelt de [`Timescale`](./timescale/) waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer een project wordt opgeslagen in een grafisch formaat. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Haalt op of stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Haalt een lijst op of stelt deze in van de weergavekolommen die moeten worden gerenderd ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Indien niet ingesteld, worden alleen taak‑ID's, taaknamen, start‑ en einddatums gerenderd. Als zowel View‑ als [`ViewSettings`](./viewsettings/)‑eigenschappen zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Haalt een weergave op of stelt deze in ([`View`](./view/)) die moet worden gerenderd. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen naar PDF-, HTML- of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) eigenschap genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn van een van de volgende schermen (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Opmerkingen

Een instantie van een afgeleide klasse van de SaveOptions‑klasse wordt doorgegeven aan de stream‑Save‑ of string‑Save‑overloads zodat de gebruiker aangepaste opties kan definiëren bij het opslaan van een document.

## Voorbeelden

Toont hoe de optie in te stellen of de rijhoogte moet worden vergroot om de inhoud te passen.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Stel optie fit content in op true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Zie ook

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


