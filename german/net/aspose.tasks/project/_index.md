---
title: Project
second_title: Aspose.Tasks für .NET-API-Referenz
description: steht für ein Projekt.
type: docs
weight: 1180
url: /de/net/aspose.tasks/project/
---
## Project class

steht für ein Projekt.

```csharp
public class Project
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Project](project#constructor)() | Initialisiert eine neue Instanz von[`Project`](../project) Klasse. |
| [Project](project#constructor_1)(DbSettings) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse zum Lesen von Daten aus einer Datenbank, die durch die Instanz von angegeben wird[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) Klasse. |
| [Project](project#constructor_2)(Stream) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einem Stream. |
| [Project](project#constructor_9)(StreamReader) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer StreamReader-Instanz. |
| [Project](project#constructor_10)(string) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene mpp- oder mpt-Datei). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus Stream mit der angegebenen Instanz der[`LoadOptions`](../loadoptions) Klasse. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene mpp- oder mpt-Datei). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus Stream mit der angegebenen Instanz der[`PrimaveraReadOptions`](../primaverareadoptions) Klasse. |
| [Project](project#constructor_8)(Stream, string) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene mpp- oder mpt-Datei). |
| [Project](project#constructor_11)(string, LoadOptions) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene mpp- oder mpt-Datei) mit der angegebenen Instanz der[`LoadOptions`](../loadoptions) Klasse. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene mpp- oder mpt-Datei). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer Vorlage (vorhandene MPP- oder MPT-Datei) mit der angegebenen Instanz der[`PrimaveraReadOptions`](../primaverareadoptions) Klasse. |
| [Project](project#constructor_16)(string, string) | Initialisiert eine neue Instanz von[`Project`](../project) Klasse aus einer passwortgeschützten Vorlage (vorhandene mpp- oder mpt-Datei). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Ruft die integrierte Eigenschaftensammlung des Projekts ab. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Ruft den Berechnungsmodus eines Projekts ab oder legt ihn fest. Kann einer der Werte von sein[`CalculationMode`](./calculationmode) Aufzählung. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | erhält[`CalendarCollection`](../calendarcollection) Objekt dieser Projektinstanz. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Ruft eine Sammlung ab, die eine Liste kritischer Aufgaben enthält, die den kritischen Pfad dieses Projekts umfassen. Dies ist eine O(n)-Operation, wobei n die Anzahl der Aufgaben im Projekt ist. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Ruft die Sammlung benutzerdefinierter Eigenschaften des Projekts ab. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Ruft die Standardansicht des Projekts ab oder legt sie fest. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Ruft die Instanz von ab[`WeekDayCollection`](../weekdaycollection) Klasse, die eine Sammlung von Projekt-Standardwochenarbeitstagen und -arbeitszeiten darstellt. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Ruft eine Instanz von ab[`ProjectDisplayOptions`](../projectdisplayoptions) Klasse. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Ruft das ExtendedAttributeDefinitionCollection-Objekt ab. Die Sammlung von erweiterten Attributdefinitionen (benutzerdefinierte Felder), die einem Projekt zugeordnet sind. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Ruft eine Sammlung ab, die die Instanzen von enthält[`OleObject`](../oleobject) Klasse, die mit dieser Projektdatei verknüpft oder eingebettet sind. Nur für mpp-Dateiformat verfügbar. Diese Sammlung ist schreibgeschützt, mit Ausnahme des 'Clear'-Vorgangs. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Ruft das OutlineCodeDefinitionCollection-Objekt ab. Die Sammlung von Gliederungscodedefinitionen, die einem Projekt zugeordnet sind. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Ruft das ResourceAssignmentCollection-Objekt ab. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Ruft alle ressourcenbasierten Filterdefinitionen ab. ResourceFilters ist eine Sammlung von[`Filter`](../filter) Objekte. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Ruft alle ressourcenbasierten Gruppendefinitionen ab. ResourceGroups ist eine Sammlung von[`Group`](../group) Objekte. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Ruft das ResourceCollection-Objekt ab. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Ruft die Wurzel des Aufgabenbaums ab. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Ruft eine Liste von ab[`Table`](../table) Objekte. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Ruft alle aufgabenbasierten Filterdefinitionen ab. TaskFilters ist eine Sammlung von[`Filter`](../filter) Objekte. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Ruft alle aufgabenbasierten Gruppendefinitionen ab. TaskGroups ist eine Sammlung von[`Group`](../group) Objekte. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | erhält[`TaskLinkCollection`](../tasklinkcollection) Objekt. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Ruft eine Instanz von ab[`VbaProject`](./vbaproject) Klasse. |
| [Views](../../aspose.tasks/project/views) { get; } | Ruft eine Liste von ab[`View`](../view) Objekte. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Ruft die PSP-Code-Definition für das Projekt ab oder legt sie fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Listet rekursiv alle Aufgaben des Projekts auf, einschließlich der Stammaufgabe. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Gibt die Grundspeicherzeit zurück. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | erhält[`Duration`](../duration) Objekt mit der angegebenen Anzahl von Einheiten und dem Standarddauerformat, das in den Projekteinstellungen definiert ist[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | erhält[`Duration`](../duration) Objekt mit der angegebenen Anzahl von[`TimeUnitType`](../timeunittype) Einheiten. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | erhält[`Duration`](../duration) Objekt mit dem angegebenenTimeSpan Wert und angegeben[`TimeUnitType`](../timeunittype) wert. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Gibt die Seitenzahl für das zu rendernde Projekt zurück, wobei der Standardwert verwendet wird[`Timescale`](../../aspose.tasks.visualization/timescale) (Tage). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Gibt die Seitenzahl für das zu rendernde Projekt zurück, wobei der Standardwert verwendet wird[`Timescale`](../../aspose.tasks.visualization/timescale) (Tage) und gegeben[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../aspose.tasks.visualization/timescale) und[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../aspose.tasks.visualization/timescale) und[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Gibt die Seitenzahl für das zu rendernde Projekt mit der angegebenen zurück[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) und Datumsbereich. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Gibt eine Sammlung von Aufgabenverknüpfungen zurück, die Vorgänger der angegebenen Aufgabe sind. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | erhält[`Duration`](../duration) Objekt mit dem angegebenenDouble Wert und Standardarbeitsformat. |
| [Print](../../aspose.tasks/project/print#print)() | Druckt das Projekt auf dem Standarddrucker mit Standarddruckereinstellungen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Druckt das Projekt auf dem Standarddrucker mit Standarddruckereinstellungen und benutzerdefinierten Speicheroptionen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Druckt das Projekt auf dem angegebenen Drucker mit Standarddruckereinstellungen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen und benutzerdefinierten Speicheroptionen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Druckt das Projekt gemäß den angegebenen Druckereinstellungen, benutzerdefinierten Speicheroptionen und dem angegebenen Dokumentnamen unter Verwendung des Standarddruckcontrollers (ohne Benutzeroberfläche). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Endtermine neu, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Endtermine neu, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder mit optionaler Validierung. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Berechnet ID, Start und Ende der Ressourcen neu. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Berechnet Start und Ende von Ressourcen neu. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Entfernt ungültige Ressourcenzuweisungen aus der Liste der Projektressourcenzuweisungen. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | PSP-Code aller Vorgänge neu nummerieren. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | PSP-Code der bestandenen Aufgaben neu nummerieren. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Plant nicht abgeschlossene Projektarbeit neu, sodass sie nach einem bestimmten Datum beginnt. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Plant nicht abgeschlossene Arbeiten für eine bestimmte Liste von Aufgaben neu, damit sie nach einem bestimmten Datum beginnen. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Speichert die Projektdaten in die Datei im mpp-Format. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Speichert das Projekt unter Verwendung der angegebenen Speicheroptionen in einem Stream. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Speichert die Projektdaten im Stream. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Speichert das Projekt unter Verwendung der angegebenen Speicheroptionen in einem Stream. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Speichert das Dokument unter Verwendung der angegebenen Speicheroptionen im mpp-Dateiformat. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Speichert die Projektdaten in der Datei. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Speichert das Dokument unter Verwendung der angegebenen Speicheroptionen in einer Datei. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Speichert das Projekt als Vorlage in einem angegebenen Stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Speichert das Projekt als Vorlage im angegebenen Dateipfad. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Speichert das Projekt als Vorlage in einem angegebenen Stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Speichert das Projekt als Vorlage. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Speichert den Projektübersichtsbericht im Stream. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Speichert den Projektübersichtsbericht als PDF-Datei. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Speichert den Projektbericht des angegebenen Typs im angegebenen Stream. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Speichert den Projektbericht des angegebenen Typs im PDF-Format im angegebenen Dateipfad. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Sammelt rekursiv alle untergeordneten Tasks der Root-Task. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Speichert Baseline-Felder in der angegebenen Baseline für das gesamte Projekt. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Speichert Baseline-Felder in der angegebenen Baseline für die ausgewählten Aufgaben. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Legt die grundlegende Speicherzeit fest. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Aktualisiert alle Arbeiten als abgeschlossen bis zu einem bestimmten Datum für das gesamte Projekt. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Aktualisiert alle Arbeiten als abgeschlossen bis zu einem bestimmten Datum für die angegebene Aufgabenliste. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Ruft Projektdateiinformationen aus dem Stream ab. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Projektdateiinformationen aus der Datei lesen. |

### Bemerkungen

Das **Projekt** ist eine zentrale Klasse in der Aspose.Tasks-Bibliothek.

Kann man verwenden **Projekt** um eines der unterstützten Projektmanagementformate zu lesen: MPP, MPT, MPX, XML.

Um ein vorhandenes Dokument in einem der unterstützten Formate zu laden, übergeben Sie einen Dateinamen oder einen Stream an eines der **Projekt** Konstrukteure. Um ein leeres Projekt zu erstellen, rufen Sie den parameterlosen Konstruktor auf.

Verwenden Sie eine der Save-Methodenüberladungen, um das Projekt in einem der zu speichern[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) Formate: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Festes Layout: PDF; Bilder: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Sonstiges: HTML.

Verwenden Sie zum Drucken des Projekts eine der[`Print`](./print) Methodenüberladungen.

Das **Projekt** speichert projektweite Informationen wie z[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , und[`ExtendedAttributes`](./extendedattributes) . Auf die meisten dieser Objekte kann über die entsprechenden Eigenschaften des zugegriffen werden **Projekt** Klasse.

Das **Projekt** ist eine Root-Entität, die Einstiegspunkte enthält, um andere Projektentitäten zu manipulieren, wie z[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) und[`Calendar`](../calendar).

Die **Projekt** Auf Entitäten kann beispielsweise über typisierte Sammlungen zugegriffen werden[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , etc.

### Siehe auch

* namensraum [Aspose.Tasks](../../aspose.tasks)
* Montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
