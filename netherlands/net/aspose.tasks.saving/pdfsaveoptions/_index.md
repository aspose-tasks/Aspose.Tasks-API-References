---
title: PdfSaveOptions
second_title: Aspose.Tasks voor .NET API-referentie
description: Maakt het mogelijk om extra opties te specificeren bij het renderen van projectpaginas naar PDF.
type: docs
weight: 1860
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Maakt het mogelijk om extra opties te specificeren bij het renderen van projectpagina's naar PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Initialiseert een nieuw exemplaar van het`PdfSaveOptions`klasse die kan worden gebruikt om een document op te slaan in de[`Pdf`](../savefileformat/) formaat. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Haalt of stelt de lijst met instanties van het[`BarStyle`](../../aspose.tasks.visualization/barstyle/) klasse die in de projectweergave verschijnen. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Haalt of stelt een gewenst nalevingsniveau in voor gegenereerd PDF-document. Standaard isPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Hiermee wordt het aangepaste paginaformaat in punten opgehaald of ingesteld (1 punt = 1/72 inch). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname/) { get; set; } | Hiermee wordt het standaardlettertype voor weergave opgehaald of ingesteld. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Haalt of stelt een digitale handtekening in. Indien niet ingesteld, wordt er niet ondertekend. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Haalt of stelt een waarde in die aangeeft of niet-werktijd moet worden getekend (standaardwaarde is TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Verkrijgt of stelt coderingsdetails in. Indien niet ingesteld, wordt er geen codering uitgevoerd. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Haalt een datum op of stelt deze in om het renderen te voltooien naar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de rijhoogte moet worden verhoogd om in de inhoud te passen. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Bepaalt of stelt in of een kalendersectie van een weergave moet worden weergegeven aan het einde (rechterkant) van de laatste pagina. Als de waarde onwaar is, wordt de kalendersectie precies weergegeven op EndDate, zelfs als er een lege ruimte op een pagina is. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback/) { get; set; } | Krijgt of stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Haalt of stelt een lijst van[`Gridline`](../../aspose.tasks.visualization/gridline/) die verschijnen in projectweergave. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de legenda op elke pagina moet worden weergegeven (standaardwaarde is TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Haalt of stelt een waarde in die aangeeft of kritieke taken in rood moeten worden weergegeven (standaardwaarde is FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Krijgt of stelt de niet-werktijdkleur in. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Haalt het aantal pagina's van het project op of stelt het in. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Haalt de lijst met paginanummers op of stelt deze in om op te slaan wanneer de projectlay-out in afzonderlijke bestanden wordt opgeslagen. Alle pagina's worden opgeslagen als deze lijst leeg is. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Krijgt of stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een uitvoerstroom voor elke weergegeven pagina te krijgen. Is van toepassing wanneer[`SaveToSeparateFiles`](./savetoseparatefiles/) optie wordt gebruikt. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Hiermee wordt de grootte van de weer te geven pagina opgehaald of ingesteld (standaardwaarde is PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Haalt of stelt de[`PresentationFormat`](../saveoptions/presentationformat/) waarin het document wordt opgeslagen. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Haalt of stelt een waarde in die aangeeft of een opening tussen de laatste taak en de voettekst moet worden verkleind. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een project op één pagina moet worden weergegeven wanneer het project in grafische indeling wordt opgeslagen. Het paginaformaat wordt gewijzigd zodat het gerenderde project op één pagina past. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of subtaken op de overzichtstaakbalk moeten worden gemarkeerd. Voor subtaken geeft het veld Rollup aan of informatie over de Gantt-balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor overzichtstaken, de Rollup veld geeft aan of de overzichtstaakbalk opgerolde balken weergeeft. U moet het veld Samenvouwen voor overzichtstaken hebben ingesteld op Ja om subtaken te kunnen samenvoegen. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Hiermee wordt de indeling waarin het document wordt opgeslagen als dit object voor opslagopties wordt gebruikt, opgehaald of ingesteld. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Haalt of stelt een waarde in die aangeeft of projectpagina's in afzonderlijke bestanden moeten worden opgeslagen. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Haalt of stelt de datum in om te beginnen met renderen vanaf. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Haalt of stelt de vergelijker in om taken te sorteren op Gantt-diagram en Taakblad-diagram. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Hiermee wordt de voorwaarde opgehaald of ingesteld die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, taakblad- en taakgebruiksdiagrammen. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Hiermee wordt een compressietype opgehaald of ingesteld dat moet worden gebruikt voor alle inhoudsstromen behalve afbeeldingen. Standaard isFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Haalt of stelt de lijst met instanties van het[`TextStyle`](../../aspose.tasks.visualization/textstyle/) klasse die in de projectweergave verschijnen. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Haalt of stelt de[`Timescale`](../saveoptions/timescale/) waarde die wordt gebruikt om te bepalen hoe tijdschaal (indien aanwezig) wordt weergegeven wanneer het project wordt opgeslagen in grafisch formaat. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of het verlooppenseel moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of het standaardlettertype moet worden gebruikt voor weergave. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Haalt of stelt een lijst in van de te renderen weergavekolommen ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Indien niet ingesteld, worden alleen taak-id's, taaknamen, begin en einde weergegeven. Als zowel Bekijken als[`ViewSettings`](../saveoptions/viewsettings/)eigenschappen zijn ingesteld, kolommen uit View overschrijven kolommen uit ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Krijgt of stelt een weergave in ([`View`](../saveoptions/view/) ) renderen. U kunt deze opties gebruiken om expliciet te specificeren welke weergave moet worden opgeslagen in PDF-, HTML- of afbeeldingsindeling. Als deze eigenschap is ingesteld,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) eigenschap wordt genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn uit een van de volgende schermen (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
