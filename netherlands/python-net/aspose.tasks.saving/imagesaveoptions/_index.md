---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Python via .NET API-referentie"
description: 
type: docs
weight: 40
url: /nl/python-net/aspose.tasks.saving/imagesaveoptions/
---

## ImageSaveOptions class

Staat toe om extra opties op te geven bij het renderen van projectpagina's naar afbeeldingen.

Het type ImageSaveOptions bevat de volgende leden:
## Constructors
| Naam | Beschrijving |
| :- | :- |
| ImageSaveOptions(save_format) | Initialiseert een nieuw exemplaar van de [ImageSaveOptions](/tasks/python-net/aspose.tasks.saving/imagesaveoptions/) klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-formaten. |
## Eigenschappen
| Naam | Beschrijving |
| :- | :- |
| save_format |  |
| bar_styles | Haalt de lijst met exemplaren van de [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) klasse op of stelt deze in die verschijnen in de projectweergave. |
| draw_non_working_time | Haalt een waarde op of stelt deze in die aangeeft of niet-werkelijke tijd moet worden getekend (Standaardwaarde is WAAR). |
| end_date | Haalt een datum op of stelt deze in tot wanneer gerenderd moet worden. |
| timescale_fit_behavior | Haalt een gedrag op of stelt dit in dat bepaalt hoe het rechteruiteinde van de tijdlijn moet worden uitgelijnd met het einde van de pagina. |
| fit_content | Haalt een waarde op of stelt deze in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| gridlines | Haalt op of stelt een lijst van [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) in die verschijnen in de projectweergave. |
| legend_drawing_options | Haalt op of stelt een waarde in die bepaalt hoe een legenda wordt gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage. |
| legend_items | Haalt op of stelt een array van PageLegendItem in die bepaalt welke balken moeten worden gerenderd in de paginale legenda.<br/>            Als null, worden de standaarditems gerenderd. |
| mark_critical_tasks | Haalt op of stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (Standaardwaarde is FALSE). |
| non_working_time_color | Haalt op of stelt de kleur voor niet-werkuren in. |
| page_count | Haalt op of stelt het aantal pagina's van het project in. |
| page_size | Haalt op of stelt de grootte van de te renderen pagina in (Standaardwaarde is PageSize.A4). |
| is_portrait | Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
| presentation_format | Haalt op of stelt het [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) in waarin het document wordt opgeslagen. |
| roll_up_gantt_bars | Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden.<br/>            Voor subtaken geeft het Rollup-veld aan of informatie over de subtaken Gantt-balken wordt opgeteld naar de samenvattingstaakbalk.<br/>            Voor samenvattingstaken geeft het Rollup-veld aan of de samenvattingstaakbalk opgetelde balken weergeeft.<br/>            Het Rollup-veld voor samenvattingstaken moet op Ja staan om subtaken naar hen op te tellen. |
| start_date | Haalt op of stelt de datum in vanaf wanneer gerenderd moet worden. |
| text_styles | Haalt op of stelt de lijst van tekststijlen in die worden toegepast tijdens het renderen van een projectweergave. |
| timescale | Haalt op of stelt de [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| use_gradient_brush | Geeft of stelt een waarde in die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de Gantt‑chart. |
| view | Haalt op of stelt een lijst van de weergavekolommen in die moeten worden gerenderd ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Indien niet ingesteld, worden alleen taak‑ID's, taaknamen, start en einde gerenderd.<br/>            Als zowel View als [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) eigenschappen zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| view_settings | Haalt op of stelt een weergave ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen als PDF, HTML of afbeelding.<br/>            Als deze eigenschap is ingesteld, wordt de [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) eigenschap genegeerd wanneer het project wordt opgeslagen.<br/>            De weergave moet afkomstig zijn van een van de volgende schermen (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Haalt op of stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 van een inch). |
| render_to_single_page | Haalt op of stelt een waarde in die aangeeft of een project moet worden gerenderd naar één pagina<br/>            wanneer het project wordt opgeslagen in een grafisch formaat.<br/>            De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| font_settings | Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave. |
| pages | Haalt op of stelt een lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |
| jpeg_quality | Haalt op of stelt een JPEG-kwaliteit in. Het toegestane waardebereik is 0..100. |
| reduce_footer_gap | Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind. |
| tiff_compression | Haalt op of stelt het type compressie in dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |
| pixel_format | Haalt op of stelt het formaat van de kleurgegevens voor elke pixel in de afbeelding in. |
| horizontal_resolution | Haalt op of stelt de horizontale resolutie in dpi in. |
| vertical_resolution | Haalt op of stelt de verticale resolutie in dpi in. |
| page_saving_callback | Haalt of stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te verkrijgen. |

### Zie ook

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

