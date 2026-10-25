---
title: "Classe Project"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Project. Rappresenta un progetto"
type: docs
weight: 1440
url: /it/net/aspose.tasks/project/
---
## Project class

Rappresenta un progetto.

```csharp
public class Project
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Project](project/#constructor)() | Inizializza una nuova istanza della classe `Project`. |
| [Project](project/#constructor_1)(DbSettings) | Inizializza una nuova istanza della classe `Project` per leggere i dati da un database specificato dall'istanza della classe [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/). |
| [Project](project/#constructor_2)(Stream) | Inizializza una nuova istanza della classe `Project` da uno stream. |
| [Project](project/#constructor_7)(StreamReader) | Inizializza una nuova istanza della classe `Project` da un'istanza di StreamReader. |
| [Project](project/#constructor_8)(string) | Inizializza una nuova istanza della classe `Project` da un modello (file mpp o mpt esistente). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Inizializza una nuova istanza della classe `Project` dallo Stream con l'istanza specificata della classe [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Inizializza una nuova istanza della classe `Project` da un modello (file mpp o mpt esistente). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Inizializza una nuova istanza della classe `Project` dallo Stream con l'istanza specificata della classe [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_6)(Stream, string) | Inizializza una nuova istanza della classe `Project` da un modello (file mpp o mpt esistente). |
| [Project](project/#constructor_9)(string, LoadOptions) | Inizializza una nuova istanza della classe `Project` da un modello (file mpp o mpt esistente) con l'istanza specificata della classe [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Inizializza una nuova istanza della classe `Project` da un modello (file mpp o mpt esistente). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Inizializza una nuova istanza della classe `Project` da un modello (file MPP o MPT esistente) con l'istanza specificata della classe [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_12)(string, string) | Inizializza una nuova istanza della classe `Project` da un modello protetto da password (file mpp o mpt esistente). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Ottiene o imposta un valore che indica se ActualsInSync è impostato o meno. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Ottiene o imposta un valore che indica se AdminProject è impostato o meno. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Ottiene o imposta un valore che indica se AreEditableActualCosts è impostato o meno. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Ottiene o imposta un valore di Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Ottiene o imposta un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Ottiene o imposta se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Ottiene o imposta un valore che indica se Autolink è impostato o meno. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Ottiene o imposta un valore di BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Ottiene la collezione delle proprietà incorporate del progetto. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Ottiene o imposta la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione [`CalculationMode`](./calculationmode/). |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Ottiene o imposta un valore di Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Ottiene l'oggetto [`CalendarCollection`](../calendarcollection/) di questa istanza di Project. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Ottiene o imposta un valore di Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Ottiene o imposta un valore di Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Ottiene o imposta un valore di Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Ottiene o imposta un valore di CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Ottiene una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto. Questa è un'operazione O(n), dove n è il numero di attività nel progetto. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Ottiene o imposta un valore di CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Ottiene o imposta un valore di CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Ottiene o imposta un valore di CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Ottiene o imposta un valore di CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Ottiene o imposta un valore di CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Ottiene o imposta un valore di CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Ottiene la collezione delle proprietà personalizzate del progetto. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Ottiene o imposta un valore di DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Ottiene o imposta un valore di DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Ottiene o imposta un valore di DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Ottiene o imposta un valore di DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Ottiene o imposta un valore di DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Ottiene o imposta un valore di DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Ottiene o imposta un valore di DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Ottiene o imposta un valore di DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Ottiene o imposta un valore di DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Ottiene o imposta la vista predefinita del progetto. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Ottiene l'istanza della classe [`WeekDayCollection`](../weekdaycollection/) che rappresenta una raccolta dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Ottiene un'istanza della classe [`ProjectDisplayOptions`](../projectdisplayoptions/). |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Ottiene o imposta un valore di DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Ottiene o imposta un valore di EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La raccolta delle definizioni di attributi estesi (campi personalizzati) associati a un progetto. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Ottiene o imposta un valore di ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Ottiene o imposta un valore di FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Ottiene o imposta un valore che indica se FiscalYearStart è impostato o meno. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Ottiene o imposta un valore di FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Ottiene o imposta le impostazioni di globalizzazione (specifiche della lingua) del progetto. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Ottiene o imposta un valore di Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Ottiene o imposta un valore che indica se HonorConstraints è impostato o meno. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Ottiene o imposta un valore di HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Ottiene o imposta un valore che indica se InsertedProjectsLikeSummary è impostato o meno. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Ottiene o imposta un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Ottiene o imposta un valore di Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Ottiene o imposta un valore di LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Ottiene o imposta un valore di LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Ottiene o imposta un valore di LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Ottiene o imposta un valore di Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Ottiene o imposta un valore che indica se MicrosoftProjectServerURL è impostato o meno. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Ottiene o imposta un valore di MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Ottiene o imposta un valore di MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Ottiene o imposta un valore che indica se MoveCompletedEndsBack è impostato o meno. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Ottiene o imposta un valore che indica se MoveCompletedEndsForward è impostato o meno. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Ottiene o imposta un valore che indica se MoveRemainingStartsBack è impostato o meno. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Ottiene o imposta un valore che indica se MoveRemainingStartsForward è impostato o meno. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Ottiene o imposta un valore che indica se MultipleCriticalPaths è impostato o meno. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Ottiene o imposta un valore di Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Ottiene o imposta un valore che indica se NewTasksAreManual è impostato o meno. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Ottiene o imposta un valore che indica se NewTasksEffortDriven è impostato o meno. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Ottiene o imposta un valore che indica se NewTasksEstimated è impostato o meno. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Ottiene o imposta un valore di NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Ottiene una collezione contenente le istanze della classe [`OleObject`](../oleobject/) che sono collegate o incorporate a questo file di progetto. Disponibile solo per il formato file mpp. Questa collezione è di sola lettura eccetto per l'operazione 'Clear'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Ottiene l'oggetto OutlineCodeDefinitionCollection. La collezione delle definizioni di codice di struttura associate a un progetto. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Ottiene un oggetto contenente le proprietà specifiche di Primavera per un progetto letto da un file Primavera. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Ottiene o imposta un valore che indica se ProjectExternallyEdited è impostato o meno. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Ottiene o imposta un valore che indica se RemoveFileProperties è impostato o meno. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Ottiene l'oggetto ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Ottiene tutte le definizioni di filtro basate sulle risorse. ResourceFilters è una collezione di oggetti [`Filter`](../filter/). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Ottiene tutte le definizioni di gruppo basate sulle risorse. ResourceGroups è una collezione di oggetti [`Group`](../group/). |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Ottiene l'oggetto ResourceCollection. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Ottiene o imposta un valore di Revisione. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Ottiene la radice dell'albero delle attività. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Ottiene o imposta un valore di SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Ottiene o imposta un valore che indica se ScheduleFromStart è impostato o meno. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Ottiene o imposta un valore che indica se ShowProjectSummaryTask è impostato o meno. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Ottiene o imposta un valore che indica se SplitsInProgressTasks è impostato o meno. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Ottiene o imposta un valore che indica se SpreadActualCost è impostato o meno. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Ottiene o imposta un valore che indica se SpreadPercentComplete è impostato o meno. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Ottiene o imposta un valore di StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Ottiene o imposta un valore di StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Ottiene o imposta un valore di Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Ottiene un elenco di oggetti [`Table`](../table/). |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Ottiene tutte le definizioni di filtro basate sulle attività. TaskFilters è una raccolta di oggetti [`Filter`](../filter/). |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Ottiene tutte le definizioni di gruppo basate sulle attività. TaskGroups è una raccolta di oggetti [`Group`](../group/). |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Ottiene l'oggetto [`TaskLinkCollection`](../tasklinkcollection/). |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Ottiene o imposta un valore che indica se TaskUpdatesResource è impostato o meno. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Ottiene o imposta un valore di Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Ottiene o imposta un valore di TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Ottiene o imposta un valore di TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Ottiene o imposta un valore di Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Ottiene o imposta un valore di Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Ottiene o imposta un valore che indica se UpdateManuallyScheduledTasksWhenEditingLinks è impostato o meno. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Ottiene un'istanza della classe [`VbaProject`](./vbaproject/). |
| [Views](../../aspose.tasks/project/views/) { get; } | Ottiene un elenco di oggetti [`View`](../view/). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Ottiene o imposta la definizione del codice WBS per il progetto. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Ottiene o imposta un valore di WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Ottiene o imposta un valore di WorkFormat. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Copia i dati principali e le proprietà del progetto in un altro progetto. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Copia i dati principali e le proprietà del progetto in un altro progetto. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Enumera ricorsivamente tutte le attività del progetto, inclusa l'attività radice. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Restituisce il tempo di salvataggio della baseline. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Ottiene l'oggetto [`Duration`](../duration/) con il numero specificato di unità e il formato di durata predefinito, definito nelle impostazioni del progetto [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Ottiene l'oggetto [`Duration`](../duration/) con il numero specificato di unità [`TimeUnitType`](../timeunittype/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Ottiene l'oggetto [`Duration`](../duration/) con il valore TimeSpan specificato e il valore [`TimeUnitType`](../timeunittype/) specificato. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/) predefinito (Giorni). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/) predefinito (Giorni) e il [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) fornito. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando le [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) specificate. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/) specificato. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/) e la [`PageSize`](../../aspose.tasks.visualization/pagesize/) specificati. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/) e il [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) specificati. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando il [`Timescale`](../../aspose.tasks.visualization/timescale/), il [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) e l'intervallo di date. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Restituisce una raccolta di collegamenti di attività che sono predecessori dell'attività specificata. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Ottiene l'oggetto [`Duration`](../duration/) con il valore Double specificato e il formato di lavoro predefinito. |
| [Print](../../aspose.tasks/project/print/#print)() | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Stampa il progetto secondo le impostazioni della stampante specificate usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante e opzioni di salvataggio personalizzate usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Stampa il progetto sulla stampante specificata con le impostazioni predefinite della stampante usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Stampa il progetto secondo le impostazioni della stampante specificate e opzioni di salvataggio personalizzate usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Stampa il progetto secondo le impostazioni della stampante specificate usando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Stampa il progetto secondo le impostazioni della stampante specificate, opzioni di salvataggio personalizzate e il nome del documento specificato usando il controller di stampa standard (senza interfaccia utente). |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo con convalida opzionale. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Ricalcola ID, Inizio e Fine delle risorse. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Rinumerare il codice WBS di tutte le attività. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Rinumerare il codice WBS delle attività superate. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Riprogramma il lavoro di progetto non completato per iniziare dopo una data specificata. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Riprogramma il lavoro non completato per un elenco specificato di attività per iniziare dopo una data specificata. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Salva i dati del progetto nel file in formato mpp. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Salva i dati del progetto nello stream. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Salva il progetto in uno stream utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Salva i dati del progetto nel file. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Salva il documento in un file utilizzando le opzioni di salvataggio specificate. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Salva il progetto come modello in uno stream specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Salva il progetto come modello nel percorso file specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Salva il progetto come modello in uno stream specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Salva il progetto come modello. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Salva il report di panoramica del progetto nello stream. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Salva il report di panoramica del progetto in un file PDF. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Salva il report del progetto del tipo specificato nello stream specificato. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Salva il report del progetto del tipo specificato in formato PDF nel percorso file specificato. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Raccoglie ricorsivamente tutte le attività figlio dell'attività radice. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Salva i campi di baseline nella baseline specificata per l'intero progetto. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Salva i campi di baseline nella baseline specificata per le attività selezionate. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Imposta l'ora di salvataggio della baseline. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Aggiorna tutto il lavoro come completato fino a una data specificata per l'elenco specificato di attività. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Ottiene le informazioni del file di progetto dallo stream. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Legge le informazioni del file di progetto dal file. |

## Osservazioni

Il **Project** è una classe centrale nella libreria Aspose.Tasks.

È possibile utilizzare **Project** per leggere uno dei formati di gestione progetti supportati: MPP, MPT, MPX, XML.

Per caricare un documento esistente in uno dei formati supportati, passare un nome file o uno stream a uno dei costruttori di **Project**. Per creare un progetto vuoto, chiamare il costruttore senza parametri.

Utilizzare una delle sovraccariche del metodo Save per salvare il progetto in uno dei formati [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Layout fisso: PDF; Immagini: JPEG, PNG, BMP, TIFF, SVG; Testo: TXT; Altri: HTML.

Il **Project** memorizza informazioni a livello di progetto come [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/) e [`ExtendedAttributes`](./extendedattributes/). La maggior parte di questi oggetti è accessibile tramite le proprietà corrispondenti della classe **Project**.

Il **Project** è un'entità radice che contiene punti di ingresso per manipolare altre entità del progetto, come [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) e [`Calendar`](../calendar/).

Le entità **Project** possono essere accessibili tramite collezioni tipizzate, ad esempio [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), ecc.

## Esempi

Mostra come lavorare con un'istanza &lt;see cref=\"Aspose.Tasks.Project\"/&gt;.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// aggiungere nuovi task e impostare le proprietà desiderate
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// aggiungere nuove risorse
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// aggiungere nuove assegnazioni di risorse
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// salvare il progetto in uno dei formati disponibili
// qui lo stiamo salvando nel formato file Microsoft Project XML.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


