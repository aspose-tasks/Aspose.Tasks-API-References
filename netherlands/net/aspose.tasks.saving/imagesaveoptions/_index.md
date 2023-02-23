---
title: ImageSaveOptions
second_title: Aspose.Tasks voor .NET API-referentie
description: Maakt het mogelijk om extra opties te specificeren bij het renderen van projectpaginas naar afbeeldingen.
type: docs
weight: 1770
url: /nl/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Maakt het mogelijk om extra opties te specificeren bij het renderen van projectpagina's naar afbeeldingen.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | Initialiseert een nieuw exemplaar van het`ImageSaveOptions` klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-indeling. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Haalt of stelt de lijst met instanties van het[`BarStyle`](../../aspose.tasks.visualization/barstyle/) klasse die in de projectweergave verschijnen. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Hiermee wordt het aangepaste paginaformaat in punten opgehaald of ingesteld (1 punt = 1/72 inch). |
| [DefaultFontName](../../aspose.tasks.saving/imagesaveoptions/defaultfontname/) { get; set; } | Hiermee wordt het standaardlettertype voor weergave opgehaald of ingesteld. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Haalt of stelt een waarde in die aangeeft of niet-werktijd moet worden getekend (standaardwaarde is TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Haalt een datum op of stelt deze in om het renderen te voltooien naar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de rijhoogte moet worden verhoogd om in de inhoud te passen. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Bepaalt of stelt in of een kalendersectie van een weergave moet worden weergegeven aan het einde (rechterkant) van de laatste pagina. Als de waarde onwaar is, wordt de kalendersectie precies weergegeven op EndDate, zelfs als er een lege ruimte op een pagina is. |
| [FontResolveCallback](../../aspose.tasks.saving/imagesaveoptions/fontresolvecallback/) { get; set; } | Krijgt of stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Haalt of stelt een lijst van[`Gridline`](../../aspose.tasks.visualization/gridline/) die verschijnen in projectweergave. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | Haalt of stelt de horizontale resolutie in dpi in. |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | Haalt of stelt een JPEG-kwaliteit in. Het toegestane waardebereik is 0..100. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de legenda op elke pagina moet worden weergegeven (standaardwaarde is TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Haalt of stelt een waarde in die aangeeft of kritieke taken in rood moeten worden weergegeven (standaardwaarde is FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Krijgt of stelt de niet-werktijdkleur in. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Haalt het aantal pagina's van het project op of stelt het in. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Haalt een lijst met paginanummers op of stelt deze in om op te slaan wanneer de projectlay-out in afzonderlijke bestanden wordt opgeslagen. Alle pagina's worden opgeslagen als deze lijst leeg is. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Krijgt of stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te krijgen. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Hiermee wordt de grootte van de weer te geven pagina opgehaald of ingesteld (standaardwaarde is PageSize.A4). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Hiermee wordt de indeling van de kleurgegevens voor elke pixel in de afbeelding opgehaald of ingesteld. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Haalt of stelt de[`PresentationFormat`](../saveoptions/presentationformat/) waarin het document wordt opgeslagen. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Haalt of stelt een waarde in die aangeeft of een opening tussen de laatste taak en de voettekst moet worden verkleind. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een project op één pagina moet worden weergegeven wanneer het project in grafische indeling wordt opgeslagen. Het paginaformaat wordt gewijzigd zodat het gerenderde project op één pagina past. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of subtaken op de overzichtstaakbalk moeten worden gemarkeerd. Voor subtaken geeft het veld Rollup aan of informatie over de Gantt-balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor overzichtstaken, de Rollup veld geeft aan of de overzichtstaakbalk opgerolde balken weergeeft. U moet het veld Samenvouwen voor overzichtstaken hebben ingesteld op Ja om subtaken te kunnen samenvoegen. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Hiermee wordt de indeling waarin het document wordt opgeslagen als dit object voor opslagopties wordt gebruikt, opgehaald of ingesteld. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Haalt of stelt de datum in om te beginnen met renderen vanaf. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Haalt of stelt de vergelijker in om taken te sorteren op Gantt-diagram en Taakblad-diagram. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Hiermee wordt de voorwaarde opgehaald of ingesteld die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, taakblad- en taakgebruiksdiagrammen. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Haalt of stelt de lijst met instanties van het[`TextStyle`](../../aspose.tasks.visualization/textstyle/) klasse die in de projectweergave verschijnen. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Hiermee wordt het type compressie opgehaald of ingesteld dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in de TIFF-indeling. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Haalt of stelt de[`Timescale`](../saveoptions/timescale/) waarde die wordt gebruikt om te bepalen hoe tijdschaal (indien aanwezig) wordt weergegeven wanneer het project wordt opgeslagen in grafisch formaat. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of het verlooppenseel moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of het standaardlettertype moet worden gebruikt voor weergave. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | Haalt of stelt de verticale resolutie in dpi in. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Haalt of stelt een lijst in van de te renderen weergavekolommen ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Indien niet ingesteld, worden alleen taak-id's, taaknamen, begin en einde weergegeven. Als zowel Bekijken als[`ViewSettings`](../saveoptions/viewsettings/)eigenschappen zijn ingesteld, kolommen uit View overschrijven kolommen uit ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Krijgt of stelt een weergave in ([`View`](../saveoptions/view/) ) renderen. U kunt deze opties gebruiken om expliciet te specificeren welke weergave moet worden opgeslagen in PDF-, HTML- of afbeeldingsindeling. Als deze eigenschap is ingesteld,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) eigenschap wordt genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn uit een van de volgende schermen (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
