---
title: "Project"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Geeft een project weer."
type: docs
weight: 220
url: /nl/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Geeft een project weer.

--------------------

De **Project** is een centrale klasse in de Aspose.Tasks bibliotheek.

Men kan **Project** gebruiken om een van de ondersteunde projectmanagementformaten te lezen: MPP, MPT, MPX, XML.

Om een bestaand document in een van de ondersteunde formaten te laden, geef een bestandsnaam of een stream door aan een van de **Project**-constructors. Om een leeg project te maken, roep de parameterloze constructor aan.

Gebruik een van de overloads van de Save-methode om het project op te slaan in een van de [SaveFileFormat](../../com.aspose.tasks/savefileformat)-formaten: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Vaste lay-out: PDF; Afbeeldingen: JPEG, PNG, BMP, TIFF, SVG; Tekst: TXT; Overige: HTML.

Om het project af te drukken, gebruik een van de overloads van de [print()](../../com.aspose.tasks/project\#print--) methode.

De **Project** slaat projectbrede informatie op, zoals `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), en `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). De meeste van deze objecten zijn toegankelijk via de overeenkomstige eigenschappen van de **Project**-klasse.

De **Project** is een root‑entity die toegangspunten bevat om andere project‑entiteiten te manipuleren, zoals [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) en [Calendar](../../com.aspose.tasks/calendar).

De **Project**-entity's kunnen worden benaderd via getypeerde collecties, bijvoorbeeld `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), enz.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Project()](#Project--) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een met wachtwoord beveiligde sjabloon (bestaand mpp- of mpt‑bestand). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit de Stream met de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-klasse. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een stream. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand MPP‑ of MPT‑bestand) met de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-klasse. |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse om gegevens te lezen uit een database die wordt gespecificeerd door het exemplaar van de [DbSettings](../../com.aspose.tasks/dbsettings) klasse. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand) met het gespecificeerde exemplaar van de [LoadOptions](../../com.aspose.tasks/loadoptions) klasse. |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit de Stream met het gespecificeerde exemplaar van de [LoadOptions](../../com.aspose.tasks/loadoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Somt recursief alle taken van het project op, inclusief de hoofdtaak. |
| [getActualsInSync()](#getActualsInSync--) | Haalt een waarde op die aangeeft of ActualsInSync is ingesteld of niet. |
| [getAdminProject()](#getAdminProject--) | Haalt een waarde op die aangeeft of AdminProject is ingesteld of niet. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Haalt een waarde op die aangeeft of AreEditableActualCosts is ingesteld of niet. |
| [getAuthor()](#getAuthor--) | Haalt de waarde van Author op. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Haalt een waarde op die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Haalt op of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk en de tarief van de toewijzing. |
| [getAutolink()](#getAutolink--) | Haalt een waarde op die aangeeft of Autolink is ingesteld of niet. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Haalt de waarde van BaselineForEarnedValue op. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Retourneert de tijd waarop de basislijn is opgeslagen. |
| [getBuiltInProps()](#getBuiltInProps--) | Haalt de verzameling ingebouwde eigenschappen van het project op. |
| [getCalculationMode()](#getCalculationMode--) | Haalt de berekeningsmodus van een project op. |
| [getCalendar()](#getCalendar--) | Haalt een waarde van Calendar op. |
| [getCalendars()](#getCalendars--) | Haalt het [CalendarCollection](../../com.aspose.tasks/calendarcollection) object op van dit Project‑exemplaar. |
| [getCategory()](#getCategory--) | Haalt de waarde van Category op. |
| [getComments()](#getComments--) | Haalt de waarde van Comments op. |
| [getCompany()](#getCompany--) | Haalt de waarde van Company op. |
| [getCreationDate()](#getCreationDate--) | Haalt de waarde van CreationDate op. |
| [getCriticalPath()](#getCriticalPath--) | Haalt een verzameling op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Taken worden door MS Project als kritisch beschouwd als de totale speling minder dan of gelijk aan dit aantal dagen is. |
| [getCurrencyCode()](#getCurrencyCode--) | Haalt de waarde van CurrencyCode op. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Haalt een waarde op van CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Haalt een waarde op van CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Haalt een waarde op van CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Haalt een waarde op van CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Haalt een waarde op van CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Haalt de collectie met aangepaste projecteigenschappen op. |
| [getDateFormat()](#getDateFormat--) | Haalt een waarde op van DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Haalt een waarde op van DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Haalt een waarde op van DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Haalt een waarde op van DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Haalt een waarde op van DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Haalt een waarde op van DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Haalt een waarde op van DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Haalt een waarde op van DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Haalt een waarde op van DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Haalt de standaardweergave van het project op. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Haalt de instantie van de klasse [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) op, die een collectie van de standaardwerkdagen en werktijden van het project vertegenwoordigt. |
| [getDisplayOptions()](#getDisplayOptions--) | Haalt een instantie van de klasse [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) op. |
| [getDuration(double val)](#getDuration-double-) | Haalt een [Duration](../../com.aspose.tasks/duration)-object op met het opgegeven aantal eenheden en het standaardduurtijdformaat dat is gedefinieerd in de projectinstellingen [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Haalt een [Duration](../../com.aspose.tasks/duration)-object op met het opgegeven aantal [TimeUnitType](../../com.aspose.tasks/timeunittype)-eenheden. |
| [getDurationFormat()](#getDurationFormat--) | Haalt een waarde op van DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Haalt een waarde op van EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Haalt een ExtendedAttributeDefinitionCollection-object op. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Haalt een waarde op van ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Haalt een waarde op van FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Haalt een waarde op die aangeeft of FiscalYearStart is ingesteld of niet. |
| [getFyStartDate()](#getFyStartDate--) | Haalt een waarde op van FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Haalt globalisatie (taalspecifieke) instellingen van het project op. |
| [getGuid()](#getGuid--) | Haalt een waarde van Guid op. |
| [getHonorConstraints()](#getHonorConstraints--) | Haalt een waarde op die aangeeft of HonorConstraints is ingesteld of niet. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Haalt een waarde op van HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Haalt een waarde op die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Haalt een waarde op die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet. |
| [getKeywords()](#getKeywords--) | Haalt een waarde op van Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Haalt een waarde op van LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Haalt een waarde op van LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Haalt een waarde op van LastSaved. |
| [getManager()](#getManager--) | Haalt een waarde op van Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Haalt een waarde op die aangeeft of MicrosoftProjectServerURL is ingesteld of niet. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Haalt een waarde op van MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Haalt een waarde op van MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Haalt een waarde op die aangeeft of MoveCompletedEndsBack is ingesteld of niet. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Haalt een waarde op die aangeeft of MoveCompletedEndsForward is ingesteld of niet. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Haalt een waarde op die aangeeft of MoveRemainingStartsBack is ingesteld of niet. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Haalt een waarde op die aangeeft of MoveRemainingStartsForward is ingesteld of niet. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Haalt een waarde op die aangeeft of MultipleCriticalPaths is ingesteld of niet. |
| [getName()](#getName--) | Haalt een waarde van Name op. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Haalt een waarde op van NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Haalt een waarde op die aangeeft of NewTasksAreManual is ingesteld of niet. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Haalt een waarde op die aangeeft of NewTasksEffortDriven is ingesteld of niet. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Haalt een waarde op die aangeeft of NewTasksEstimated is ingesteld of niet. |
| [getOleObjects()](#getOleObjects--) | Haalt een collectie op die de instanties van de [OleObject](../../com.aspose.tasks/oleobject) klasse bevat die gekoppeld of ingesloten zijn in dit projectbestand. |
| [getOutlineCodes()](#getOutlineCodes--) | Haalt OutlineCodeDefinitionCollection-object op. |
| [getPageCount()](#getPageCount--) | Retourneert paginatelling voor het project dat wordt gerenderd met de standaard [Timescale](../../com.aspose.tasks/timescale)(Dagen). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [SaveOptions](../../com.aspose.tasks/saveoptions). |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [Timescale](../../com.aspose.tasks/timescale) en [PresentationFormat](../../com.aspose.tasks/presentationformat). |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [Timescale](../../com.aspose.tasks/timescale) en [PageSize](../../com.aspose.tasks/pagesize). |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) en datumbereik. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Retourneert paginatelling voor het project dat wordt gerenderd met de standaard [Timescale](../../com.aspose.tasks/timescale)(Dagen) en de opgegeven [PresentationFormat](../../com.aspose.tasks/presentationformat) |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [Timescale](../../com.aspose.tasks/timescale). |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Retourneert een verzameling taakkoppelingen die voorgangers zijn van de opgegeven taak. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Haalt een object op dat Primavera-specifieke eigenschappen bevat voor een project dat is gelezen uit een Primavera-bestand. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Haalt een waarde op die aangeeft of ProjectExternallyEdited is ingesteld of niet. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Haalt projectbestandsinformatie op uit de stream. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Lees projectbestandsinformatie uit het bestand. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Haalt een waarde op die aangeeft of RemoveFileProperties is ingesteld of niet. |
| [getResourceAssignments()](#getResourceAssignments--) | Haalt ResourceAssignmentCollection-object op. |
| [getResourceFilters()](#getResourceFilters--) | Haalt alle op resources gebaseerde filterdefinities op. |
| [getResourceGroups()](#getResourceGroups--) | Haalt alle op resources gebaseerde groepsdefinities op. |
| [getResources()](#getResources--) | Haalt ResourceCollection-object op. |
| [getRevision()](#getRevision--) | Haalt een waarde van Revision op. |
| [getRootTask()](#getRootTask--) | Haalt de wortel van de taakboom op. |
| [getSaveVersion()](#getSaveVersion--) | Haalt een waarde van SaveVersion op. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Haalt een waarde op die aangeeft of ScheduleFromStart is ingesteld of niet. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Haalt een waarde op die aangeeft of ShowProjectSummaryTask is ingesteld of niet. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Haalt een waarde op die aangeeft of SplitsInProgressTasks is ingesteld of niet. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Haalt een waarde op die aangeeft of SpreadActualCost is ingesteld of niet. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Haalt een waarde op die aangeeft of SpreadPercentComplete is ingesteld of niet. |
| [getStartDate()](#getStartDate--) | Haalt een waarde van StartDate op. |
| [getStatusDate()](#getStatusDate--) | Haalt een waarde van StatusDate op. |
| [getSubject()](#getSubject--) | Haalt een waarde van Subject op. |
| [getTables()](#getTables--) | Haalt een lijst met [Table](../../com.aspose.tasks/table) objecten op. |
| [getTaskFilters()](#getTaskFilters--) | Haalt alle taakgebaseerde filterdefinities op. |
| [getTaskGroups()](#getTaskGroups--) | Haalt alle taakgebaseerde groepsdefinities op. |
| [getTaskLinks()](#getTaskLinks--) | Haalt een [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object op. |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Haalt een waarde op die aangeeft of TaskUpdatesResource is ingesteld of niet. |
| [getTemplate()](#getTemplate--) | Haalt een waarde van Template op. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Haalt een waarde van TimescaleFinish op. |
| [getTimescaleStart()](#getTimescaleStart--) | Haalt een waarde van TimescaleStart op. |
| [getTitle()](#getTitle--) | Haalt een waarde van Title op. |
| [getUid()](#getUid--) | Haalt een waarde op van Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Haalt een waarde op die aangeeft of UpdateManuallyScheduledTasksWhenEditingLinks is ingesteld of niet. |
| [getVbaProject()](#getVbaProject--) | Haalt een instantie van `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) klasse op. |
| [getViews()](#getViews--) | Haalt een lijst met [View](../../com.aspose.tasks/view) objecten op. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Haalt WBS Code Definition voor het project op. |
| [getWeekStartDay()](#getWeekStartDay--) | Haalt een waarde van WeekStartDay op. |
| [getWork(double val)](#getWork-double-) | Haalt een [Duration](../../com.aspose.tasks/duration) object op met de opgegeven `double` waarde en standaard werkformaat. |
| [getWorkFormat()](#getWorkFormat--) | Haalt een waarde van WorkFormat op. |
| [print()](#print--) | Print het project naar de standaardprinter met standaard printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Print het project naar de standaardprinter met standaard printerinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Print het project volgens de opgegeven printerinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Print het project volgens de opgegeven printerinstellingen, aangepaste opslagopties en de opgegeven documentnaam met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [print(String printerName)](#print-java.lang.String-) | Print het project naar de opgegeven printer met standaard printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [recalculate()](#recalculate--) | Plant alle projecttaak‑ID's, outline‑niveaus, start-/einddatums opnieuw in, stelt vroege/late datums in, berekent speling, werk- en kostengegevens. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Plant alle projecttaak‑ID's, outline‑niveaus, start-/einddatums opnieuw in, stelt vroege/late datums in, berekent speling, werk- en kostengegevens met optionele validatie. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Herberekent ID, start en eind van resources. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Herberekent start en eind van resources. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Verwijdert ongeldige resource‑toewijzingen uit de lijst met projectresource‑toewijzingen. |
| [renumberWBSCode()](#renumberWBSCode--) | Hernummer WBS‑code van alle taken. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Hernummer WBS‑code van doorgegeven taken. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Plant onvoltooide projectwerkzaamheden opnieuw in om te starten na een opgegeven datum. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Plant onvoltooide werkzaamheden voor een opgegeven takenlijst opnieuw in om te starten na een opgegeven datum. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Slaat het project op in een stream met de opgegeven opslagopties. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Slaat de projectgegevens op in de stream. |
| [save(String filename)](#save-java.lang.String-) | Slaat de projectgegevens op in het bestand in mpp‑formaat. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Slaat het document op in een bestand met de opgegeven opslagopties. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Slaat de projectgegevens op in het bestand. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Slaat het project op als sjabloon in een opgegeven stream. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Slaat het project op als sjabloon in een opgegeven stream. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Slaat het project op als sjabloon op het opgegeven bestandspad. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Slaat het project op als sjabloon. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Slaat het projectoverzichtsrapport op in de stream. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Slaat het projectrapport van het opgegeven type op in de opgegeven stream. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Slaat het projectoverzichtsrapport op in een PDF‑bestand. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Slaat het projectrapport van het opgegeven type in PDF‑formaat op naar het opgegeven bestandspad. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Verzamelt recursief alle onderliggende taken van de hoofdtaak. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of ActualsInSync is ingesteld of niet. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of AdminProject is ingesteld of niet. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of AreEditableActualCosts is ingesteld of niet. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Stelt een waarde in voor Auteur. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Stelt in of toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk van de toewijzing en de tarieven van de resource. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of Autolink is ingesteld of niet. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Slaat basislijnvelden op naar de opgegeven basislijn voor het gehele project. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Slaat basislijnvelden op naar de opgegeven basislijn voor de geselecteerde taken. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Stelt een waarde in voor BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Stelt de tijd voor het opslaan van de basislijn in. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Stelt de berekeningsmodus van een project in. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Stelt een waarde in voor Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Stelt een waarde in voor Categorie. |
| [setComments(String value)](#setComments-java.lang.String-) | Stelt een waarde in voor Opmerkingen. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Stelt een waarde in voor Bedrijf. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Stelt een waarde in voor Aanmaakdatum. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Taken worden door MS Project als kritisch beschouwd als de totale speling minder dan of gelijk aan dit aantal dagen is. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Stelt een waarde in voor Valutacode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Stelt een waarde in voor ValutaDecimalen. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Stelt een waarde in voor Valutasymbool. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Stelt een waarde in voor PositieValutasymbool. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Stelt een waarde in voor HuidigeDatum. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Stelt een waarde in voor AangepastDatumformaat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Stelt een waarde in voor Datumformaat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Stelt een waarde in voor DagenPerMaand. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Stelt een waarde in voor StandaardEindtijd. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Stelt een waarde in voor StandaardVasteKostenToerekening. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Stelt een waarde in voor StandaardOvertijdTarief. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Stelt een waarde in voor DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Stelt een waarde in voor DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Stelt een waarde in voor DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Stelt een waarde in voor DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Stelt de standaardweergave van het project in. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Stelt een waarde in voor DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Stelt een waarde in voor EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Stelt een waarde in voor ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Stelt een waarde in voor FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of FiscalYearStart is ingesteld of niet. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Stelt een waarde in voor FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Stelt globalisatie (taalspecifieke) instellingen van het project in. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Stelt een waarde in voor Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of HonorConstraints is ingesteld of niet. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Stelt een waarde in voor HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Stelt een waarde in voor Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Stelt een waarde in voor LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Stelt een waarde in voor LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Stelt een waarde in voor LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Stelt een waarde in voor Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MicrosoftProjectServerURL is ingesteld of niet. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Stelt een waarde in voor MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Stelt een waarde in voor MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MoveCompletedEndsBack is ingesteld of niet. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MoveCompletedEndsForward is ingesteld of niet. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MoveRemainingStartsBack is ingesteld of niet. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MoveRemainingStartsForward is ingesteld of niet. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of MultipleCriticalPaths is ingesteld of niet. |
| [setName(String value)](#setName-java.lang.String-) | Stelt een waarde in voor Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Stelt een waarde in voor NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of NewTasksAreManual is ingesteld of niet. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of NewTasksEffortDriven is ingesteld of niet. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of NewTasksEstimated is ingesteld of niet. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of ProjectExternallyEdited is ingesteld of niet. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of RemoveFileProperties is ingesteld of niet. |
| [setRevision(int value)](#setRevision-int-) | Stelt een waarde in voor Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Stelt een waarde in voor SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of ScheduleFromStart is ingesteld of niet. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Stelt een waarde in die aangeeft of ShowProjectSummaryTask is ingesteld of niet. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of SplitsInProgressTasks is ingesteld of niet. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of SpreadActualCost is ingesteld of niet. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of SpreadPercentComplete is ingesteld of niet. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Stelt een waarde in voor StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Stelt een waarde in voor StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Stelt een waarde in voor Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of TaskUpdatesResource is ingesteld of niet. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Stelt een waarde in voor Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Stelt een waarde in voor TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Stelt een waarde in voor TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Stelt een waarde in voor Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Stelt een waarde van Uid in. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of UpdateManuallyScheduledTasksWhenEditingLinks is ingesteld of niet. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Stelt de WBS-code-definitie in voor het project. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Stelt een waarde in voor WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Stelt een waarde in voor WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Markeert al het werk als voltooid tot een opgegeven datum voor het gehele project. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Markeert al het werk als voltooid tot een opgegeven datum voor de opgegeven lijst met taken. |
### Project() {#Project--}
```
public Project()
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een met wachtwoord beveiligde sjabloon (bestaand mpp- of mpt‑bestand).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pad naar sjabloon om een project van te maken. |
|  | protectionPassword | java.lang.String | Beschermingswachtwoord. |

--------------------

Het lezen van met wachtwoord beveiligde bestanden wordt momenteel alleen ondersteund voor het MSP 2003-bestandsformaat. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pad naar sjabloon om een project van te maken. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit de Stream met de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Stream van de Project java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)class die het mogelijk maakt om het lezen van Primavera-formaten (XER of XML) aan te passen. |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pad naar sjabloon om een project van te maken. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | de opgegeven callback-methode om xml-parsefouten af te handelen. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream om een sjabloon van te laden. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project)-klasse vanuit een sjabloon (bestaand MPP‑ of MPT‑bestand) met de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pad naar sjabloon om een project van te maken |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | de opgegeven instantie van de [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse om gegevens te lezen uit een database die wordt gespecificeerd door het exemplaar van de [DbSettings](../../com.aspose.tasks/dbsettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | de opgegeven instantie van de [DbSettings](../../com.aspose.tasks/dbsettings) class. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream om een sjabloon van te laden. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | de opgegeven callback-methode om xml-parsefouten af te handelen. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream om een sjabloon van te laden. |
|  | protectionPassword | java.lang.String | Beschermingswachtwoord. |

--------------------

Het lezen van met wachtwoord beveiligde bestanden wordt momenteel alleen ondersteund voor het MSP 2003-bestandsformaat. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand) met het gespecificeerde exemplaar van de [LoadOptions](../../com.aspose.tasks/loadoptions) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pad naar sjabloon om een project van te maken |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | de opgegeven instantie van de [LoadOptions](../../com.aspose.tasks/loadoptions) class. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Initialiseert een nieuw exemplaar van de [Project](../../com.aspose.tasks/project) klasse vanuit de Stream met het gespecificeerde exemplaar van de [LoadOptions](../../com.aspose.tasks/loadoptions) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Stream van de Project java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | de opgegeven instantie van de [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Retourneert de waarde waaraan de eigenschap in deze container is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Prj](../../com.aspose.tasks/prj) om de eigenschapssleutel op te halen. |

**Returns:**
T - de waarde waaraan de eigenschap in deze container is toegewezen.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Prj](../../com.aspose.tasks/prj) om de eigenschapssleutel op te halen. |
| val | T | de waarde. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Een ander project om gegevens naartoe te kopiëren. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Een ander project om gegevens naartoe te kopiëren. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Kopieeropties om het kopieerproces te beheersen. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Somt recursief alle taken van het project op, inclusief de hoofdtaak.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable die kan worden gebruikt om over alle taken van het project te itereren.

--------------------

Biedt een lichtere manier om over taken te itereren vergeleken met de [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) methode, omdat deze geen geheugen toewijst voor alle taken.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Haalt een waarde op die aangeeft of ActualsInSync is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Haalt een waarde op die aangeeft of AdminProject is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Haalt een waarde op die aangeeft of AreEditableActualCosts is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Haalt de waarde van Author op.

**Returns:**
java.lang.String - een waarde van Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Haalt een waarde op die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Haalt op of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk en de tarief van de toewijzing.

**Returns:**
boolean - of assignment cost en remaining cost automatisch moeten worden berekend met behulp van assignment's work en resource rates.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Haalt een waarde op die aangeeft of Autolink is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Haalt de waarde van BaselineForEarnedValue op.

**Returns:**
int - een waarde van BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Retourneert de opslagtijd van de baseline. Retourneert DateTime.MinValue (00:00:00.0000000 UTC, 1 januari 0001) als de baseline niet is opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| baselineNumber | int | Het nummer van de baseline [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - De laatste opslagtijd en datum van de baseline.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Haalt de verzameling ingebouwde eigenschappen van het project op.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Haalt de berekeningsmodus van een project op. Kan een van de waarden van `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeratie zijn.

**Returns:**
int - berekeningsmodus van een project.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Haalt een waarde van Calendar op.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Haalt het [CalendarCollection](../../com.aspose.tasks/calendarcollection) object op van dit Project‑exemplaar.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Haalt de waarde van Category op.

**Returns:**
java.lang.String - een waarde van Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Haalt de waarde van Comments op.

**Returns:**
java.lang.String - een waarde van Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Haalt de waarde van Company op.

**Returns:**
java.lang.String - een waarde van Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Haalt de waarde van CreationDate op.

**Returns:**
java.util.Date - een waarde van CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Haalt een verzameling op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Dit is een O(n)-operatie, waarbij n het aantal taken in het project is.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Taken worden door MS Project als kritisch beschouwd als de totale speling minder dan of gelijk aan dit aantal dagen is.

**Returns:**
int - de maximale waarde van totale spelingstijd (in dagen) waarbij een taak als kritisch wordt beschouwd
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Haalt de waarde van CurrencyCode op.

**Returns:**
java.lang.String - een waarde van CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Haalt een waarde op van CurrencyDigits.

**Returns:**
int - een waarde van CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Haalt een waarde op van CurrencySymbol.

**Returns:**
java.lang.String - een waarde van CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Haalt een waarde op van CurrencySymbolPosition.

**Returns:**
int - een waarde van CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Haalt een waarde op van CurrentDate.

**Returns:**
java.util.Date - een waarde van CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Haalt een waarde op van CustomDateFormat.

**Returns:**
java.lang.String - een waarde van CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Haalt de collectie met aangepaste projecteigenschappen op.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Haalt een waarde op van DateFormat.

**Returns:**
int - een waarde van DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Haalt een waarde op van DaysPerMonth.

**Returns:**
int - een waarde van DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Haalt een waarde op van DefaultFinishTime.

**Returns:**
java.util.Date - een waarde van DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Haalt een waarde op van DefaultFixedCostAccrual.

**Returns:**
int - een waarde van DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Haalt een waarde op van DefaultOvertimeRate.

**Returns:**
double - een waarde van DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Haalt een waarde op van DefaultStandardRate.

**Returns:**
double - een waarde van DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Haalt een waarde op van DefaultStartTime.

**Returns:**
java.util.Date - een waarde van DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Haalt een waarde op van DefaultTaskEVMethod.

**Returns:**
int - een waarde van DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Haalt een waarde op van DefaultTaskType.

**Returns:**
int - een waarde van DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Haalt de standaardweergave van het project op.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Haalt de instantie van de klasse [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) op, die een collectie van de standaardwerkdagen en werktijden van het project vertegenwoordigt.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

De gegevens komen alleen voor in mpp‑bestanden (niet in xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Haalt een instantie van de klasse [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) op.

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Haalt een [Duration](../../com.aspose.tasks/duration)-object op met het opgegeven aantal eenheden en het standaardduurtijdformaat dat is gedefinieerd in de projectinstellingen [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | val | double | gespecificeerd aantal eenheden. |

--------------------

Deze methode moet zorgvuldig worden gebruikt omdat deze verschillende duurwaarden retourneert, afhankelijk van de instelling Project.DurationFormat. Bijvoorbeeld, GetWork(1.0) retourneert 1 uur wanneer Project.DurationFormat TimeUnitType.Hour is of 1 dag als Project.DurationFormat TimeUnitType.Day is. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Haalt een [Duration](../../com.aspose.tasks/duration)-object op met het opgegeven aantal [TimeUnitType](../../com.aspose.tasks/timeunittype)-eenheden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| val | double | gespecificeerd aantal eenheden. |
| timeUnit | byte | gespecificeerde TimeUnitType‑waarde. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Haalt een waarde op van DurationFormat.

**Returns:**
byte - een waarde van DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Haalt een waarde op van EarnedValueMethod.

**Returns:**
int - een waarde van EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Haalt ExtendedAttributeDefinitionCollection‑object op. De collectie van definities van uitgebreide attributen (aangepaste velden) die aan een project zijn gekoppeld.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Haalt een waarde op van ExtendedCreationDate.

**Returns:**
java.util.Date - een waarde van ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Haalt een waarde op van FinishDate.

**Returns:**
java.util.Date - een waarde van FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Haalt een waarde op die aangeeft of FiscalYearStart is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Haalt een waarde op van FyStartDate.

**Returns:**
int - een waarde van FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Haalt globalisatie (taalspecifieke) instellingen van het project op.

De aanbevolen manier is om cultuur‑invariante literals of opmaak te gebruiken gedurende het hele project. Als een project echter cultuur‑specifieke literals gebruikt, kan deze klasse worden gebruikt om de berekeningsengine te helpen die literals te parseren.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Haalt een waarde van Guid op.

**Returns:**
java.util.UUID - een waarde van Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Haalt een waarde op die aangeeft of HonorConstraints is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Haalt een waarde op van HyperlinkBase.

**Returns:**
java.lang.String - een waarde van HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Haalt een waarde op die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Haalt een waarde op die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Haalt een waarde op van Keywords.

**Returns:**
java.lang.String - een waarde van Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Haalt een waarde op van LastAuthor.

**Returns:**
java.lang.String - een waarde van LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Haalt een waarde op van LastPrinted.

**Returns:**
java.util.Date - een waarde van LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Haalt een waarde op van LastSaved.

**Returns:**
java.util.Date - een waarde van LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Haalt een waarde op van Manager.

**Returns:**
java.lang.String - een waarde van Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Haalt een waarde op die aangeeft of MicrosoftProjectServerURL is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Haalt een waarde op van MinutesPerDay.

**Returns:**
int - een waarde van MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Haalt een waarde op van MinutesPerWeek.

**Returns:**
int - een waarde van MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Haalt een waarde op die aangeeft of MoveCompletedEndsBack is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Haalt een waarde op die aangeeft of MoveCompletedEndsForward is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Haalt een waarde op die aangeeft of MoveRemainingStartsBack is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Haalt een waarde op die aangeeft of MoveRemainingStartsForward is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Haalt een waarde op die aangeeft of MultipleCriticalPaths is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Haalt een waarde van Name op.

**Returns:**
java.lang.String - een waarde van Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Haalt een waarde op van NewTaskStartDate.

**Returns:**
int - een waarde van NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Haalt een waarde op die aangeeft of NewTasksAreManual is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Haalt een waarde op die aangeeft of NewTasksEffortDriven is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Haalt een waarde op die aangeeft of NewTasksEstimated is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Haalt een collectie op die de instanties van de [OleObject](../../com.aspose.tasks/oleobject) klasse bevat die gekoppeld of ingesloten zijn in dit projectbestand.

--------------------

Alleen beschikbaar voor mpp-bestandsformaat. Deze collectie is alleen-lezen, behalve voor de 'Clear'-bewerking.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Haalt OutlineCodeDefinitionCollection-object op. De collectie van outline-code-definities die aan een project zijn gekoppeld.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Retourneert paginatelling voor het project dat wordt gerenderd met de standaard [Timescale](../../com.aspose.tasks/timescale)(Dagen).

**Returns:**
int - Aantal pagina's dat moet worden gerenderd.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven [SaveOptions](../../com.aspose.tasks/saveoptions).

--------------------

&gt; ```
&gt; In dit voorbeeld wordt een instantie van HtmlSaveOptions en het aantal pagina's in de resulterende HTML naar de console geschreven.
&gt; ``````

  [C#]
Project project = new Project(@"test.mpp");
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

