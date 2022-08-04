---
title: CsvOptions
second_title: Aspose.Tasks för .NET API-referens
description: Tillåter att ange ytterligare alternativ när du sparar projekt till CSV.
type: docs
weight: 1710
url: /sv/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Tillåter att ange ytterligare alternativ när du sparar projekt till CSV.

```csharp
public class CsvOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [CsvOptions](csvoptions)() | Initierar en ny instans av[`CsvOptions`](../csvoptions) klass som kan användas för att spara projekt i CSV-format. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Hämtar eller ställer in listan över instanserna av[`BarStyle`](../../aspose.tasks.visualization/barstyle) klass som visas i projektvyn. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Hämtar eller ställer in den anpassade sidstorleken i poäng (1 punkt = 1/72 tum). |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory) { get; set; } | Hämtar eller ställer in en datakategori som ska sparas. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Hämtar eller ställer in ett värde som indikerar om icke-arbetstid ska dras (standardvärdet är TRUE). |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding) { get; set; } | Hämtar eller ställer in en kodning att spara CSV med. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Hämtar eller ställer in ett datum att slutföra renderingen till. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Hämtar eller ställer in ett värde som anger om radhöjden ska ökas för att passa dess innehåll. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Hämtar eller ställer in en lista över[`Gridline`](../../aspose.tasks.visualization/gridline) som visas i projektvyn. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders) { get; set; } | Hämtar eller ställer in ett värde som anger om rubriker ska inkluderas eller inte (standardvärdet är TRUE). |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Hämtar eller ställer in ett värde som anger om förklaring ska visas på varje sida (standardvärdet är TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Hämtar eller ställer in ett värde som anger om kritiska uppgifter ska visas i röd färg (standardvärdet är FALSK). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Hämtar eller ställer in färgen för icke-arbetstid. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Hämtar eller ställer in antalet sidor i projektet. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Hämtar eller ställer in storleken på sidan som ska renderas (standardvärdet är PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Hämtar eller ställer in[`PresentationFormat`](../saveoptions/presentationformat) där dokumentet kommer att sparas. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Hämtar eller ställer in ett värde som anger om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. Sidstorleken kommer att ändras så att det renderade projektet får plats på en sida. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Hämtar eller ställer in ett värde som indikerar om deluppgifter i aktivitetsfältet för sammanfattning ska markeras. För deluppgifter anger fältet Sammanställning om information om Gantt-fälten för deluppgifter kommer att rullas upp till sammanfattande aktivitetsfält. För sammanfattande uppgifter, fältet anger om det sammanfattande aktivitetsfältet visar upprullade staplar. Du måste ha fältet Samlad sammanfattning för sammanfattningsuppgifter inställt på Ja för att eventuella deluppgifter ska rullas upp till dem. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Hämtar eller ställer in formatet som dokumentet kommer att sparas i om detta sparaalternativ-objekt används. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Hämtar eller ställer in datumet att börja rendera från. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Hämtar eller ställer in jämförelsen för att sortera uppgifter på Gantt-diagram och Uppgiftsbladsdiagram. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Hämtar eller ställer in villkoret som används för att filtrera uppgifter som återges på Gantt-, Task Sheet och Task Usage-diagram. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter) { get; set; } | Hämtar eller ställer in en textavgränsare. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Hämtar eller ställer in listan över instanserna av[`TextStyle`](../../aspose.tasks.visualization/textstyle) klass som visas i projektvyn. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Hämtar eller ställer in[`Timescale`](../saveoptions/timescale) värde som används för att styra hur tidsskala (om sådan finns) renderas när projektet sparas i grafiskt format. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Hämtar eller ställer in ett värde som anger om övertoningspensel ska användas vid rendering av Gantt-diagram. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Hämtar eller ställer in en lista över de vykolumner som ska renderas ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Om det inte är inställt renderas uppgifts-ID, uppgiftsnamn, start och slut endast. Om både View och[`ViewSettings`](../saveoptions/viewsettings) egenskaper är inställda, kolumner från View åsidosätter kolumner från ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Hämtar eller ställer in en vy ([`View`](../saveoptions/view) att återge. Du kan använda de här alternativen för att uttryckligen ange vilken vy som ska sparas i PDF-, HTML- eller bildformat. Om den här egenskapen är inställd,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) egenskapen ignoreras när projektet sparas. Vyn ska vara från en av följande skärmar (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
