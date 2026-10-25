---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 90
url: /sv/python-net/aspose.tasks.saving/pdfsaveoptions/
---

## PdfSaveOptions class

Tillåter att ange ytterligare alternativ när projektsidor renderas till PDF.

Typen PdfSaveOptions exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| PdfSaveOptions() | Initierar en ny instans av klassen [PdfSaveOptions](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) som kan användas för att spara ett dokument i |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| save_format |  |
| bar_styles | Hämtar eller anger listan med instanser av klassen [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) som visas i projektvyn. |
| draw_non_working_time | Hämtar eller anger ett värde som indikerar om icke-arbetstid ska ritas (Standardvärde är TRUE). |
| end_date | Hämtar eller anger ett datum att slutföra rendering till. |
| timescale_fit_behavior | Hämtar eller anger ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut. |
| fit_content | Hämtar eller anger ett värde som indikerar om radhöjden ska ökas för att passa innehållet. |
| gridlines | Hämtar eller anger en lista med [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) som visas i projektvyn. |
| legend_drawing_options | Hämtar eller anger ett värde som definierar hur en legend ska renderas. Standardvärde är LegendDrawingOptions.OnEveryPage. |
| legend_items | Hämtar eller anger en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden.<br/>            Om null renderas standardobjekten. |
| mark_critical_tasks | Hämtar eller anger ett värde som indikerar om kritiska uppgifter ska visas i röd färg (Standardvärde är FALSE). |
| non_working_time_color | Hämtar eller anger färgen för icke-arbetstid. |
| page_count | Hämtar eller anger antalet sidor i projektet. |
| page_size | Hämtar eller anger sidans storlek som ska renderas (Standardvärde är PageSize.A4). |
| is_portrait | Hämtar eller anger ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |
| presentation_format | Hämtar eller anger [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) som dokumentet ska sparas i. |
| roll_up_gantt_bars | Hämtar eller anger ett värde som indikerar om deluppgifter på sammanfattningsuppgiftens stapel ska markeras.<br/>            För deluppgifter indikerar Rollup-fältet om information på deluppgiftens Gantt-staplar kommer att rullas upp till sammanfattningsuppgiftens stapel.<br/>            För sammanfattningsuppgifter indikerar Rollup-fältet om stapeln för sammanfattningsuppgiften visar upprullade staplar.<br/>            Du måste ha Rollup-fältet för sammanfattningsuppgifter inställt på Ja för att någon deluppgift ska kunna rullas upp till dem. |
| start_date | Hämtar eller anger datumet att börja rendera från. |
| text_styles | Hämtar eller anger listan med textstilar som tillämpas under rendering av en projektvy. |
| timescale | Hämtar eller anger värdet för [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) som används för att kontrollera hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format. |
| use_gradient_brush | Hämtar eller anger ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram. |
| view | Hämtar eller anger en lista med visningskolumner som ska renderas ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Om den inte är angiven renderas endast uppgifts‑ID, uppgiftsnamn, start och slut.<br/>            Om både View och [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) egenskaper är angivna, åsidosätter kolumner från View kolumner från ViewSettings. |
| view_settings | Hämtar eller anger en vy ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) att rendera. Du kan använda detta alternativ för att uttryckligen ange vilken vy som ska sparas till PDF-, HTML- eller Bildformat.<br/>            Om denna egenskap är angiven ignoreras egenskapen [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) när projektet sparas.<br/>            Vyn ska komma från en av följande skärmar (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Hämtar eller anger den anpassade sidstorleken i punkter (1 punkt = 1/72 tum). |
| render_to_single_page | Hämtar eller anger ett värde som indikerar om ett projekt ska renderas till en enda sida<br/>            när projektet sparas i grafiskt format.<br/>            Sidstorleken kommer att ändras så att det renderade projektet får plats på en sida. |
| reduce_footer_gap | Hämtar eller anger ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas. |
| compliance | Hämtar eller anger en önskad efterlevnadsnivå för genererat PDF-dokument.<br/>            Standard är [PDF15](/tasks/python-net/aspose.tasks.saving/pdfcompliance/). |
| encryption_details | Hämtar eller anger en krypteringsdetalj. Om den inte anges, utförs ingen kryptering. |
| text_compression | Hämtar eller anger en kompressionstyp som ska användas för alla innehållsströmmar förutom bilder.<br/>            Standard är [FLATE](/tasks/python-net/aspose.tasks.saving/pdftextcompression/). |
| digital_signature_details | Hämtar eller anger en digital signaturdetalj. Om den inte anges, utförs ingen signering. |
| save_to_separate_files | Hämtar eller anger ett värde som indikerar om projektsidor ska sparas till separata filer. |
| page_saving_callback | Hämtar eller anger en användardefinierad återuppringning som används för att få en utdataström för varje renderad sida.<br/>            Gäller när alternativet [save_to_separate_files](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) används. |
| pages | Hämtar eller anger listan med sidnummer som ska sparas när projektlayout sparas till separata filer. |
| font_settings | Specificerar teckensnittsinställningar som används vid rendering av projektets vy. |

### Se även

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

