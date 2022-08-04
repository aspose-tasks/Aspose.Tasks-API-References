---
title: PdfSaveOptions
second_title: Aspose.Tasks för .NET API-referens
description: Gör det möjligt att ange ytterligare alternativ när projektsidor renderas till PDF.
type: docs
weight: 1850
url: /sv/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Gör det möjligt att ange ytterligare alternativ när projektsidor renderas till PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Initierar en ny instans av[`PdfSaveOptions`](../pdfsaveoptions)klass som kan användas för att spara ett dokument i[`PDF`](../savefileformat) formatera. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Hämtar eller ställer in listan över instanserna av[`BarStyle`](../../aspose.tasks.visualization/barstyle) klass som visas i projektvyn. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance) { get; set; } | Hämtar eller ställer in en önskad efterlevnadsnivå för genererat PDF-dokument. Standard ärPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Hämtar eller ställer in den anpassade sidstorleken i poäng (1 punkt = 1/72 tum). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname) { get; set; } | Hämtar eller ställer in standardteckensnittet för rendering. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails) { get; set; } | Hämtar eller ställer in information om en digital signatur. Om inte inställt kommer ingen signering att utföras. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Hämtar eller ställer in ett värde som indikerar om icke-arbetstid ska dras (standardvärdet är TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails) { get; set; } | Hämtar eller ställer in en krypteringsinformation. Om inte inställt kommer ingen kryptering att utföras. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Hämtar eller ställer in ett datum att slutföra renderingen till. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Hämtar eller ställer in ett värde som anger om radhöjden ska ökas för att passa dess innehåll. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback) { get; set; } | Hämtar eller ställer in en återuppringning som kan användas för att anpassa lösta teckensnitt. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Hämtar eller ställer in en lista över[`Gridline`](../../aspose.tasks.visualization/gridline) som visas i projektvyn. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Hämtar eller ställer in ett värde som anger om förklaring ska visas på varje sida (standardvärdet är TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Hämtar eller ställer in ett värde som anger om kritiska uppgifter ska visas i röd färg (standardvärdet är FALSK). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Hämtar eller ställer in färgen för icke-arbetstid. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Hämtar eller ställer in antalet sidor i projektet. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages) { get; set; } | Hämtar eller ställer in listan med sidnummer som ska sparas när projektlayouten sparas i separata filer. Alla sidor kommer att sparas om listan är tom. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback) { get; set; } | Hämtar eller ställer in en användardefinierad callback som används för att få en utdataström för varje renderad sida. Är tillämpligt när[`SaveToSeparateFiles`](./savetoseparatefiles) alternativet används. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Hämtar eller ställer in storleken på sidan som ska renderas (standardvärdet är PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Hämtar eller ställer in[`PresentationFormat`](../saveoptions/presentationformat) där dokumentet kommer att sparas. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap) { get; set; } | Hämtar eller ställer in ett värde som indikerar om ett gap mellan den senaste uppgiften och sidfoten måste minskas. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Hämtar eller ställer in ett värde som anger om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. Sidstorleken kommer att ändras så att det renderade projektet får plats på en sida. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Hämtar eller ställer in ett värde som indikerar om deluppgifter i aktivitetsfältet för sammanfattning ska markeras. För deluppgifter anger fältet Sammanställning om information om Gantt-fälten för deluppgifter kommer att rullas upp till sammanfattande aktivitetsfält. För sammanfattande uppgifter, fältet anger om det sammanfattande aktivitetsfältet visar upprullade staplar. Du måste ha fältet Samlad sammanfattning för sammanfattningsuppgifter inställt på Ja för att eventuella deluppgifter ska rullas upp till dem. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Hämtar eller ställer in formatet som dokumentet kommer att sparas i om detta sparaalternativ-objekt används. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles) { get; set; } | Hämtar eller ställer in ett värde som anger om projektsidor ska sparas till separata filer. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Hämtar eller ställer in datumet att börja rendera från. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Hämtar eller ställer in jämförelsen för att sortera uppgifter på Gantt-diagram och Uppgiftsbladsdiagram. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Hämtar eller ställer in villkoret som används för att filtrera uppgifter som återges på Gantt-, Task Sheet och Task Usage-diagram. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression) { get; set; } | Hämtar eller ställer in en komprimeringstyp som ska användas för alla innehållsströmmar utom bilder. Standard ärFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Hämtar eller ställer in listan över instanserna av[`TextStyle`](../../aspose.tasks.visualization/textstyle) klass som visas i projektvyn. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Hämtar eller ställer in[`Timescale`](../saveoptions/timescale) värde som används för att styra hur tidsskala (om sådan finns) renderas när projektet sparas i grafiskt format. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Hämtar eller ställer in ett värde som anger om övertoningspensel ska användas vid rendering av Gantt-diagram. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont) { get; set; } | Hämtar eller ställer in ett värde som anger om standardteckensnittet måste användas för rendering. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Hämtar eller ställer in en lista över de vykolumner som ska renderas ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Om det inte är inställt renderas uppgifts-ID, uppgiftsnamn, start och slut endast. Om både View och[`ViewSettings`](../saveoptions/viewsettings) egenskaper är inställda, kolumner från View åsidosätter kolumner från ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Hämtar eller ställer in en vy ([`View`](../saveoptions/view) att återge. Du kan använda de här alternativen för att uttryckligen ange vilken vy som ska sparas i PDF-, HTML- eller bildformat. Om den här egenskapen är inställd,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) egenskapen ignoreras när projektet sparas. Vyn ska vara från en av följande skärmar (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
