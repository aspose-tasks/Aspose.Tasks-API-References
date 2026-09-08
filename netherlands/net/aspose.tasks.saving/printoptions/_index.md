---
title: "Klasse PrintOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PrintOptions klasse. Stelt u in staat om extra opties op te geven bij het afdrukken van een project."
type: docs
weight: 2170
url: /nl/net/aspose.tasks.saving/printoptions/
---
## PrintOptions class

Staat toe extra opties op te geven bij het afdrukken van een project.

```csharp
public class PrintOptions : SaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrintOptions](printoptions/)() | Initialiseert een nieuw exemplaar van de `PrintOptions` klasse die kan worden gebruikt om verschillende opties in te stellen voor het afdrukken van een project. |

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
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Haalt op of stelt de [`PresentationFormat`](../saveoptions/presentationformat/) in waarin het document wordt opgeslagen. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingstaakbalk opgerolde balken weergeeft. Het Rollup‑veld voor samenvattingstaken moet op Ja staan om subtaken naar hen op te rollen. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Haalt op of stelt de datum in vanaf wanneer gerenderd moet worden. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Haalt op of stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Haalt op of stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Haalt op of stelt de [`Timescale`](../saveoptions/timescale/)‑waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Haalt op of stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Haalt op of stelt een lijst met weergavekolommen in die moeten worden gerenderd ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Indien niet ingesteld, worden alleen taak‑ID’s, taaknamen, start‑ en einddatums gerenderd. Als zowel View als de eigenschap [`ViewSettings`](../saveoptions/viewsettings/) zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Haalt op of stelt een weergave ([`View`](../saveoptions/view/)) in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen in PDF‑, HTML‑ of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de eigenschap [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn van een van de volgende schermen (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Voorbeelden

Toont hoe afdrukopties te gebruiken.

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Zie ook

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


