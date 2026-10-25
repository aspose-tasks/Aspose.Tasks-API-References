---
title: "Klasse PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfSaveOptions klasse. Stelt u in staat extra opties op te geven bij het renderen van projectpagina's naar PDF"
type: docs
weight: 2130
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Staat toe extra opties op te geven bij het renderen van projectpagina's naar PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Initialiseert een nieuw exemplaar van de `PdfSaveOptions` klasse die kan worden gebruikt om een document op te slaan in het [`PDF`](../savefileformat/) formaat. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Haalt op of stelt de lijst van instanties van de [`BarStyle`](../../aspose.tasks.visualization/barstyle/) klasse in die verschijnen in de projectweergave. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Haalt op of stelt een gewenst conformiteitsniveau in voor het gegenereerde PDF‑document. Standaard is Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Haalt op of stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Haalt op of stelt details van een digitale handtekening in. Indien niet ingesteld, wordt er geen ondertekening uitgevoerd. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of niet-werkelijke tijd moet worden getekend (Standaardwaarde is WAAR). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Haalt op of stelt encryptiedetails in. Indien niet ingesteld, wordt er geen encryptie uitgevoerd. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Haalt op of stelt een datum in waarop het renderen moet worden voltooid. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | Specificeert de fontinstellingen die worden gebruikt bij het renderen van de projectweergave. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Haalt op of stelt een lijst van [`Gridline`](../../aspose.tasks.visualization/gridline/) in die verschijnen in de projectweergave. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; geeft onwaar terug als de paginarichting landschap is. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Haalt op of stelt een waarde in die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Haalt op of stelt een array van PageLegendItem in die bepaalt welke balken in de paginalegenda moeten worden gerenderd. Indien null, worden de standaarditems gerenderd. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (Standaardwaarde is ONWAAR). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Haalt op of stelt de kleur voor niet-werkelijke tijd in. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Haalt op of stelt het aantal pagina's van het project in. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Haalt op of stelt de lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. Alle pagina's worden opgeslagen als deze lijst leeg is. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Haalt op of stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. Van toepassing wanneer de optie [`SaveToSeparateFiles`](./savetoseparatefiles/) wordt gebruikt. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Haalt op of stelt de grootte van de te renderen pagina in (Standaardwaarde is PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Haalt op of stelt de [`PresentationFormat`](../saveoptions/presentationformat/) in waarin het document wordt opgeslagen. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingstaakbalk opgerolde balken weergeeft. Het Rollup‑veld voor samenvattingstaken moet op Ja staan om subtaken naar hen op te rollen. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Haalt op of stelt de datum in vanaf wanneer gerenderd moet worden. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Haalt op of stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Haalt op of stelt een compressietype in dat moet worden gebruikt voor alle content‑streams behalve afbeeldingen. Standaard is Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Haalt op of stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Haalt op of stelt de [`Timescale`](../saveoptions/timescale/)‑waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Haalt op of stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Haalt op of stelt een lijst met weergavekolommen in die moeten worden gerenderd ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Indien niet ingesteld, worden alleen taak‑ID’s, taaknamen, start‑ en einddatums gerenderd. Als zowel View als de eigenschap [`ViewSettings`](../saveoptions/viewsettings/) zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Haalt op of stelt een weergave ([`View`](../saveoptions/view/)) in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen in PDF‑, HTML‑ of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de eigenschap [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn van een van de volgende schermen (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Voorbeelden

Toont hoe geselecteerde pagina's van een project kunnen worden opgeslagen in een PDF‑bestand.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// laten we controleren hoeveel pagina's kunnen worden geëxporteerd
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


