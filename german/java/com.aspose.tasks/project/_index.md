---
title: "Projekt"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Projekt dar."
type: docs
weight: 220
url: /de/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Stellt ein Projekt dar.

--------------------

Die **Project** ist eine zentrale Klasse in der Aspose.Tasks-Bibliothek.

Man kann **Project** verwenden, um eines der unterstützten Projektmanagement‑Formate zu lesen: MPP, MPT, MPX, XML.

Um ein vorhandenes Dokument in einem der unterstützten Formate zu laden, übergeben Sie einen Dateinamen oder einen Stream an einen der **Project**‑Konstruktoren. Um ein leeres Projekt zu erstellen, rufen Sie den parameterlosen Konstruktor auf.

Verwenden Sie eine der Überladungen der Save‑Methode, um das Projekt in einem der [SaveFileFormat](../../com.aspose.tasks/savefileformat) Formate zu speichern: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Festes Layout: PDF; Bilder: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Andere: HTML.

Um das Projekt zu drucken, verwenden Sie eine der [print()](../../com.aspose.tasks/project\#print--) Methodenüberladungen.

Die **Project** speichert projektweite Informationen wie `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)) und `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). Die meisten dieser Objekte sind über die entsprechenden Eigenschaften der **Project**‑Klasse zugänglich.

Die **Project** ist eine Basiseinheit, die Einstiegspunkte enthält, um andere Projektelemente zu manipulieren, wie [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) und [Calendar](../../com.aspose.tasks/calendar).

Die **Project**-Entitäten können über typisierte Sammlungen abgerufen werden, zum Beispiel `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), usw.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Project()](#Project--) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer passwortgeschützten Vorlage (bestehende mpp- oder mpt-Datei). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus dem Stream mit der angegebenen Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einem Stream. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende MPP- oder MPT-Datei) mit der angegebenen Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse. |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse, um Daten aus einer Datenbank zu lesen, die durch die Instanz der [DbSettings](../../com.aspose.tasks/dbsettings)-Klasse angegeben ist. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei) mit der angegebenen Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions)-Klasse. |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus dem Stream mit der angegebenen Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Enumeriert rekursiv alle Aufgaben des Projekts, einschließlich der Root-Aufgabe. |
| [getActualsInSync()](#getActualsInSync--) | Gibt einen Wert zurück, der angibt, ob ActualsInSync gesetzt ist oder nicht. |
| [getAdminProject()](#getAdminProject--) | Gibt einen Wert zurück, der angibt, ob AdminProject gesetzt ist oder nicht. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Gibt einen Wert zurück, der angibt, ob AreEditableActualCosts gesetzt ist oder nicht. |
| [getAuthor()](#getAuthor--) | Gibt den Wert von Author zurück. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Gibt einen Wert zurück, der angibt, ob AutoAddNewResourcesAndTasks gesetzt ist oder nicht. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Gibt an, ob die Aufgabenkosten und Restkosten automatisch anhand der Arbeitszeit der Aufgabe und der Ressourcensätze berechnet werden sollen. |
| [getAutolink()](#getAutolink--) | Gibt einen Wert zurück, der angibt, ob Autolink gesetzt ist oder nicht. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Gibt den Wert von BaselineForEarnedValue zurück. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Gibt die Basislinien‑Speicherzeit zurück. |
| [getBuiltInProps()](#getBuiltInProps--) | Ruft die integrierte Eigenschaftensammlung des Projekts ab. |
| [getCalculationMode()](#getCalculationMode--) | Ruft den Berechnungsmodus eines Projekts ab. |
| [getCalendar()](#getCalendar--) | Ruft den Wert von Calendar ab. |
| [getCalendars()](#getCalendars--) | Ruft das [CalendarCollection](../../com.aspose.tasks/calendarcollection)-Objekt dieser Projektinstanz ab. |
| [getCategory()](#getCategory--) | Ruft den Wert von Kategorie ab. |
| [getComments()](#getComments--) | Ruft den Wert von Kommentaren ab. |
| [getCompany()](#getCompany--) | Ruft den Wert von Unternehmen ab. |
| [getCreationDate()](#getCreationDate--) | Ruft den Wert von Erstellungsdatum ab. |
| [getCriticalPath()](#getCriticalPath--) | Ruft eine Sammlung ab, die eine Liste kritischer Vorgänge enthält, die den kritischen Pfad dieses Projekts bilden. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Vorgänge gelten in MS Project als kritisch, wenn die Gesamtspanne kleiner oder gleich dieser Anzahl von Tagen ist. |
| [getCurrencyCode()](#getCurrencyCode--) | Ruft den Wert von Währungscode ab. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Ruft den Wert von Währungsstellen ab. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Ruft den Wert von Währungssymbol ab. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Ruft den Wert von Position des Währungssymbols ab. |
| [getCurrentDate()](#getCurrentDate--) | Ruft den Wert von aktuellem Datum ab. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Ruft den Wert von benutzerdefiniertem Datumsformat ab. |
| [getCustomProps()](#getCustomProps--) | Ruft die benutzerdefinierte Eigenschaftensammlung des Projekts ab. |
| [getDateFormat()](#getDateFormat--) | Ruft den Wert von Datumsformat ab. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Ruft den Wert von Tagen pro Monat ab. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Ruft den Wert von Standard-Endzeit ab. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Ruft den Wert von Standard-Festkosten-Zuordnung ab. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Ruft den Wert von Standard-Überstundensatz ab. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Ruft den Wert von Standard-Standardrate ab. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Ruft den Wert von Standard-Startzeit ab. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Ruft den Wert von Standard‑Aufgaben‑EV‑Methode ab. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Gibt einen Wert von DefaultTaskType zurück. |
| [getDefaultView()](#getDefaultView--) | Gibt die Standardansicht des Projekts zurück. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Gibt die Instanz der Klasse [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) zurück, die eine Sammlung der standardmäßigen Arbeitswochentage und Arbeitszeiten des Projekts darstellt. |
| [getDisplayOptions()](#getDisplayOptions--) | Gibt eine Instanz der Klasse [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) zurück. |
| [getDuration(double val)](#getDuration-double-) | Gibt ein [Duration](../../com.aspose.tasks/duration)-Objekt mit der angegebenen Anzahl von Einheiten und dem Standarddauerformat zurück, das in den Projekteinstellungen [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) definiert ist. |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Gibt ein [Duration](../../com.aspose.tasks/duration)-Objekt mit der angegebenen Anzahl von [TimeUnitType](../../com.aspose.tasks/timeunittype)-Einheiten zurück. |
| [getDurationFormat()](#getDurationFormat--) | Gibt einen Wert von DurationFormat zurück. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Gibt einen Wert von EarnedValueMethod zurück. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gibt ein ExtendedAttributeDefinitionCollection-Objekt zurück. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Gibt einen Wert von ExtendedCreationDate zurück. |
| [getFinishDate()](#getFinishDate--) | Gibt einen Wert von FinishDate zurück. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Gibt einen Wert zurück, der angibt, ob FiscalYearStart gesetzt ist oder nicht. |
| [getFyStartDate()](#getFyStartDate--) | Gibt einen Wert von FyStartDate zurück. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Gibt die Globalisierungs- (sprachspezifischen) Einstellungen des Projekts zurück. |
| [getGuid()](#getGuid--) | Ruft den Wert von Guid ab. |
| [getHonorConstraints()](#getHonorConstraints--) | Gibt einen Wert zurück, der angibt, ob HonorConstraints gesetzt ist oder nicht. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Gibt einen Wert von HyperlinkBase zurück. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Gibt einen Wert zurück, der angibt, ob InsertedProjectsLikeSummary gesetzt ist oder nicht. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Gibt einen Wert zurück, der angibt, ob KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled gesetzt ist oder nicht. |
| [getKeywords()](#getKeywords--) | Gibt einen Wert von Keywords zurück. |
| [getLastAuthor()](#getLastAuthor--) | Gibt einen Wert von LastAuthor zurück. |
| [getLastPrinted()](#getLastPrinted--) | Gibt einen Wert von LastPrinted zurück. |
| [getLastSaved()](#getLastSaved--) | Gibt einen Wert von LastSaved zurück. |
| [getManager()](#getManager--) | Gibt einen Wert von Manager zurück. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Gibt einen Wert zurück, der angibt, ob MicrosoftProjectServerURL gesetzt ist oder nicht. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Gibt einen Wert von MinutesPerDay zurück. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Gibt einen Wert von MinutesPerWeek zurück. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsBack gesetzt ist oder nicht. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsForward gesetzt ist oder nicht. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsBack gesetzt ist oder nicht. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsForward gesetzt ist oder nicht. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Gibt einen Wert zurück, der angibt, ob MultipleCriticalPaths gesetzt ist oder nicht. |
| [getName()](#getName--) | Ruft den Wert von Name ab. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Gibt einen Wert von NewTaskStartDate zurück. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Gibt einen Wert zurück, der angibt, ob NewTasksAreManual gesetzt ist oder nicht. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Gibt einen Wert zurück, der angibt, ob NewTasksEffortDriven gesetzt ist oder nicht. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Gibt einen Wert zurück, der angibt, ob NewTasksEstimated gesetzt ist oder nicht. |
| [getOleObjects()](#getOleObjects--) | Ruft eine Sammlung ab, die die Instanzen der Klasse [OleObject](../../com.aspose.tasks/oleobject) enthält, die mit dieser Projektdatei verknüpft oder eingebettet sind. |
| [getOutlineCodes()](#getOutlineCodes--) | Ruft das Objekt OutlineCodeDefinitionCollection ab. |
| [getPageCount()](#getPageCount--) | Gibt die Seitenzahl für das Projekt zurück, das mit dem Standard-[Timescale](../../com.aspose.tasks/timescale) (Tage) gerendert wird. |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Gibt die Seitenzahl für das Projekt zurück, das mit den angegebenen [SaveOptions](../../com.aspose.tasks/saveoptions) gerendert wird. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Gibt die Seitenzahl für das Projekt zurück, das mit dem angegebenen [Timescale](../../com.aspose.tasks/timescale) und [PresentationFormat](../../com.aspose.tasks/presentationformat) gerendert wird. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Gibt die Seitenzahl für das Projekt zurück, das mit dem angegebenen [Timescale](../../com.aspose.tasks/timescale) und [PageSize](../../com.aspose.tasks/pagesize) gerendert wird. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Gibt die Seitenzahl für das Projekt zurück, das mit dem angegebenen [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) und dem Datumsbereich gerendert wird. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Gibt die Seitenzahl für das Projekt zurück, das mit dem Standard-[Timescale](../../com.aspose.tasks/timescale) (Tage) und dem angegebenen [PresentationFormat](../../com.aspose.tasks/presentationformat) gerendert wird. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Gibt die Seitenzahl für das Projekt zurück, das mit dem angegebenen [Timescale](../../com.aspose.tasks/timescale) gerendert wird. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Gibt eine Sammlung von Aufgabenverknüpfungen zurück, die Vorgänger der angegebenen Aufgabe sind. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Ruft ein Objekt ab, das Primavera-spezifische Eigenschaften für ein aus einer Primavera-Datei gelesenes Projekt enthält. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Gibt einen Wert zurück, der angibt, ob ProjectExternallyEdited gesetzt ist oder nicht. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Ruft Projektdateiinformationen aus dem Stream ab. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Liest Projektdateiinformationen aus der Datei. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Gibt einen Wert zurück, der angibt, ob RemoveFileProperties gesetzt ist oder nicht. |
| [getResourceAssignments()](#getResourceAssignments--) | Liefert das ResourceAssignmentCollection-Objekt. |
| [getResourceFilters()](#getResourceFilters--) | Liefert alle ressourcenbasierten Filterdefinitionen. |
| [getResourceGroups()](#getResourceGroups--) | Liefert alle ressourcenbasierten Gruppendefinitionen. |
| [getResources()](#getResources--) | Liefert das ResourceCollection-Objekt. |
| [getRevision()](#getRevision--) | Liefert einen Wert von Revision. |
| [getRootTask()](#getRootTask--) | Liefert die Wurzel des Aufgabenbaums. |
| [getSaveVersion()](#getSaveVersion--) | Liefert einen Wert von SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Liefert einen Wert, der angibt, ob ScheduleFromStart gesetzt ist oder nicht. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Liefert einen Wert, der angibt, ob ShowProjectSummaryTask gesetzt ist oder nicht. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Liefert einen Wert, der angibt, ob SplitsInProgressTasks gesetzt ist oder nicht. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Liefert einen Wert, der angibt, ob SpreadActualCost gesetzt ist oder nicht. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Liefert einen Wert, der angibt, ob SpreadPercentComplete gesetzt ist oder nicht. |
| [getStartDate()](#getStartDate--) | Liefert einen Wert von StartDate. |
| [getStatusDate()](#getStatusDate--) | Liefert einen Wert von StatusDate. |
| [getSubject()](#getSubject--) | Liefert einen Wert von Subject. |
| [getTables()](#getTables--) | Liefert eine Liste von [Table](../../com.aspose.tasks/table)-Objekten. |
| [getTaskFilters()](#getTaskFilters--) | Liefert alle aufgabenbasierten Filterdefinitionen. |
| [getTaskGroups()](#getTaskGroups--) | Liefert alle aufgabenbasierten Gruppendefinitionen. |
| [getTaskLinks()](#getTaskLinks--) | Liefert das [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection)-Objekt. |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Liefert einen Wert, der angibt, ob TaskUpdatesResource gesetzt ist oder nicht. |
| [getTemplate()](#getTemplate--) | Liefert einen Wert von Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Liefert einen Wert von TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Liefert einen Wert von TimescaleStart. |
| [getTitle()](#getTitle--) | Liefert einen Wert von Title. |
| [getUid()](#getUid--) | Liefert einen Wert von Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Liefert einen Wert, der angibt, ob UpdateManuallyScheduledTasksWhenEditingLinks gesetzt ist oder nicht. |
| [getVbaProject()](#getVbaProject--) | Ruft eine Instanz von `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) Klasse ab. |
| [getViews()](#getViews--) | Ruft eine Liste von [View](../../com.aspose.tasks/view) Objekten ab. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Ruft die WBS-Code-Definition für das Projekt ab. |
| [getWeekStartDay()](#getWeekStartDay--) | Ruft den Wert von WeekStartDay ab. |
| [getWork(double val)](#getWork-double-) | Ruft ein [Duration](../../com.aspose.tasks/duration) Objekt mit dem angegebenen `double` Wert und dem Standardarbeitsformat ab. |
| [getWorkFormat()](#getWorkFormat--) | Ruft den Wert von WorkFormat ab. |
| [print()](#print--) | Druckt das Projekt an den Standarddrucker mit den Standarddruckereinstellungen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Druckt das Projekt an den Standarddrucker mit den Standarddruckereinstellungen und benutzerdefinierten Speicheroptionen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen und benutzerdefinierten Speicheroptionen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen, benutzerdefinierten Speicheroptionen und dem angegebenen Dokumentnamen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [print(String printerName)](#print-java.lang.String-) | Druckt das Projekt an den angegebenen Drucker mit den Standarddruckereinstellungen unter Verwendung des Standard‑Druckcontrollers (no User Interface). |
| [recalculate()](#recalculate--) | Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spättermine, berechnet Puffer, Arbeits- und Kostenfelder neu. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spättermine, berechnet Puffer, Arbeits- und Kostenfelder neu mit optionaler Validierung. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Berechnet Id, Start und Ende von Ressourcen neu. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Berechnet Start und Ende von Ressourcen neu. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Entfernt ungültige Ressourcen‑Zuweisungen aus der Ressourcen‑Zuweisungsliste des Projekts. |
| [renumberWBSCode()](#renumberWBSCode--) | Nummeriert den WBS-Code aller Aufgaben neu. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Nummeriert den WBS-Code übergebener Aufgaben neu. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Plant nicht abgeschlossene Projektarbeit so, dass sie nach einem angegebenen Datum beginnt. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Plant nicht abgeschlossene Arbeit für eine angegebene Aufgabenliste so, dass sie nach einem angegebenen Datum beginnt. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Speichert das Projekt in einen Stream unter Verwendung der angegebenen Speicheroptionen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Speichert die Projektdaten in den Stream. |
| [save(String filename)](#save-java.lang.String-) | Speichert die Projektdaten in die Datei im mpp-Format. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Speichert das Dokument in eine Datei unter Verwendung der angegebenen Speicheroptionen. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Speichert die Projektdaten in die Datei. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Speichert das Projekt als Vorlage in einen angegebenen Stream. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Speichert das Projekt als Vorlage in einen angegebenen Stream. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Speichert das Projekt als Vorlage in den angegebenen Dateipfad. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Speichert das Projekt als Vorlage. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Speichert den Projektübersichtsbericht in den Stream. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Speichert den Projektbericht des angegebenen Typs in den angegebenen Stream. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Speichert den Projektübersichtsbericht in eine PDF-Datei. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Speichert den Projektbericht des angegebenen Typs im PDF-Format in den angegebenen Dateipfad. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Sammelt rekursiv alle Unteraufgaben der Stammaufgabe. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Legt einen Wert fest, der angibt, ob ActualsInSync gesetzt ist oder nicht. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Legt einen Wert fest, der angibt, ob AdminProject gesetzt ist oder nicht. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Legt einen Wert fest, der angibt, ob AreEditableActualCosts gesetzt ist oder nicht. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Legt einen Wert für Author fest. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Legt einen Wert fest, der angibt, ob AutoAddNewResourcesAndTasks gesetzt ist oder nicht. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Legt fest, ob Aufgabenkosten und Restkosten automatisch anhand der Arbeitszeit der Zuordnung und der Ressourcensätze berechnet werden sollen. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Legt einen Wert fest, der angibt, ob Autolink gesetzt ist oder nicht. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Speichert Basislinienfelder in die angegebene Basislinie für das gesamte Projekt. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Speichert Basislinienfelder in die angegebene Basislinie für die ausgewählten Aufgaben. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Legt einen Wert für BaselineForEarnedValue fest. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Legt die Speicherzeit der Basislinie fest. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Legt den Berechnungsmodus eines Projekts fest. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Setzt einen Wert für Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Legt einen Wert für Category fest. |
| [setComments(String value)](#setComments-java.lang.String-) | Legt einen Wert für Comments fest. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Legt einen Wert für Company fest. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Legt einen Wert für CreationDate fest. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Vorgänge gelten in MS Project als kritisch, wenn die Gesamtspanne kleiner oder gleich dieser Anzahl von Tagen ist. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Setzt einen Wert für CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Setzt einen Wert für CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Setzt einen Wert für CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Setzt einen Wert für CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Setzt einen Wert für CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Setzt einen Wert für CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Setzt einen Wert für DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Setzt einen Wert für DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Setzt einen Wert für DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Setzt einen Wert für DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Setzt einen Wert für DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Setzt einen Wert für DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Setzt einen Wert für DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Setzt einen Wert für DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Setzt einen Wert für DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Setzt die Standardansicht des Projekts. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Setzt einen Wert für DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Setzt einen Wert für EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Setzt einen Wert für ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Setzt einen Wert für FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob FiscalYearStart gesetzt ist oder nicht. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Setzt einen Wert für FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Setzt die Globalisierung (sprachspezifische) Einstellungen des Projekts. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Setzt einen Wert für Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob HonorConstraints gesetzt ist oder nicht. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Setzt einen Wert für HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob InsertedProjectsLikeSummary gesetzt ist oder nicht. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled gesetzt ist oder nicht. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Setzt einen Wert für Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Setzt einen Wert für LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Setzt einen Wert für LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Setzt einen Wert für LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Setzt einen Wert für Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MicrosoftProjectServerURL gesetzt ist oder nicht. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Setzt einen Wert für MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Setzt einen Wert für MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MoveCompletedEndsBack gesetzt ist oder nicht. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MoveCompletedEndsForward gesetzt ist oder nicht. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MoveRemainingStartsBack gesetzt ist oder nicht. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MoveRemainingStartsForward gesetzt ist oder nicht. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob MultipleCriticalPaths gesetzt ist oder nicht. |
| [setName(String value)](#setName-java.lang.String-) | Setzt einen Wert für Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Setzt einen Wert für NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob NewTasksAreManual gesetzt ist oder nicht. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob NewTasksEffortDriven gesetzt ist oder nicht. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob NewTasksEstimated gesetzt ist oder nicht. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob ProjectExternallyEdited gesetzt ist oder nicht. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob RemoveFileProperties gesetzt ist oder nicht. |
| [setRevision(int value)](#setRevision-int-) | Setzt einen Wert für Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Setzt einen Wert für SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob ScheduleFromStart gesetzt ist oder nicht. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Setzt einen Wert, der angibt, ob ShowProjectSummaryTask gesetzt ist oder nicht. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob SplitsInProgressTasks gesetzt ist oder nicht. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob SpreadActualCost gesetzt ist oder nicht. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob SpreadPercentComplete gesetzt ist oder nicht. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Setzt einen Wert für StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Setzt einen Wert für StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Setzt einen Wert für Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob TaskUpdatesResource gesetzt ist oder nicht. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Setzt einen Wert für Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Setzt einen Wert für TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Setzt einen Wert für TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Setzt einen Wert für Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Setzt einen Wert für Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob UpdateManuallyScheduledTasksWhenEditingLinks gesetzt ist oder nicht. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Setzt die WBS-Code-Definition für das Projekt. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Setzt einen Wert für WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Setzt einen Wert für WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Aktualisiert alle Arbeiten als abgeschlossen bis zu einem angegebenen Datum für das gesamte Projekt. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Aktualisiert alle Arbeiten als abgeschlossen bis zu einem angegebenen Datum für die angegebene Aufgabenliste. |
### Project() {#Project--}
```
public Project()
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer passwortgeschützten Vorlage (bestehende mpp- oder mpt-Datei).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pfad zur Vorlage, aus der das Projekt erstellt wird. |
|  | protectionPassword | java.lang.String | Schutzkennwort. |

--------------------

Das Lesen passwortgeschützter Dateien wird derzeit nur für das MSP‑2003-Dateiformat unterstützt. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pfad zur Vorlage, aus der das Projekt erstellt wird. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus dem Stream mit der angegebenen Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Stream des Projekts java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | die angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) Klasse, die das Anpassen des Lesens von Primavera-Formaten (XER oder XML) ermöglicht. |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pfad zur Vorlage, aus der das Projekt erstellt wird. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | die angegebene Callback-Methode zum Behandeln von XML-Parse-Fehlern. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einem Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream, um eine Vorlage zu laden. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende MPP- oder MPT-Datei) mit der angegebenen Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pfad zur Vorlage, aus der das Projekt erstellt wird |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | die angegebene Instanz der [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) Klasse. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse, um Daten aus einer Datenbank zu lesen, die durch die Instanz der [DbSettings](../../com.aspose.tasks/dbsettings)-Klasse angegeben ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | die angegebene Instanz der [DbSettings](../../com.aspose.tasks/dbsettings) Klasse. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream, um eine Vorlage zu laden. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | die angegebene Callback-Methode zum Behandeln von XML-Parse-Fehlern. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream, um eine Vorlage zu laden. |
|  | protectionPassword | java.lang.String | Schutzkennwort. |

--------------------

Das Lesen passwortgeschützter Dateien wird derzeit nur für das MSP‑2003-Dateiformat unterstützt. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei) mit der angegebenen Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectTemplate | java.lang.String | Pfad zur Vorlage, aus der das Projekt erstellt wird |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | die angegebene Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions) Klasse. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Initialisiert eine neue Instanz der [Project](../../com.aspose.tasks/project)-Klasse aus dem Stream mit der angegebenen Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Stream des Projekts java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | die angegebene Instanz der [LoadOptions](../../com.aspose.tasks/loadoptions) Klasse |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | der angegebene Eigenschaftsschlüssel. [Prj](../../com.aspose.tasks/prj) zum Abrufen des Eigenschaftsschlüssels. |

**Returns:**
T - der Wert, dem die Eigenschaft in diesem Container zugeordnet ist.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | der angegebene Eigenschaftsschlüssel. [Prj](../../com.aspose.tasks/prj) zum Abrufen des Eigenschaftsschlüssels. |
| val | T | der Wert. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Ein weiteres Projekt, zu dem Daten kopiert werden. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Ein weiteres Projekt, zu dem Daten kopiert werden. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Kopieroptionen zur Steuerung des Kopiervorgangs. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Enumeriert rekursiv alle Aufgaben des Projekts, einschließlich der Root-Aufgabe.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable, das verwendet werden kann, um über alle Aufgaben des Projekts zu iterieren.

--------------------

Bietet eine ressourcenschonendere Möglichkeit, über Aufgaben zu iterieren, verglichen mit der Methode [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--), da sie keinen Speicher für alle Aufgaben reserviert.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Gibt einen Wert zurück, der angibt, ob ActualsInSync gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Gibt einen Wert zurück, der angibt, ob AdminProject gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Gibt einen Wert zurück, der angibt, ob AreEditableActualCosts gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Gibt den Wert von Author zurück.

**Returns:**
java.lang.String - ein Wert von Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Gibt einen Wert zurück, der angibt, ob AutoAddNewResourcesAndTasks gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Gibt an, ob die Aufgabenkosten und Restkosten automatisch anhand der Arbeitszeit der Aufgabe und der Ressourcensätze berechnet werden sollen.

**Returns:**
boolean - ob die Kosten der Zuordnung und die Restkosten automatisch anhand der Arbeitszeit der Zuordnung und der Ressourcensätze berechnet werden sollen.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Gibt einen Wert zurück, der angibt, ob Autolink gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Gibt den Wert von BaselineForEarnedValue zurück.

**Returns:**
int - ein Wert von BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Gibt die Speicherzeit des Baselines zurück. Gibt DateTime.MinValue (00:00:00.0000000 UTC, 1. Januar 0001) zurück, wenn das Baseline nicht gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baselineNumber | int | Die Nummer des Baselines [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - Das letzte Speicherdatum und die -zeit des Baselines.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Ruft die integrierte Eigenschaftensammlung des Projekts ab.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Ermittelt den Berechnungsmodus eines Projekts. Kann einer der Werte der Aufzählung `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) sein.

**Returns:**
int - Berechnungsmodus eines Projekts.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Ruft den Wert von Calendar ab.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Ruft das [CalendarCollection](../../com.aspose.tasks/calendarcollection)-Objekt dieser Projektinstanz ab.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Ruft den Wert von Kategorie ab.

**Returns:**
java.lang.String - ein Wert von Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Ruft den Wert von Kommentaren ab.

**Returns:**
java.lang.String - ein Wert von Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Ruft den Wert von Unternehmen ab.

**Returns:**
java.lang.String - ein Wert von Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Ruft den Wert von Erstellungsdatum ab.

**Returns:**
java.util.Date - ein Wert von CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Ruft eine Sammlung ab, die eine Liste kritischer Vorgänge enthält, die den kritischen Pfad dieses Projekts bilden.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Dies ist eine O(n)-Operation, wobei n die Anzahl der Aufgaben im Projekt ist.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Vorgänge gelten in MS Project als kritisch, wenn die Gesamtspanne kleiner oder gleich dieser Anzahl von Tagen ist.

**Returns:**
int – der maximale Wert der Gesamtslackzeit (in Tagen), bei dem eine Aufgabe als kritisch gilt.
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Ruft den Wert von Währungscode ab.

**Returns:**
java.lang.String – ein Wert von CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Ruft den Wert von Währungsstellen ab.

**Returns:**
int – ein Wert von CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Ruft den Wert von Währungssymbol ab.

**Returns:**
java.lang.String – ein Wert von CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Ruft den Wert von Position des Währungssymbols ab.

**Returns:**
int – ein Wert von CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Ruft den Wert von aktuellem Datum ab.

**Returns:**
java.util.Date – ein Wert von CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Ruft den Wert von benutzerdefiniertem Datumsformat ab.

**Returns:**
java.lang.String – ein Wert von CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Ruft die benutzerdefinierte Eigenschaftensammlung des Projekts ab.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Ruft den Wert von Datumsformat ab.

**Returns:**
int – ein Wert von DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Ruft den Wert von Tagen pro Monat ab.

**Returns:**
int – ein Wert von DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Ruft den Wert von Standard-Endzeit ab.

**Returns:**
java.util.Date – ein Wert von DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Ruft den Wert von Standard-Festkosten-Zuordnung ab.

**Returns:**
int – ein Wert von DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Ruft den Wert von Standard-Überstundensatz ab.

**Returns:**
double – ein Wert von DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Ruft den Wert von Standard-Standardrate ab.

**Returns:**
double – ein Wert von DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Ruft den Wert von Standard-Startzeit ab.

**Returns:**
java.util.Date – ein Wert von DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Ruft den Wert von Standard‑Aufgaben‑EV‑Methode ab.

**Returns:**
int – ein Wert von DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Gibt einen Wert von DefaultTaskType zurück.

**Returns:**
int – ein Wert von DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Gibt die Standardansicht des Projekts zurück.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Gibt die Instanz der Klasse [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) zurück, die eine Sammlung der standardmäßigen Arbeitswochentage und Arbeitszeiten des Projekts darstellt.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Die Daten sind nur in mpp-Dateien enthalten (nicht in xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Gibt eine Instanz der Klasse [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) zurück.

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Gibt ein [Duration](../../com.aspose.tasks/duration)-Objekt mit der angegebenen Anzahl von Einheiten und dem Standarddauerformat zurück, das in den Projekteinstellungen [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) definiert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | val | double | angegebene Anzahl von Einheiten. |

--------------------

Diese Methode sollte vorsichtig verwendet werden, da sie je nach Einstellung von Project.DurationFormat unterschiedliche Dauern zurückgibt. Zum Beispiel gibt GetWork(1.0) 1 Stunde zurück, wenn Project.DurationFormat TimeUnitType.Hour ist, oder 1 Tag, wenn Project.DurationFormat TimeUnitType.Day ist. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Gibt ein [Duration](../../com.aspose.tasks/duration)-Objekt mit der angegebenen Anzahl von [TimeUnitType](../../com.aspose.tasks/timeunittype)-Einheiten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| val | double | angegebene Anzahl von Einheiten. |
| timeUnit | byte | angegebener TimeUnitType-Wert. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Gibt einen Wert von DurationFormat zurück.

**Returns:**
byte – ein Wert von DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Gibt einen Wert von EarnedValueMethod zurück.

**Returns:**
int – ein Wert von EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Ruft das Objekt ExtendedAttributeDefinitionCollection ab. Die Sammlung von Definitionen erweiterter Attribute (benutzerdefinierter Felder), die einem Projekt zugeordnet sind.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Gibt einen Wert von ExtendedCreationDate zurück.

**Returns:**
java.util.Date - ein Wert von ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Gibt einen Wert von FinishDate zurück.

**Returns:**
java.util.Date - ein Wert von FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Gibt einen Wert zurück, der angibt, ob FiscalYearStart gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Gibt einen Wert von FyStartDate zurück.

**Returns:**
int - ein Wert von FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Gibt die Globalisierungs- (sprachspezifischen) Einstellungen des Projekts zurück.

Die empfohlene Vorgehensweise ist, kulturunabhängige Literale oder Formate im gesamten Projekt zu verwenden. Wenn ein Projekt jedoch kulturspezifische Literale verwendet, kann diese Klasse verwendet werden, um der Berechnungs-Engine beim Parsen dieser Literale zu helfen.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Ruft den Wert von Guid ab.

**Returns:**
java.util.UUID - ein Wert von Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Gibt einen Wert zurück, der angibt, ob HonorConstraints gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Gibt einen Wert von HyperlinkBase zurück.

**Returns:**
java.lang.String - ein Wert von HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Gibt einen Wert zurück, der angibt, ob InsertedProjectsLikeSummary gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Gibt einen Wert zurück, der angibt, ob KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Gibt einen Wert von Keywords zurück.

**Returns:**
java.lang.String - ein Wert von Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Gibt einen Wert von LastAuthor zurück.

**Returns:**
java.lang.String - ein Wert von LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Gibt einen Wert von LastPrinted zurück.

**Returns:**
java.util.Date - ein Wert von LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Gibt einen Wert von LastSaved zurück.

**Returns:**
java.util.Date - ein Wert von LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Gibt einen Wert von Manager zurück.

**Returns:**
java.lang.String - ein Wert von Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Gibt einen Wert zurück, der angibt, ob MicrosoftProjectServerURL gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Gibt einen Wert von MinutesPerDay zurück.

**Returns:**
int - ein Wert von MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Gibt einen Wert von MinutesPerWeek zurück.

**Returns:**
int - ein Wert von MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsBack gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsForward gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsBack gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsForward gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Gibt einen Wert zurück, der angibt, ob MultipleCriticalPaths gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Wert von Name ab.

**Returns:**
java.lang.String - ein Wert von Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Gibt einen Wert von NewTaskStartDate zurück.

**Returns:**
int - ein Wert von NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Gibt einen Wert zurück, der angibt, ob NewTasksAreManual gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Gibt einen Wert zurück, der angibt, ob NewTasksEffortDriven gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Gibt einen Wert zurück, der angibt, ob NewTasksEstimated gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Ruft eine Sammlung ab, die die Instanzen der Klasse [OleObject](../../com.aspose.tasks/oleobject) enthält, die mit dieser Projektdatei verknüpft oder eingebettet sind.

--------------------

Nur für das mpp-Dateiformat verfügbar. Diese Sammlung ist schreibgeschützt, außer für die 'Clear'-Operation.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Ruft das OutlineCodeDefinitionCollection-Objekt ab. Die Sammlung von Gliederungscode-Definitionen, die mit einem Projekt verknüpft sind.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gibt die Seitenzahl für das Projekt zurück, das mit dem Standard-[Timescale](../../com.aspose.tasks/timescale) (Tage) gerendert wird.

**Returns:**
int - Seitenanzahl, die gerendert werden soll.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Gibt die Seitenzahl für das Projekt zurück, das mit den angegebenen [SaveOptions](../../com.aspose.tasks/saveoptions) gerendert wird.

--------------------

&gt; ```
&gt; In diesem Beispiel wird die Instanz von HtmlSaveOptions und die Seitenzahl des resultierenden HTML in die Konsole geschrieben.
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

