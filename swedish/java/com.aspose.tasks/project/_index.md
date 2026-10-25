---
title: "Projekt"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett projekt."
type: docs
weight: 220
url: /sv/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Representerar ett projekt.

--------------------

Den **Project** är en central klass i Aspose.Tasks-biblioteket.

Man kan använda **Project** för att läsa ett av de stödda projektledningsformaten: MPP, MPT, MPX, XML.

För att läsa in ett befintligt dokument i något av de stödda formaten, skicka ett filnamn eller en ström till en av **Project**-konstruktörerna. För att skapa ett tomt projekt, anropa den parameterlösa konstruktören.

Använd en av Save‑metodens överlagringar för att spara projektet i något av [SaveFileFormat](../../com.aspose.tasks/savefileformat)-formaten: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fast layout: PDF; Bilder: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Övrigt: HTML.

För att skriva ut projektet, använd en av [print()](../../com.aspose.tasks/project\#print--) metodens överlagringar.

Den **Project** lagrar projektomfattande information såsom `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), och `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). De flesta av dessa objekt är åtkomliga via motsvarande egenskaper i **Project**-klassen.

Den **Project** är en rot‑entitet som innehåller ingångspunkter för att manipulera andra projekt‑entiteter, såsom [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) och [Calendar](../../com.aspose.tasks/calendar).

Projekt‑entiteterna **Project** kan nås via typade samlingar, till exempel `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), etc.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Project()](#Project--) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en lösenordsskyddad mall (existerande mpp‑ eller mpt‑fil). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från strömmen med den angivna instansen av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en ström. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande MPP‑ eller MPT‑fil) med den angivna instansen av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) för att läsa data från en databas som anges av instansen av klassen [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil) med den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från strömmen med den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returnerar värdet som egenskapen är mappad till i den här behållaren. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Kopierar projektets huvuddata och egenskaper till ett annat projekt. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Kopierar projektets huvuddata och egenskaper till ett annat projekt. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Enumererar rekursivt alla projektets uppgifter inklusive rotuppgift. |
| [getActualsInSync()](#getActualsInSync--) | Hämtar ett värde som indikerar om ActualsInSync är satt eller inte. |
| [getAdminProject()](#getAdminProject--) | Hämtar ett värde som indikerar om AdminProject är satt eller inte. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Hämtar ett värde som indikerar om AreEditableActualCosts är satt eller inte. |
| [getAuthor()](#getAuthor--) | Hämtar värdet för Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Hämtar ett värde som indikerar om AutoAddNewResourcesAndTasks är satt eller inte. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Hämtar om tilldelningskostnad och återstående kostnad ska beräknas automatiskt med hjälp av tilldelningens arbete och resurspriser. |
| [getAutolink()](#getAutolink--) | Hämtar ett värde som indikerar om Autolink är satt eller inte. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Hämtar värdet för BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Returnerar den sparade baslinjetiden. |
| [getBuiltInProps()](#getBuiltInProps--) | Hämtar projektets inbyggda egenskapskollektion. |
| [getCalculationMode()](#getCalculationMode--) | Hämtar beräkningsläget för ett projekt. |
| [getCalendar()](#getCalendar--) | Hämtar ett värde för Calendar. |
| [getCalendars()](#getCalendars--) | Hämtar [CalendarCollection](../../com.aspose.tasks/calendarcollection)-objektet för den här Projekt‑instansen. |
| [getCategory()](#getCategory--) | Hämtar ett värde för Kategori. |
| [getComments()](#getComments--) | Hämtar ett värde för Kommentarer. |
| [getCompany()](#getCompany--) | Hämtar ett värde för Företag. |
| [getCreationDate()](#getCreationDate--) | Hämtar ett värde för Skapandedatum. |
| [getCriticalPath()](#getCriticalPath--) | Hämtar en samling som innehåller en lista över kritiska uppgifter som utgör den kritiska vägen för detta projekt. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Uppgifter anses kritiska av MS Project om total marginal är mindre än eller lika med detta antal dagar. |
| [getCurrencyCode()](#getCurrencyCode--) | Hämtar ett värde för Valutakod. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Hämtar ett värde för Valutasiffror. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Hämtar ett värde för Valutasymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Hämtar ett värde för Valutasymbolens position. |
| [getCurrentDate()](#getCurrentDate--) | Hämtar ett värde för Aktuellt datum. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Hämtar ett värde för Anpassat datumformat. |
| [getCustomProps()](#getCustomProps--) | Hämtar projektets samling av anpassade egenskaper. |
| [getDateFormat()](#getDateFormat--) | Hämtar ett värde för Datumformat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Hämtar ett värde för Dagar per månad. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Hämtar ett värde för Standard sluttid. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Hämtar ett värde för Standard fast kostnadsackumulering. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Hämtar ett värde för Standard övertidsnivå. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Hämtar ett värde för Standard standardpris. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Hämtar ett värde för Standard starttid. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Hämtar ett värde för Standarduppgift‑EV‑metod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Hämtar ett värde för Standarduppgiftstyp. |
| [getDefaultView()](#getDefaultView--) | Hämtar standardvyn för projektet. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Hämtar instansen av klassen [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) som representerar en samling av projektets standardarbetsdagar och arbetstider för veckan. |
| [getDisplayOptions()](#getDisplayOptions--) | Hämtar en instans av klassen [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Hämtar [Duration](../../com.aspose.tasks/duration)-objektet med det angivna antalet enheter och standardformat för varaktighet som definieras i projektets inställningar [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Hämtar [Duration](../../com.aspose.tasks/duration)-objektet med det angivna antalet [TimeUnitType](../../com.aspose.tasks/timeunittype)-enheter. |
| [getDurationFormat()](#getDurationFormat--) | Hämtar ett värde för DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Hämtar ett värde för EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Hämtar ExtendedAttributeDefinitionCollection-objektet. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Hämtar ett värde för ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Hämtar ett värde för FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Hämtar ett värde som indikerar om FiscalYearStart är angivet eller inte. |
| [getFyStartDate()](#getFyStartDate--) | Hämtar ett värde för FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Hämtar globaliseringsinställningarna (språkspecifika) för projektet. |
| [getGuid()](#getGuid--) | Hämtar ett värde av Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Hämtar ett värde som indikerar om HonorConstraints är angivet eller inte. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Hämtar ett värde för HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Hämtar ett värde som indikerar om InsertedProjectsLikeSummary är angivet eller inte. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Hämtar ett värde som indikerar om KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled är angivet eller inte. |
| [getKeywords()](#getKeywords--) | Hämtar ett värde för Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Hämtar ett värde för LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Hämtar ett värde för LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Hämtar ett värde för LastSaved. |
| [getManager()](#getManager--) | Hämtar ett värde för Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Hämtar ett värde som indikerar om MicrosoftProjectServerURL är angivet eller inte. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Hämtar ett värde för MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Hämtar ett värde för MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Hämtar ett värde som indikerar om MoveCompletedEndsBack är angivet eller inte. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Hämtar ett värde som indikerar om MoveCompletedEndsForward är angivet eller inte. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Hämtar ett värde som indikerar om MoveRemainingStartsBack är inställt eller inte. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Hämtar ett värde som indikerar om MoveRemainingStartsForward är inställt eller inte. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Hämtar ett värde som indikerar om MultipleCriticalPaths är inställt eller inte. |
| [getName()](#getName--) | Hämtar ett värde av Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Hämtar värdet för NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Hämtar ett värde som indikerar om NewTasksAreManual är inställt eller inte. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Hämtar ett värde som indikerar om NewTasksEffortDriven är inställt eller inte. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Hämtar ett värde som indikerar om NewTasksEstimated är inställt eller inte. |
| [getOleObjects()](#getOleObjects--) | Hämtar en samling som innehåller instanser av klassen [OleObject](../../com.aspose.tasks/oleobject) som är länkade eller inbäddade i den här projektfilen. |
| [getOutlineCodes()](#getOutlineCodes--) | Hämtar OutlineCodeDefinitionCollection-objektet. |
| [getPageCount()](#getPageCount--) | Returnerar sidantalet för projektet som ska renderas med standard [Timescale](../../com.aspose.tasks/timescale) (Dagar). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Returnerar sidantalet för projektet som ska renderas med angivna [SaveOptions](../../com.aspose.tasks/saveoptions). |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Returnerar sidantalet för projektet som ska renderas med angiven [Timescale](../../com.aspose.tasks/timescale) och [PresentationFormat](../../com.aspose.tasks/presentationformat). |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Returnerar sidantalet för projektet som ska renderas med angiven [Timescale](../../com.aspose.tasks/timescale) och [PageSize](../../com.aspose.tasks/pagesize). |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Returnerar sidantalet för projektet som ska renderas med angiven [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) och datumintervall. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Returnerar sidantalet för projektet som ska renderas med standard [Timescale](../../com.aspose.tasks/timescale) (Dagar) och angiven [PresentationFormat](../../com.aspose.tasks/presentationformat) |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Returnerar sidantalet för projektet som ska renderas med angiven [Timescale](../../com.aspose.tasks/timescale). |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Returnerar en samling av uppgiftslänkar som är föregångare till den angivna uppgiften. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Hämtar ett objekt som innehåller Primavera-specifika egenskaper för ett projekt läst från en Primavera-fil. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Hämtar ett värde som indikerar om ProjectExternallyEdited är inställt eller inte. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Hämtar projektfilens information från strömmen. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Läs projektfilens information från filen. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Hämtar ett värde som indikerar om RemoveFileProperties är inställt eller inte. |
| [getResourceAssignments()](#getResourceAssignments--) | Hämtar ResourceAssignmentCollection-objektet. |
| [getResourceFilters()](#getResourceFilters--) | Hämtar alla resursbaserade filterdefinitioner. |
| [getResourceGroups()](#getResourceGroups--) | Hämtar alla resursbaserade gruppdefinitioner. |
| [getResources()](#getResources--) | Hämtar ResourceCollection-objektet. |
| [getRevision()](#getRevision--) | Hämtar ett värde för Revision. |
| [getRootTask()](#getRootTask--) | Hämtar roten av trädstrukturen för uppgifter. |
| [getSaveVersion()](#getSaveVersion--) | Hämtar ett värde för SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Hämtar ett värde som indikerar om ScheduleFromStart är satt eller inte. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Hämtar ett värde som indikerar om ShowProjectSummaryTask är satt eller inte. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Hämtar ett värde som indikerar om SplitsInProgressTasks är satt eller inte. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Hämtar ett värde som indikerar om SpreadActualCost är satt eller inte. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Hämtar ett värde som indikerar om SpreadPercentComplete är satt eller inte. |
| [getStartDate()](#getStartDate--) | Hämtar ett värde för StartDate. |
| [getStatusDate()](#getStatusDate--) | Hämtar ett värde för StatusDate. |
| [getSubject()](#getSubject--) | Hämtar ett värde för Subject. |
| [getTables()](#getTables--) | Hämtar en lista med [Table](../../com.aspose.tasks/table)-objekt. |
| [getTaskFilters()](#getTaskFilters--) | Hämtar alla uppgiftsbaserade filterdefinitioner. |
| [getTaskGroups()](#getTaskGroups--) | Hämtar alla uppgiftsbaserade gruppdefinitioner. |
| [getTaskLinks()](#getTaskLinks--) | Hämtar [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection)-objektet. |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Hämtar ett värde som indikerar om TaskUpdatesResource är satt eller inte. |
| [getTemplate()](#getTemplate--) | Hämtar ett värde för Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Hämtar ett värde för TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Hämtar ett värde för TimescaleStart. |
| [getTitle()](#getTitle--) | Hämtar ett värde för Title. |
| [getUid()](#getUid--) | Hämtar ett värde för Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Hämtar ett värde som indikerar om UpdateManuallyScheduledTasksWhenEditingLinks är satt eller inte. |
| [getVbaProject()](#getVbaProject--) | Hämtar en instans av `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-))-klassen. |
| [getViews()](#getViews--) | Hämtar en lista med [View](../../com.aspose.tasks/view)-objekt. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Hämtar WBS Code Definition för projektet. |
| [getWeekStartDay()](#getWeekStartDay--) | Hämtar ett värde för WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Hämtar [Duration](../../com.aspose.tasks/duration)-objektet med det angivna `double`-värdet och standardarbetsformatet. |
| [getWorkFormat()](#getWorkFormat--) | Hämtar ett värde för WorkFormat. |
| [print()](#print--) | Skriver ut projektet till standardskrivaren med standardinställningar för skrivaren med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Skriver ut projektet till standardskrivaren med standardinställningar för skrivaren och anpassade sparaalternativ med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Skriver ut projektet enligt de angivna skrivarinställningarna med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Skriver ut projektet enligt de angivna skrivarinställningarna och anpassade sparaalternativ med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Skriver ut projektet enligt de angivna skrivarinställningarna, anpassade sparaalternativ och det angivna dokumentnamnet med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Skriver ut projektet enligt de angivna skrivarinställningarna med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [print(String printerName)](#print-java.lang.String-) | Skriver ut projektet till den angivna skrivaren med standardinställningar för skrivaren med hjälp av den standard (utan användargränssnitt) utskriftskontrollen. |
| [recalculate()](#recalculate--) | Omplanerar alla projektuppgifts‑id:n, outline‑nivåer, start-/slutdatum, sätter tidiga/sena datum, beräknar slack, arbete och kostnadsfält. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Omplanerar alla projektuppgifts‑id:n, outline‑nivåer, start-/slutdatum, sätter tidiga/sena datum, beräknar slack, arbete och kostnadsfält med valfri validering. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Beräknar om Id, Start och Finish för resurser. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Beräknar om Start och Finish för resurser. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Eliminerar ogiltiga resursallokeringar från projektets lista över resursallokeringar. |
| [renumberWBSCode()](#renumberWBSCode--) | Numrerar om WBS‑koden för alla uppgifter. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Numrerar om WBS‑koden för de angivna uppgifterna. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Omplanerar ofullständigt projektarbete så att det startar efter ett angivet datum. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Omplanerar ofullständigt arbete för en angiven lista av uppgifter så att det startar efter ett angivet datum. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Sparar projektet till en ström med de angivna sparaalternativen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Sparar projektdata till strömmen. |
| [save(String filename)](#save-java.lang.String-) | Sparar projektdata till filen i mpp-format. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Sparar dokumentet till en fil med de angivna sparaalternativen. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Sparar projektdata till filen. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Sparar projektet som en mall till en angiven ström. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Sparar projektet som en mall till en angiven ström. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Sparar projektet som en mall till den angivna filsökvägen. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Sparar projektet som en mall. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Sparar projektöversiktsrapporten till strömmen. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Sparar projektrapporten av den angivna typen till den angivna strömmen. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Sparar projektöversiktsrapporten till en PDF-fil. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Sparar projektrapporten av den angivna typen i PDF-format till den angivna filsökvägen. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Samlar rekursivt in alla underuppgifter till rotuppgiften. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Ställer in ett värde som indikerar om ActualsInSync är satt eller inte. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Ställer in ett värde som indikerar om AdminProject är satt eller inte. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Ställer in ett värde som indikerar om AreEditableActualCosts är satt eller inte. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in ett värde för Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Ställer in ett värde som indikerar om AutoAddNewResourcesAndTasks är satt eller inte. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Ställer in om uppdragskostnad och återstående kostnad ska beräknas automatiskt med hjälp av uppdragets arbete och resursers satser. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Ställer in ett värde som indikerar om Autolink är satt eller inte. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Sparar baslinjefält till den angivna baslinjen för hela projektet. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Sparar baslinjefält till den angivna baslinjen för de markerade uppgifterna. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Ställer in ett värde för BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Ställer in baslinjesparningstiden. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Ställer in beräkningsläget för ett projekt. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Sätter ett värde för Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Ställer in ett värde för Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Ställer in ett värde för Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Ställer in ett värde för Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Ställer in ett värde för CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Uppgifter anses kritiska av MS Project om total marginal är mindre än eller lika med detta antal dagar. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Ställer in ett värde för CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Ställer in ett värde för CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Ställer in ett värde för CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Ställer in ett värde för CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Ställer in ett värde för CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Ställer in ett värde för CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Ställer in ett värde för DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Ställer in ett värde för DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Ställer in ett värde för DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Ställer in ett värde för DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Ställer in ett värde för DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Ställer in ett värde för DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Ställer in ett värde för DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Ställer in ett värde för DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Ställer in ett värde för DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Ställer in standardvyn för projektet. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Ställer in ett värde för DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Ställer in ett värde för EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Ställer in ett värde för ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Ställer in ett värde för FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om FiscalYearStart är angivet eller inte. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Ställer in ett värde för FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Ställer in globaliseringsinställningar (språkspecifika) för projektet. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Sätter ett värde för Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om HonorConstraints är angivet eller inte. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Ställer in ett värde för HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om InsertedProjectsLikeSummary är angivet eller inte. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled är angivet eller inte. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Ställer in ett värde för Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Ställer in ett värde för LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Ställer in ett värde för LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Ställer in ett värde för LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Ställer in ett värde för Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MicrosoftProjectServerURL är inställt eller inte. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Ställer in ett värde för MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Ställer in ett värde för MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MoveCompletedEndsBack är inställt eller inte. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MoveCompletedEndsForward är inställt eller inte. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MoveRemainingStartsBack är inställt eller inte. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MoveRemainingStartsForward är inställt eller inte. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om MultipleCriticalPaths är inställt eller inte. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in ett värde för Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Ställer in ett värde för NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om NewTasksAreManual är inställt eller inte. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om NewTasksEffortDriven är inställt eller inte. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om NewTasksEstimated är inställt eller inte. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om ProjectExternallyEdited är inställt eller inte. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om RemoveFileProperties är inställt eller inte. |
| [setRevision(int value)](#setRevision-int-) | Ställer in ett värde för Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Ställer in ett värde för SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om ScheduleFromStart är inställt eller inte. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Ställer in ett värde som anger om ShowProjectSummaryTask är inställt eller inte. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om SplitsInProgressTasks är inställt eller inte. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om SpreadActualCost är inställt eller inte. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om SpreadPercentComplete är inställt eller inte. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Sätter ett värde för StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Sätter ett värde för StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Sätter ett värde för Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om TaskUpdatesResource är satt eller inte. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Sätter ett värde för Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Sätter ett värde för TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Sätter ett värde för TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Sätter ett värde för Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Ställer in ett värde för Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om UpdateManuallyScheduledTasksWhenEditingLinks är satt eller inte. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Sätter WBS Code Definition för projektet. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Sätter ett värde för WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Sätter ett värde för WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Uppdaterar allt arbete som slutfört fram till ett angivet datum för hela projektet. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Uppdaterar allt arbete som slutfört fram till ett angivet datum för den angivna listan med uppgifter. |
### Project() {#Project--}
```
public Project()
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en lösenordsskyddad mall (existerande mpp‑ eller mpt‑fil).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectTemplate | java.lang.String | Sökväg till mall att skapa projekt från. |
|  | protectionPassword | java.lang.String | Skyddslösenord. |

--------------------

Läsning av lösenordsskyddade filer stöds för närvarande endast för MSP 2003-filformatet. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectTemplate | java.lang.String | Sökväg till mall att skapa projekt från. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från strömmen med den angivna instansen av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Ström av projektet java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | den specificerade instansen av [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)class som möjliggör anpassning av läsning av Primavera-format (XER eller XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectTemplate | java.lang.String | Sökväg till mall att skapa projekt från. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | den specificerade återuppringningsmetoden för att hantera xml-parsningsfel. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream för att läsa in en mall från. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande MPP‑ eller MPT‑fil) med den angivna instansen av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectTemplate | java.lang.String | Sökväg till mall för att skapa projekt från |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | den angivna instansen av klassen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) för att läsa data från en databas som anges av instansen av klassen [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | den angivna instansen av klassen [DbSettings](../../com.aspose.tasks/dbsettings). |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream för att läsa in en mall från. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | den specificerade återuppringningsmetoden för att hantera xml-parsningsfel. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream för att läsa in en mall från. |
|  | protectionPassword | java.lang.String | Skyddslösenord. |

--------------------

Läsning av lösenordsskyddade filer stöds för närvarande endast för MSP 2003-filformatet. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från en mall (existerande mpp‑ eller mpt‑fil) med den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectTemplate | java.lang.String | Sökväg till mall för att skapa projekt från |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions). |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Initierar en ny instans av klassen [Project](../../com.aspose.tasks/project) från strömmen med den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Ström av projektet java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | den angivna instansen av klassen [LoadOptions](../../com.aspose.tasks/loadoptions)klass |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returnerar värdet som egenskapen är mappad till i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Prj](../../com.aspose.tasks/prj) för att hämta egenskapsnyckeln. |

**Returns:**
T - värdet som egenskapen är mappad till i denna behållare.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappar den angivna egenskapen till det angivna värdet i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Prj](../../com.aspose.tasks/prj) för att hämta egenskapsnyckeln. |
| val | T | värdet. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Kopierar projektets huvuddata och egenskaper till ett annat projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Ett annat projekt att kopiera data till. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Kopierar projektets huvuddata och egenskaper till ett annat projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Ett annat projekt att kopiera data till. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Kopieringsalternativ för att styra kopieringsprocessen. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Enumererar rekursivt alla projektets uppgifter inklusive rotuppgift.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable som kan användas för att iterera över alla projektets uppgifter.

--------------------

Tillhandahåller ett mer lättviktigt sätt att iterera över uppgifter jämfört med metoden [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) eftersom den inte allokerar minne för alla uppgifter.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Hämtar ett värde som indikerar om ActualsInSync är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Hämtar ett värde som indikerar om AdminProject är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Hämtar ett värde som indikerar om AreEditableActualCosts är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Hämtar värdet för Author.

**Returns:**
java.lang.String - ett värde för Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Hämtar ett värde som indikerar om AutoAddNewResourcesAndTasks är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Hämtar om tilldelningskostnad och återstående kostnad ska beräknas automatiskt med hjälp av tilldelningens arbete och resurspriser.

**Returns:**
boolean - huruvida tilldelningskostnad och återstående kostnad ska beräknas automatiskt med hjälp av tilldelningens arbete och resurspriser.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Hämtar ett värde som indikerar om Autolink är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Hämtar värdet för BaselineForEarnedValue.

**Returns:**
int - ett värde för BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Returnerar tidpunkten för baslinjens sparning. Returnerar DateTime.MinValue (00:00:00.0000000 UTC, 1 januari 0001) om baslinjen inte sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baselineNumber | int | Baslinjens nummer [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - Baslinjens senaste sparningsdatum och tid.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Hämtar projektets inbyggda egenskapskollektion.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Hämtar beräkningsläge för ett projekt. Kan vara ett av värdena i `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-))‑enumerationen.

**Returns:**
int - beräkningsläge för ett projekt.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Hämtar ett värde för Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Hämtar [CalendarCollection](../../com.aspose.tasks/calendarcollection)-objektet för den här Projekt‑instansen.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Hämtar ett värde för Kategori.

**Returns:**
java.lang.String - ett värde för Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Hämtar ett värde för Kommentarer.

**Returns:**
java.lang.String - ett värde för Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Hämtar ett värde för Företag.

**Returns:**
java.lang.String - ett värde för Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Hämtar ett värde för Skapandedatum.

**Returns:**
java.util.Date - ett värde för CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Hämtar en samling som innehåller en lista över kritiska uppgifter som utgör den kritiska vägen för detta projekt.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Detta är en O(n)-operation, där n är antalet uppgifter i projektet.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Uppgifter anses kritiska av MS Project om total marginal är mindre än eller lika med detta antal dagar.

**Returns:**
int - det maximala värdet för total slacktid (i dagar) vid vilket en uppgift anses kritisk
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Hämtar ett värde för Valutakod.

**Returns:**
java.lang.String - ett värde för CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Hämtar ett värde för Valutasiffror.

**Returns:**
int - ett värde av CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Hämtar ett värde för Valutasymbol.

**Returns:**
java.lang.String - ett värde av CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Hämtar ett värde för Valutasymbolens position.

**Returns:**
int - ett värde av CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Hämtar ett värde för Aktuellt datum.

**Returns:**
java.util.Date - ett värde av CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Hämtar ett värde för Anpassat datumformat.

**Returns:**
java.lang.String - ett värde av CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Hämtar projektets samling av anpassade egenskaper.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Hämtar ett värde för Datumformat.

**Returns:**
int - ett värde av DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Hämtar ett värde för Dagar per månad.

**Returns:**
int - ett värde av DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Hämtar ett värde för Standard sluttid.

**Returns:**
java.util.Date - ett värde av DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Hämtar ett värde för Standard fast kostnadsackumulering.

**Returns:**
int - ett värde av DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Hämtar ett värde för Standard övertidsnivå.

**Returns:**
double - ett värde av DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Hämtar ett värde för Standard standardpris.

**Returns:**
double - ett värde av DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Hämtar ett värde för Standard starttid.

**Returns:**
java.util.Date - ett värde av DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Hämtar ett värde för Standarduppgift‑EV‑metod.

**Returns:**
int - ett värde av DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Hämtar ett värde för Standarduppgiftstyp.

**Returns:**
int - ett värde av DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Hämtar standardvyn för projektet.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Hämtar instansen av klassen [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) som representerar en samling av projektets standardarbetsdagar och arbetstider för veckan.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Data finns endast i mpp-filer (inte i xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Hämtar en instans av klassen [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Hämtar [Duration](../../com.aspose.tasks/duration)-objektet med det angivna antalet enheter och standardformat för varaktighet som definieras i projektets inställningar [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | val | double | specificerat antal enheter. |

--------------------

Denna metod bör användas försiktigt eftersom den returnerar olika varaktigheter beroende på inställningen Project.DurationFormat. Till exempel kommer GetWork(1.0) att returnera 1 timme när Project.DurationFormat är TimeUnitType.Hour eller 1 dag om Project.DurationFormat är TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Hämtar [Duration](../../com.aspose.tasks/duration)-objektet med det angivna antalet [TimeUnitType](../../com.aspose.tasks/timeunittype)-enheter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| val | double | specificerat antal enheter. |
| tidsenhet | byte | specificerat TimeUnitType-värde. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Hämtar ett värde för DurationFormat.

**Returns:**
byte - ett värde av DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Hämtar ett värde för EarnedValueMethod.

**Returns:**
int - ett värde av EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Hämtar ExtendedAttributeDefinitionCollection-objektet. Samlingen av definitioner för utökade attribut (anpassade fält) som är associerade med ett projekt.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Hämtar ett värde för ExtendedCreationDate.

**Returns:**
java.util.Date - ett värde av ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Hämtar ett värde för FinishDate.

**Returns:**
java.util.Date - ett värde av FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Hämtar ett värde som indikerar om FiscalYearStart är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Hämtar ett värde för FyStartDate.

**Returns:**
int - ett värde av FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Hämtar globaliseringsinställningarna (språkspecifika) för projektet.

Det rekommenderade sättet är att använda kultur‑oberoende litteraler eller format genom hela projektet. Men om ett projekt använder kulturspecifika litteraler kan den här klassen användas för att hjälpa beräkningsmotorn att tolka dessa litteraler.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Hämtar ett värde av Guid.

**Returns:**
java.util.UUID - ett värde av Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Hämtar ett värde som indikerar om HonorConstraints är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Hämtar ett värde för HyperlinkBase.

**Returns:**
java.lang.String - ett värde av HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Hämtar ett värde som indikerar om InsertedProjectsLikeSummary är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Hämtar ett värde som indikerar om KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Hämtar ett värde för Keywords.

**Returns:**
java.lang.String - ett värde av Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Hämtar ett värde för LastAuthor.

**Returns:**
java.lang.String - ett värde av LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Hämtar ett värde för LastPrinted.

**Returns:**
java.util.Date - ett värde av LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Hämtar ett värde för LastSaved.

**Returns:**
java.util.Date - ett värde av LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Hämtar ett värde för Manager.

**Returns:**
java.lang.String - ett värde av Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Hämtar ett värde som indikerar om MicrosoftProjectServerURL är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Hämtar ett värde för MinutesPerDay.

**Returns:**
int - ett värde av MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Hämtar ett värde för MinutesPerWeek.

**Returns:**
int - ett värde av MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Hämtar ett värde som indikerar om MoveCompletedEndsBack är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Hämtar ett värde som indikerar om MoveCompletedEndsForward är angivet eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Hämtar ett värde som indikerar om MoveRemainingStartsBack är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Hämtar ett värde som indikerar om MoveRemainingStartsForward är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Hämtar ett värde som indikerar om MultipleCriticalPaths är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Hämtar ett värde av Name.

**Returns:**
java.lang.String - ett värde av Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Hämtar värdet för NewTaskStartDate.

**Returns:**
int - ett värde av NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Hämtar ett värde som indikerar om NewTasksAreManual är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Hämtar ett värde som indikerar om NewTasksEffortDriven är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Hämtar ett värde som indikerar om NewTasksEstimated är inställt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Hämtar en samling som innehåller instanser av klassen [OleObject](../../com.aspose.tasks/oleobject) som är länkade eller inbäddade i den här projektfilen.

--------------------

Tillgänglig endast för mpp‑filformat. Denna samling är skrivskyddad förutom för 'Clear'-operationen.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Hämtar OutlineCodeDefinitionCollection‑objektet. Samlingen av konturkoddefinitioner som är associerade med ett projekt.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Returnerar sidantalet för projektet som ska renderas med standard [Timescale](../../com.aspose.tasks/timescale) (Dagar).

**Returns:**
int - Sidantal att renderas.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Returnerar sidantalet för projektet som ska renderas med angivna [SaveOptions](../../com.aspose.tasks/saveoptions).

--------------------

&gt; ```
&gt; I det här exemplet skrivs instansen av HtmlSaveOptions och antalet sidor i den resulterande HTML:n till konsolen.
&gt; ``````

  [C#]
Project project = new Project(@\"test.mpp\");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
public final int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
public final NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
public final boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
public final NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
public final NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
public final NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
public final Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
public final String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
public final NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
public final String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
public final Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
public final Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
public final String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
public final String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
public final NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
public final int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

