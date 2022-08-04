---
title: Project
second_title: Aspose.Tasks för .NET API-referens
description: Representerar ett projekt.
type: docs
weight: 1180
url: /sv/net/aspose.tasks/project/
---
## Project class

Representerar ett projekt.

```csharp
public class Project
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Project](project#constructor)() | Initierar en ny instans av[`Project`](../project) class. |
| [Project](project#constructor_1)(DbSettings) | Initierar en ny instans av[`Project`](../project) klass för att läsa data från en databas som specificeras av instansen av[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) class. |
| [Project](project#constructor_2)(Stream) | Initierar en ny instans av[`Project`](../project) klass från en ström. |
| [Project](project#constructor_9)(StreamReader) | Initierar en ny instans av[`Project`](../project) klass från en StreamReader-instans. |
| [Project](project#constructor_10)(string) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig mpp eller mpt-fil). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Initierar en ny instans av[`Project`](../project) klass från Stream med den angivna instansen av[`LoadOptions`](../loadoptions) class. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig mpp- eller mpt-fil). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Initierar en ny instans av[`Project`](../project) klass från Stream med den angivna instansen av[`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project#constructor_8)(Stream, string) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig mpp- eller mpt-fil). |
| [Project](project#constructor_11)(string, LoadOptions) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig mpp- eller mpt-fil) med den angivna instansen av[`LoadOptions`](../loadoptions) class. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig mpp eller mpt-fil). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Initierar en ny instans av[`Project`](../project) klass från en mall (befintlig MPP- eller MPT-fil) med den angivna instansen av[`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project#constructor_16)(string, string) | Initierar en ny instans av[`Project`](../project) klass från en lösenordsskyddad mall (befintlig mpp- eller mpt-fil). |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Hämtar projektets inbyggda egenskapssamling. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Hämtar eller ställer in beräkningsläge för ett projekt. Kan vara ett av värdena för[`CalculationMode`](./calculationmode) uppräkning. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Blir[`CalendarCollection`](../calendarcollection) objekt för denna projektinstans. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Hämtar en samling som innehåller en lista över kritiska uppgifter som utgör Kritisk väg för detta projekt. Detta är en O(n) operation, där n är antalet uppgifter i projektet. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Hämtar projektets samling av anpassade egenskaper. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Hämtar eller ställer in standardvy för projektet. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Hämtar instansen av[`WeekDayCollection`](../weekdaycollection) klass som representerar en samling av projektets standardveckors arbetsdagar och arbetstider. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Hämtar en instans av[`ProjectDisplayOptions`](../projectdisplayoptions) class. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | får ExtendedAttributeDefinitionCollection-objekt. Samlingen av utökade attributdefinitioner (anpassade fält) som är kopplade till ett projekt. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Hämtar en samling som innehåller instanserna av[`OleObject`](../oleobject) klass som är länkade eller inbäddade i denna projektfil. Endast tillgängligt för mpp-filformat. Den här samlingen är skrivskyddad förutom för "Rensa". |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Hämtar OutlineCodeDefinitionCollection-objekt. Samlingen av dispositionskoddefinitioner som är kopplade till ett projekt. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Hämtar ResourceAssignmentCollection-objekt. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Får alla resursbaserade filterdefinitioner. ResourceFilters är en samling av[`Filter`](../filter) objekt. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Hämtar alla resursbaserade gruppdefinitioner. ResourceGroups är en samling av[`Group`](../group) objekt. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Hämtar ResourceCollection-objekt. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Hämtar roten till uppgiftsträdet. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Får en lista över[`Table`](../table) objekt. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Får alla uppgiftsbaserade filterdefinitioner. TaskFilters är en samling av[`Filter`](../filter) objekt. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Får alla uppgiftsbaserade gruppdefinitioner. TaskGroups är en samling av[`Group`](../group) objekt. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Blir[`TaskLinkCollection`](../tasklinkcollection) objekt. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Hämtar en instans av[`VbaProject`](./vbaproject) class. |
| [Views](../../aspose.tasks/project/views) { get; } | Får en lista över[`View`](../view) objekt. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Hämtar eller ställer in WBS Code Definition för projektet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Kopierar projektets huvuddata och egenskaper till ett annat projekt. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Kopierar projektets huvuddata och egenskaper till ett annat projekt. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Rekursivt räknar upp alla projektets uppgifter inklusive rotuppgiften. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Returnerar värdet som egenskapen är mappad till i den här behållaren. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Returnerar baslinjespartiden. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Blir[`Duration`](../duration) objekt med angivet antal enheter och standardvaraktighetsformat som definieras i projektets inställningar[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Blir[`Duration`](../duration) objekt med det angivna antalet[`TimeUnitType`](../timeunittype) enheter. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Blir[`Duration`](../duration) objekt med det angivnaTimeSpan värde och specificerat[`TimeUnitType`](../timeunittype) värde. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Returnerar sidantal för projektet som ska renderas med standard[`Timescale`](../../aspose.tasks.visualization/timescale) (Dagar). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Returnerar sidantal för projektet som ska renderas med standard[`Timescale`](../../aspose.tasks.visualization/timescale) (Dagar) och givet[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Returnerar antalet sidor för projektet som ska renderas med given[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../aspose.tasks.visualization/timescale) och[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../aspose.tasks.visualization/timescale) och[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) och datumintervall. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Returnerar en samling uppgiftslänkar som är föregångare till den angivna uppgiften. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Blir[`Duration`](../duration) objekt med det angivnaDouble värde och standard arbetsformat. |
| [Print](../../aspose.tasks/project/print#print)() | Skriver ut projekt till standardskrivaren med standardskrivarinställningar med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Skriver ut projekt enligt de angivna skrivarinställningarna med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Skriver ut projekt till standardskrivaren med standardskrivarinställningar och anpassade sparalternativ med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Skriver ut projekt till den angivna skrivaren med standardskrivarinställningar med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Skriver ut projekt enligt de angivna skrivarinställningarna och anpassade sparalternativ med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Skriver ut projekt enligt de angivna skrivarinställningarna med standardutskriftskontrollern (utan användargränssnitt). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Skriver ut projekt enligt de angivna skrivarinställningarna, anpassade sparalternativ och det angivna dokumentnamnet med standardutskriftskontrollern (utan användargränssnitt). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Omschemalägger alla projektuppgifter-ID, dispositionsnivåer, start-/slutdatum, anger tidiga/sena datum, beräknar slacks, arbete och kostnadsfält. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Omschemalägger alla projektuppgifter-ID, dispositionsnivåer, start-/slutdatum, ställer in tidiga/sena datum, beräknar slack-, arbete- och kostnadsfält med valfri validering. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Beräknar om ID, start och slut på resurser. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Beräknar om start och mål för resurser. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Eliminerar ogiltiga resurstilldelningar från projektresurstilldelningslistan. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Numrera om WBS-koden för alla uppgifter. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Numrera om WBS-koden för godkända uppgifter. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Omschemalägger ofullbordat projektarbete för att starta efter ett angivet datum. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Omschemalägger ofullbordat arbete för en angiven lista med uppgifter för att starta efter ett angivet datum. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Sparar projektdata till filen i mpp-format. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Sparar projektet i en ström med de angivna sparalternativen. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Sparar projektdata i strömmen. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Sparar projektet i en ström med de angivna sparalternativen. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Sparar dokumentet till mpp-filformat med de angivna sparalternativen. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Sparar projektdata till filen. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Sparar dokumentet till en fil med de angivna sparalternativen. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Sparar projektet som en mall i en angiven ström. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Sparar projektet som en mall till den angivna sökvägen. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Sparar projektet som en mall i en angiven ström. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Sparar projektet som en mall. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Sparar projektöversiktsrapporten i strömmen. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Sparar projektöversiktsrapporten till PDF-fil. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Sparar projektrapporten av den angivna typen till den angivna strömmen. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Sparar projektrapporten av angiven typ i PDF-format till angiven filsökväg. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Samlar rekursivt alla underordnade uppgifter till rotuppgiften. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Sparar baslinjefält till angiven baslinje för hela projektet. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Sparar baslinjefält till angiven baslinje för de valda uppgifterna. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Ställer in baslinjespartiden. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Uppdaterar allt arbete som komplett till ett angivet datum för hela projektet. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Uppdaterar allt arbete som komplett till ett angivet datum för den angivna listan med uppgifter. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Hämtar projektfilinformation från strömmen. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Läs projektfilinformation från filen. |

### Anmärkningar

De **Projekt** är en central klass i Aspose.Tasks-biblioteket.

Man kan använda **Projekt** för att läsa ett av projekthanteringsformaten som stöds: MPP, MPT, MPX, XML.

För att ladda ett befintligt dokument i något av de format som stöds, skicka ett filnamn eller en ström till ett av de **Projekt** konstruktörer. För att skapa ett tomt projekt, anrop den parameterlösa konstruktorn.

Använd en av Spara-metodens överbelastningar för att spara projektet i någon av[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) format: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fast layout: PDF; Bilder: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Övrigt: HTML.

För att skriva ut projektet, använd en av de[`Print`](./print) metodöverbelastningar.

De **Projekt** lagrar projektövergripande information som t.ex[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , och[`ExtendedAttributes`](./extendedattributes) . De flesta av dessa objekt är tillgängliga via motsvarande egenskaper för **Projekt** klass.

De **Projekt** är en rotentitet som innehåller ingångspunkter för att manipulera andra projektenheter, som t.ex[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) och[`Calendar`](../calendar).

Den **Projekt** Entiteter kan till exempel nås via maskinskrivna samlingar[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , etc.

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
