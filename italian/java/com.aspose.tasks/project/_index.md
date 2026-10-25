---
title: "Progetto"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un progetto."
type: docs
weight: 220
url: /it/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Rappresenta un progetto.

--------------------

La **Project** è una classe centrale nella libreria Aspose.Tasks.

È possibile utilizzare **Project** per leggere uno dei formati di gestione progetti supportati: MPP, MPT, MPX, XML.

Per caricare un documento esistente in uno dei formati supportati, passare un nome file o uno stream a uno dei costruttori **Project**. Per creare un progetto vuoto, chiamare il costruttore senza parametri.

Utilizzare una delle sovraccariche del metodo Save per salvare il progetto in uno dei formati [SaveFileFormat](../../com.aspose.tasks/savefileformat): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Layout fisso: PDF; Immagini: JPEG, PNG, BMP, TIFF, SVG; Testo: TXT; Altri: HTML.

Per stampare il progetto, utilizzare una delle sovraccariche del metodo [print()](../../com.aspose.tasks/project\#print--).

Il **Project** memorizza informazioni a livello di progetto come `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), e `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). La maggior parte di questi oggetti è accessibile tramite le proprietà corrispondenti della classe **Project**.

Il **Project** è un'entità radice che contiene punti di ingresso per manipolare altre entità del progetto, come [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) e [Calendar](../../com.aspose.tasks/calendar).

Le entità **Project** possono essere accessibili tramite collezioni tipizzate, ad esempio `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), ecc.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Project()](#Project--) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello protetto da password (file mpp o mpt esistente). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) dallo Stream con la specifica istanza della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da uno stream. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file MPP o MPT esistente) con la specifica istanza della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) per leggere i dati da un database specificato dall'istanza della classe [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente) con l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) dallo Stream con l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Copia i dati principali e le proprietà del progetto in un altro progetto. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Copia i dati principali e le proprietà del progetto in un altro progetto. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Enumera ricorsivamente tutte le attività del progetto, inclusa l'attività radice. |
| [getActualsInSync()](#getActualsInSync--) | Restituisce un valore che indica se ActualsInSync è impostato o meno. |
| [getAdminProject()](#getAdminProject--) | Restituisce un valore che indica se AdminProject è impostato o meno. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Restituisce un valore che indica se AreEditableActualCosts è impostato o meno. |
| [getAuthor()](#getAuthor--) | Restituisce il valore di Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Restituisce un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Restituisce se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [getAutolink()](#getAutolink--) | Restituisce un valore che indica se Autolink è impostato o meno. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Restituisce il valore di BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Restituisce il tempo di salvataggio della baseline. |
| [getBuiltInProps()](#getBuiltInProps--) | Restituisce la collezione delle proprietà integrate del progetto. |
| [getCalculationMode()](#getCalculationMode--) | Restituisce la modalità di calcolo di un progetto. |
| [getCalendar()](#getCalendar--) | Ottiene un valore di Calendar. |
| [getCalendars()](#getCalendars--) | Restituisce l'oggetto [CalendarCollection](../../com.aspose.tasks/calendarcollection) di questa istanza di Project. |
| [getCategory()](#getCategory--) | Restituisce il valore di Category. |
| [getComments()](#getComments--) | Restituisce il valore di Comments. |
| [getCompany()](#getCompany--) | Restituisce il valore di Company. |
| [getCreationDate()](#getCreationDate--) | Restituisce il valore di CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | Restituisce una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni. |
| [getCurrencyCode()](#getCurrencyCode--) | Restituisce il valore di CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Ottiene un valore di CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Ottiene un valore di CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Ottiene un valore di CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Ottiene un valore di CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Ottiene un valore di CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Ottiene la collezione delle proprietà personalizzate del progetto. |
| [getDateFormat()](#getDateFormat--) | Ottiene un valore di DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Ottiene un valore di DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Ottiene un valore di DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Ottiene un valore di DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Ottiene un valore di DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Ottiene un valore di DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Ottiene un valore di DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Ottiene un valore di DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Ottiene un valore di DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Ottiene la vista predefinita del progetto. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Ottiene l'istanza della classe [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) che rappresenta una collezione dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro. |
| [getDisplayOptions()](#getDisplayOptions--) | Ottiene un'istanza della classe [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Ottiene l'oggetto [Duration](../../com.aspose.tasks/duration) con il numero specificato di unità e il formato di durata predefinito, definito nelle impostazioni del progetto [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Ottiene l'oggetto [Duration](../../com.aspose.tasks/duration) con il numero specificato di unità di [TimeUnitType](../../com.aspose.tasks/timeunittype). |
| [getDurationFormat()](#getDurationFormat--) | Ottiene un valore di DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Ottiene un valore di EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Ottiene l'oggetto ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Ottiene un valore di ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Ottiene un valore di FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Ottiene un valore che indica se FiscalYearStart è impostato o meno. |
| [getFyStartDate()](#getFyStartDate--) | Ottiene un valore di FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Ottiene le impostazioni di globalizzazione (specifiche della lingua) del progetto. |
| [getGuid()](#getGuid--) | Ottiene un valore di Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Ottiene un valore che indica se HonorConstraints è impostato o meno. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Ottiene un valore di HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Ottiene un valore che indica se InsertedProjectsLikeSummary è impostato o meno. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Ottiene un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno. |
| [getKeywords()](#getKeywords--) | Ottiene un valore di Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Ottiene un valore di LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Ottiene un valore di LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Ottiene un valore di LastSaved. |
| [getManager()](#getManager--) | Ottiene un valore di Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Ottiene un valore che indica se MicrosoftProjectServerURL è impostato o meno. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Ottiene un valore di MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Ottiene un valore di MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Ottiene un valore che indica se MoveCompletedEndsBack è impostato o meno. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Ottiene un valore che indica se MoveCompletedEndsForward è impostato o meno. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Ottiene un valore che indica se MoveRemainingStartsBack è impostato o meno. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Ottiene un valore che indica se MoveRemainingStartsForward è impostato o meno. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Ottiene un valore che indica se MultipleCriticalPaths è impostato o meno. |
| [getName()](#getName--) | Ottiene un valore di Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Ottiene un valore di NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Ottiene un valore che indica se NewTasksAreManual è impostato o meno. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Ottiene un valore che indica se NewTasksEffortDriven è impostato o meno. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Ottiene un valore che indica se NewTasksEstimated è impostato o meno. |
| [getOleObjects()](#getOleObjects--) | Ottiene una collezione contenente le istanze della classe [OleObject](../../com.aspose/tasks/oleobject) che sono collegate o incorporate in questo file di progetto. |
| [getOutlineCodes()](#getOutlineCodes--) | Ottiene l'oggetto OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) predefinito (Giorni). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Restituisce il conteggio delle pagine per il progetto da rendere usando le [SaveOptions](../../com.aspose.tasks/saveoptions) fornite. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) e il [PresentationFormat](../../com.aspose.tasks/presentationformat) forniti. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) e il [PageSize](../../com.aspose.tasks/pagesize) forniti. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale), il [PresentationFormat](../../com.aspose.tasks/presentationformat) e l'intervallo di date forniti. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) predefinito (Giorni) e il [PresentationFormat](../../com.aspose.tasks/presentationformat) fornito. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) fornito. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Restituisce una raccolta di collegamenti di attività che sono predecessori dell'attività specificata. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Ottiene un oggetto contenente proprietà specifiche di Primavera per un progetto letto dal file Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Ottiene un valore che indica se ProjectExternallyEdited è impostato o meno. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Ottiene le informazioni del file di progetto dallo stream. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Legge le informazioni del file di progetto dal file. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Ottiene un valore che indica se RemoveFileProperties è impostato o meno. |
| [getResourceAssignments()](#getResourceAssignments--) | Ottiene l'oggetto ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | Ottiene tutte le definizioni di filtro basate sulle risorse. |
| [getResourceGroups()](#getResourceGroups--) | Ottiene tutte le definizioni di gruppo basate sulle risorse. |
| [getResources()](#getResources--) | Ottiene l'oggetto ResourceCollection. |
| [getRevision()](#getRevision--) | Ottiene un valore di Revision. |
| [getRootTask()](#getRootTask--) | Ottiene la radice dell'albero delle attività. |
| [getSaveVersion()](#getSaveVersion--) | Ottiene un valore di SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Ottiene un valore che indica se ScheduleFromStart è impostato o meno. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Ottiene un valore che indica se ShowProjectSummaryTask è impostato o meno. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Ottiene un valore che indica se SplitsInProgressTasks è impostato o meno. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Ottiene un valore che indica se SpreadActualCost è impostato o meno. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Restituisce un valore che indica se SpreadPercentComplete è impostato o meno. |
| [getStartDate()](#getStartDate--) | Restituisce un valore di StartDate. |
| [getStatusDate()](#getStatusDate--) | Restituisce un valore di StatusDate. |
| [getSubject()](#getSubject--) | Restituisce un valore di Subject. |
| [getTables()](#getTables--) | Restituisce un elenco di oggetti [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | Restituisce tutte le definizioni di filtro basate sui task. |
| [getTaskGroups()](#getTaskGroups--) | Restituisce tutte le definizioni di gruppo basate sui task. |
| [getTaskLinks()](#getTaskLinks--) | Restituisce l'oggetto [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Restituisce un valore che indica se TaskUpdatesResource è impostato o meno. |
| [getTemplate()](#getTemplate--) | Restituisce un valore di Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Restituisce un valore di TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Restituisce un valore di TimescaleStart. |
| [getTitle()](#getTitle--) | Restituisce un valore di Title. |
| [getUid()](#getUid--) | Ottiene un valore di Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Restituisce un valore che indica se UpdateManuallyScheduledTasksWhenEditingLinks è impostato o meno. |
| [getVbaProject()](#getVbaProject--) | Restituisce un'istanza della classe `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | Restituisce un elenco di oggetti [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Restituisce la definizione del codice WBS per il progetto. |
| [getWeekStartDay()](#getWeekStartDay--) | Restituisce un valore di WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Restituisce l'oggetto [Duration](../../com.aspose.tasks/duration) con il valore `double` specificato e il formato di lavoro predefinito. |
| [getWorkFormat()](#getWorkFormat--) | Restituisce un valore di WorkFormat. |
| [print()](#print--) | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante e opzioni di salvataggio personalizzate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Stampa il progetto secondo le impostazioni della stampante specificate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Stampa il progetto secondo le impostazioni della stampante specificate e opzioni di salvataggio personalizzate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Stampa il progetto secondo le impostazioni della stampante specificate, opzioni di salvataggio personalizzate e il nome del documento specificato utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Stampa il progetto secondo le impostazioni della stampante specificate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [print(String printerName)](#print-java.lang.String-) | Stampa il progetto sulla stampante specificata con le impostazioni predefinite della stampante utilizzando il controller di stampa standard (senza interfaccia utente). |
| [recalculate()](#recalculate--) | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, il lavoro e i campi di costo. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, il lavoro e i campi di costo con convalida opzionale. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Ricalcola ID, Inizio e Fine delle risorse. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Ricalcola Inizio e Fine delle risorse. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto. |
| [renumberWBSCode()](#renumberWBSCode--) | Rinumerare il codice WBS di tutte le attività. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Rinumerare il codice WBS delle attività passate. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Riprogramma il lavoro del progetto non completato per iniziare dopo una data specificata. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Riprogramma il lavoro non completato per un elenco specificato di attività per iniziare dopo una data specificata. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Salva il progetto in uno stream utilizzando le opzioni di salvataggio specificate. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Salva i dati del progetto nello stream. |
| [save(String filename)](#save-java.lang.String-) | Salva i dati del progetto nel file in formato mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Salva il documento in un file utilizzando le opzioni di salvataggio specificate. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Salva i dati del progetto nel file. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Salva il progetto come modello in uno stream specificato. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Salva il progetto come modello in uno stream specificato. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Salva il progetto come modello nel percorso file specificato. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Salva il progetto come modello. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Salva il report di panoramica del progetto nello stream. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Salva il report del progetto del tipo specificato nello stream specificato. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Salva il report di panoramica del progetto in un file PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Salva il report del progetto del tipo specificato in formato PDF nel percorso file specificato. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Raccoglie ricorsivamente tutte le attività figlie dell'attività radice. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se ActualsInSync è impostato o meno. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se AdminProject è impostato o meno. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se AreEditableActualCosts è impostato o meno. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta un valore per Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Imposta se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se Autolink è impostato o meno. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Salva i campi di baseline nella baseline specificata per l'intero progetto. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Salva i campi di baseline nella baseline specificata per le attività selezionate. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Imposta un valore per BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Imposta il tempo di salvataggio della baseline. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Imposta la modalità di calcolo di un progetto. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Imposta un valore di Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Imposta un valore per Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Imposta un valore per Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Imposta un valore per Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Imposta un valore per CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Imposta un valore per CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Imposta un valore per CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Imposta un valore per CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Imposta un valore per CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Imposta un valore per CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Imposta un valore per CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Imposta un valore per DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Imposta un valore per DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Imposta un valore per DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Imposta un valore per DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Imposta un valore per DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Imposta un valore di DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Imposta un valore di DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Imposta un valore di DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Imposta un valore di DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Imposta la visualizzazione predefinita del progetto. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Imposta un valore di DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Imposta un valore di EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Imposta un valore di ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Imposta un valore di FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se FiscalYearStart è impostato o meno. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Imposta un valore di FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Imposta le impostazioni di globalizzazione (specifiche della lingua) del progetto. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Imposta un valore di Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se HonorConstraints è impostato o meno. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Imposta un valore di HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se InsertedProjectsLikeSummary è impostato o meno. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Imposta un valore di Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Imposta un valore di LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Imposta un valore di LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Imposta un valore di LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Imposta un valore di Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MicrosoftProjectServerURL è impostato o meno. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Imposta un valore di MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Imposta un valore di MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MoveCompletedEndsBack è impostato o meno. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MoveCompletedEndsForward è impostato o meno. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MoveRemainingStartsBack è impostato o meno. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MoveRemainingStartsForward è impostato o meno. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se MultipleCriticalPaths è impostato o meno. |
| [setName(String value)](#setName-java.lang.String-) | Imposta un valore di Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Imposta un valore di NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se NewTasksAreManual è impostato o meno. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se NewTasksEffortDriven è impostato o meno. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se NewTasksEstimated è impostato o meno. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se ProjectExternallyEdited è impostato o meno. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se RemoveFileProperties è impostato o meno. |
| [setRevision(int value)](#setRevision-int-) | Imposta un valore di Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Imposta un valore di SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se ScheduleFromStart è impostato o meno. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Imposta un valore che indica se ShowProjectSummaryTask è impostato o meno. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se SplitsInProgressTasks è impostato o meno. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se SpreadActualCost è impostato o meno. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se SpreadPercentComplete è impostato o meno. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Imposta un valore di StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Imposta un valore di StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Imposta un valore di Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se TaskUpdatesResource è impostato o meno. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Imposta un valore di Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Imposta un valore di TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Imposta un valore di TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Imposta un valore di Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Imposta un valore di Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se UpdateManuallyScheduledTasksWhenEditingLinks è impostato o meno. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Imposta la definizione del codice WBS per il progetto. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Imposta un valore per WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Imposta un valore per WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Aggiorna tutto il lavoro come completato fino a una data specificata per l'elenco specificato di attività. |
### Project() {#Project--}
```
public Project()
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello protetto da password (file mpp o mpt esistente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | java.lang.String | Percorso al modello da cui creare il progetto. |
|  | protectionPassword | java.lang.String | Password di protezione. |

--------------------

La lettura di file protetti da password è attualmente supportata solo per il formato file MSP 2003. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | java.lang.String | Percorso al modello da cui creare il progetto. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) dallo Stream con la specifica istanza della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Stream del progetto java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | l'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) che consente di personalizzare la lettura dei formati Primavera (XER o XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | java.lang.String | Percorso al modello da cui creare il progetto. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | il metodo di callback specificato per gestire gli errori di parsing XML. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream da cui caricare un modello. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file MPP o MPT esistente) con la specifica istanza della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | java.lang.String | Percorso al modello da cui creare il progetto |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | l'istanza specificata della classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) per leggere i dati da un database specificato dall'istanza della classe [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | l'istanza specificata della classe [DbSettings](../../com.aspose.tasks/dbsettings). |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream da cui caricare un modello. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | il metodo di callback specificato per gestire gli errori di parsing XML. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream da cui caricare un modello. |
|  | protectionPassword | java.lang.String | Password di protezione. |

--------------------

La lettura di file protetti da password è attualmente supportata solo per il formato file MSP 2003. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) da un modello (file mpp o mpt esistente) con l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | java.lang.String | Percorso al modello da cui creare il progetto |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions). |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Inizializza una nuova istanza della classe [Project](../../com.aspose.tasks/project) dallo Stream con l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Stream del progetto java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | l'istanza specificata della classe [LoadOptions](../../com.aspose.tasks/loadoptions) |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Restituisce il valore a cui la proprietà è mappata in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Prj](../../com.aspose.tasks/prj) per ottenere la chiave della proprietà. |

**Returns:**
T - il valore a cui la proprietà è mappata in questo contenitore.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappa la proprietà specificata al valore specificato in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Prj](../../com.aspose.tasks/prj) per ottenere la chiave della proprietà. |
| val | T | il valore. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Copia i dati principali e le proprietà del progetto in un altro progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Un altro progetto a cui copiare i dati. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Copia i dati principali e le proprietà del progetto in un altro progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Un altro progetto a cui copiare i dati. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Opzioni di copia per controllare il processo di copia. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Enumera ricorsivamente tutte le attività del progetto, inclusa l'attività radice.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable che può essere usato per iterare su tutte le attività del progetto.

--------------------

Fornisce un modo più leggero per iterare sulle attività rispetto al metodo [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) poiché non alloca memoria per tutte le attività.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Restituisce un valore che indica se ActualsInSync è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Restituisce un valore che indica se AdminProject è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Restituisce un valore che indica se AreEditableActualCosts è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Restituisce il valore di Author.

**Returns:**
java.lang.String - un valore di Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Restituisce un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Restituisce se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse.

**Returns:**
boolean - se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Restituisce un valore che indica se Autolink è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Restituisce il valore di BaselineForEarnedValue.

**Returns:**
int - un valore di BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Restituisce l'ora di salvataggio della baseline. Restituisce DateTime.MinValue (00:00:00.0000000 UTC, 1° gennaio 0001) se la baseline non è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baselineNumber | int | Il numero della baseline [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - L'ultima data e ora di salvataggio della baseline.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Restituisce la collezione delle proprietà integrate del progetto.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Ottiene la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - modalità di calcolo di un progetto.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Ottiene un valore di Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Restituisce l'oggetto [CalendarCollection](../../com.aspose.tasks/calendarcollection) di questa istanza di Project.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Restituisce il valore di Category.

**Returns:**
java.lang.String - un valore di Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Restituisce il valore di Comments.

**Returns:**
java.lang.String - un valore di Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Restituisce il valore di Company.

**Returns:**
java.lang.String - un valore di Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Restituisce il valore di CreationDate.

**Returns:**
java.util.Date - un valore di CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Restituisce una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Questa è un'operazione O(n), dove n è il numero di attività nel progetto.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni.

**Returns:**
int - il valore massimo di tempo di slittamento totale (in giorni) al quale un'attività è considerata critica
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Restituisce il valore di CurrencyCode.

**Returns:**
java.lang.String - un valore di CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Ottiene un valore di CurrencyDigits.

**Returns:**
int - un valore di CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Ottiene un valore di CurrencySymbol.

**Returns:**
java.lang.String - un valore di CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Ottiene un valore di CurrencySymbolPosition.

**Returns:**
int - un valore di CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Ottiene un valore di CurrentDate.

**Returns:**
java.util.Date - un valore di CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Ottiene un valore di CustomDateFormat.

**Returns:**
java.lang.String - un valore di CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Ottiene la collezione delle proprietà personalizzate del progetto.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Ottiene un valore di DateFormat.

**Returns:**
int - un valore di DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Ottiene un valore di DaysPerMonth.

**Returns:**
int - un valore di DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Ottiene un valore di DefaultFinishTime.

**Returns:**
java.util.Date - un valore di DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Ottiene un valore di DefaultFixedCostAccrual.

**Returns:**
int - un valore di DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Ottiene un valore di DefaultOvertimeRate.

**Returns:**
double - un valore di DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Ottiene un valore di DefaultStandardRate.

**Returns:**
double - un valore di DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Ottiene un valore di DefaultStartTime.

**Returns:**
java.util.Date - un valore di DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Ottiene un valore di DefaultTaskEVMethod.

**Returns:**
int - un valore di DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Ottiene un valore di DefaultTaskType.

**Returns:**
int - un valore di DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Ottiene la vista predefinita del progetto.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Ottiene l'istanza della classe [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) che rappresenta una collezione dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

I dati sono presenti solo nei file mpp (non in xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Ottiene un'istanza della classe [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Ottiene l'oggetto [Duration](../../com.aspose.tasks/duration) con il numero specificato di unità e il formato di durata predefinito, definito nelle impostazioni del progetto [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | val | double | numero specificato di unità. |

--------------------

Questo metodo dovrebbe essere usato con cautela perché restituisce durate diverse a seconda dell'impostazione Project.DurationFormat. Per esempio, GetWork(1.0) restituirà 1 ora quando Project.DurationFormat è TimeUnitType.Hour o 1 giorno se Project.DurationFormat è TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Ottiene l'oggetto [Duration](../../com.aspose.tasks/duration) con il numero specificato di unità di [TimeUnitType](../../com.aspose.tasks/timeunittype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | double | numero specificato di unità. |
| timeUnit | byte | valore specificato di TimeUnitType. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Ottiene un valore di DurationFormat.

**Returns:**
byte - un valore di DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Ottiene un valore di EarnedValueMethod.

**Returns:**
int - un valore di EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La raccolta delle definizioni di attributi estesi (campi personalizzati) associati a un progetto.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Ottiene un valore di ExtendedCreationDate.

**Returns:**
java.util.Date - un valore di ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Ottiene un valore di FinishDate.

**Returns:**
java.util.Date - un valore di FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Ottiene un valore che indica se FiscalYearStart è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Ottiene un valore di FyStartDate.

**Returns:**
int - un valore di FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Ottiene le impostazioni di globalizzazione (specifiche della lingua) del progetto.

Il modo consigliato è utilizzare costanti o formati indipendenti dalla cultura in tutto il progetto. Tuttavia, se un progetto utilizza costanti specifiche della cultura, questa classe può essere usata per aiutare il motore di calcolo a interpretare tali costanti.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Ottiene un valore di Guid.

**Returns:**
java.util.UUID - un valore di Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Ottiene un valore che indica se HonorConstraints è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Ottiene un valore di HyperlinkBase.

**Returns:**
java.lang.String - un valore di HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Ottiene un valore che indica se InsertedProjectsLikeSummary è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Ottiene un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Ottiene un valore di Keywords.

**Returns:**
java.lang.String - un valore di Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Ottiene un valore di LastAuthor.

**Returns:**
java.lang.String - un valore di LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Ottiene un valore di LastPrinted.

**Returns:**
java.util.Date - un valore di LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Ottiene un valore di LastSaved.

**Returns:**
java.util.Date - un valore di LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Ottiene un valore di Manager.

**Returns:**
java.lang.String - un valore di Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Ottiene un valore che indica se MicrosoftProjectServerURL è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Ottiene un valore di MinutesPerDay.

**Returns:**
int - un valore di MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Ottiene un valore di MinutesPerWeek.

**Returns:**
int - un valore di MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Ottiene un valore che indica se MoveCompletedEndsBack è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Ottiene un valore che indica se MoveCompletedEndsForward è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Ottiene un valore che indica se MoveRemainingStartsBack è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Ottiene un valore che indica se MoveRemainingStartsForward è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Ottiene un valore che indica se MultipleCriticalPaths è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Ottiene un valore di Name.

**Returns:**
java.lang.String - un valore di Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Ottiene un valore di NewTaskStartDate.

**Returns:**
int - un valore di NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Ottiene un valore che indica se NewTasksAreManual è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Ottiene un valore che indica se NewTasksEffortDriven è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Ottiene un valore che indica se NewTasksEstimated è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Ottiene una collezione contenente le istanze della classe [OleObject](../../com.aspose/tasks/oleobject) che sono collegate o incorporate in questo file di progetto.

--------------------

Disponibile solo per il formato file mpp. Questa collezione è di sola lettura eccetto l'operazione 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Restituisce l'oggetto OutlineCodeDefinitionCollection. La collezione di definizioni di codici di outline associate a un progetto.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Restituisce il conteggio delle pagine per il progetto da rendere usando il [Timescale](../../com.aspose.tasks/timescale) predefinito (Giorni).

**Returns:**
int - Numero di pagine da renderizzare.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Restituisce il conteggio delle pagine per il progetto da rendere usando le [SaveOptions](../../com.aspose.tasks/saveoptions) fornite.

--------------------

&gt; ```
&gt; In questo esempio l'istanza di HtmlSaveOptions e il numero di pagine nell'HTML risultante vengono scritti sulla console.
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

