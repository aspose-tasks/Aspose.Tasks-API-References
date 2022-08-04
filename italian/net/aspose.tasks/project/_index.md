---
title: Project
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Rappresenta un progetto.
type: docs
weight: 1180
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
| [Project](project#constructor)() | Inizializza una nuova istanza di[`Project`](../project) classe. |
| [Project](project#constructor_1)(DbSettings) | Inizializza una nuova istanza di[`Project`](../project) classe per leggere i dati da un database specificato dall'istanza di[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) classe. |
| [Project](project#constructor_2)(Stream) | Inizializza una nuova istanza di[`Project`](../project) classe da un flusso. |
| [Project](project#constructor_9)(StreamReader) | Inizializza una nuova istanza di[`Project`](../project) classe da un'istanza di StreamReader. |
| [Project](project#constructor_10)(string) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file mpp o mpt esistente). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Inizializza una nuova istanza di[`Project`](../project) classe da Stream con l'istanza specificata di[`LoadOptions`](../loadoptions) classe. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file mpp o mpt esistente). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Inizializza una nuova istanza di[`Project`](../project) classe da Stream con l'istanza specificata di[`PrimaveraReadOptions`](../primaverareadoptions) classe. |
| [Project](project#constructor_8)(Stream, string) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file mpp o mpt esistente). |
| [Project](project#constructor_11)(string, LoadOptions) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file mpp o mpt esistente) con l'istanza specificata di[`LoadOptions`](../loadoptions) classe. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file mpp o mpt esistente). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello (file MPP o MPT esistente) con l'istanza specificata di[`PrimaveraReadOptions`](../primaverareadoptions) classe. |
| [Project](project#constructor_16)(string, string) | Inizializza una nuova istanza di[`Project`](../project) classe da un modello protetto da password (file mpp o mpt esistente). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Ottiene la raccolta di proprietà integrate del progetto. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Ottiene o imposta la modalità di calcolo di un progetto. Può essere uno dei valori di[`CalculationMode`](./calculationmode) enumerazione. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Ottiene[`CalendarCollection`](../calendarcollection) oggetto di questa istanza del progetto. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Ottiene una raccolta che contiene un elenco di attività critiche che comprendono il percorso critico di questo progetto. Questa è un'operazione O(n), dove n è il numero di attività nel progetto. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Ottiene la raccolta di proprietà personalizzate del progetto. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Ottiene o imposta la vista predefinita del progetto. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Ottiene l'istanza di[`WeekDayCollection`](../weekdaycollection) classe che rappresenta una raccolta di giorni lavorativi settimanali e orari di lavoro predefiniti del progetto. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Ottiene un'istanza di[`ProjectDisplayOptions`](../projectdisplayoptions) classe. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La raccolta di definizioni di attributi estesi (campi personalizzati) associati a un progetto. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Ottiene una raccolta contenente le istanze di[`OleObject`](../oleobject) classe che sono collegate o incorporate in questo file di progetto. Disponibile solo per il formato file mpp. Questa raccolta è di sola lettura ad eccezione dell'operazione "Cancella". |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Ottiene l'oggetto OutlineCodeDefinitionCollection. La raccolta di definizioni del codice di struttura associate a un progetto. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Ottiene l'oggetto ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Ottiene tutte le definizioni dei filtri basati sulle risorse. ResourceFilters è una raccolta di[`Filter`](../filter) oggetti. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Ottiene tutte le definizioni dei gruppi basati sulle risorse. ResourceGroups è una raccolta di[`Group`](../group) oggetti. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Ottiene l'oggetto ResourceCollection. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Ottiene la radice dell'albero delle attività. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Ottiene un elenco di[`Table`](../table) oggetti. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Ottiene tutte le definizioni dei filtri basati sulle attività. TaskFilters è una raccolta di[`Filter`](../filter) oggetti. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Ottiene tutte le definizioni dei gruppi basati su attività. TaskGroups è una raccolta di[`Group`](../group) oggetti. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Ottiene[`TaskLinkCollection`](../tasklinkcollection) oggetto. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Ottiene un'istanza di[`VbaProject`](./vbaproject) classe. |
| [Views](../../aspose.tasks/project/views) { get; } | Ottiene un elenco di[`View`](../view) oggetti. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Ottiene o imposta la definizione del codice WBS per il progetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Copia i dati e le proprietà principali del progetto in un altro progetto. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Copia i dati e le proprietà principali del progetto in un altro progetto. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Enumera ricorsivamente tutte le attività del progetto, inclusa l'attività di root. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Restituisce il valore a cui è mappata la proprietà in questo contenitore. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Restituisce il tempo di risparmio della linea di base. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Ottiene[`Duration`](../duration) oggetto con il numero di unità specificato e il formato di durata predefinito definito nelle impostazioni del progetto[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Ottiene[`Duration`](../duration) oggetto con il numero specificato di[`TimeUnitType`](../timeunittype) unità. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Ottiene[`Duration`](../duration) oggetto con il specificatoTimeSpan valore e specificato[`TimeUnitType`](../timeunittype) valore. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../aspose.tasks.visualization/timescale) (Giorni). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Restituisce il conteggio delle pagine per il progetto di cui eseguire il rendering utilizzando l'impostazione predefinita[`Timescale`](../../aspose.tasks.visualization/timescale) (Giorni) e dato[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../aspose.tasks.visualization/timescale) e[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../aspose.tasks.visualization/timescale) e[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando dato[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) e intervallo di date. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Restituisce una raccolta di collegamenti alle attività che sono predecessori dell'attività specificata. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Ottiene[`Duration`](../duration) oggetto con il specificatoDouble valore e formato di lavoro predefinito. |
| [Print](../../aspose.tasks/project/print#print)() | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Stampa il progetto in base alle impostazioni della stampante specificate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante e le opzioni di salvataggio personalizzate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Stampa il progetto sulla stampante specificata con le impostazioni predefinite della stampante utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Stampa il progetto in base alle impostazioni della stampante specificate e alle opzioni di salvataggio personalizzate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Stampa il progetto in base alle impostazioni della stampante specificate utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Stampa il progetto in base alle impostazioni della stampante specificate, alle opzioni di salvataggio personalizzate e al nome del documento specificato utilizzando il controller di stampa standard (senza interfaccia utente). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro, di lavoro e di costo. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro e costi con la convalida opzionale. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Ricalcola ID, inizio e fine delle risorse. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Ricalcola l'inizio e la fine delle risorse. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Rinumera il codice WBS di tutte le attività. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Rinumera il codice WBS delle attività passate. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Riprogramma il lavoro del progetto non completato in modo che inizi dopo una data specificata. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Riprogramma il lavoro non completato per l'inizio di un elenco specificato di attività dopo una data specificata. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Salva i dati del progetto nel file in formato mpp. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Salva il progetto in un flusso utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Salva i dati del progetto nello stream. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Salva il progetto in un flusso utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Salva il documento in formato file MPP utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Salva i dati del progetto nel file. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Salva il documento in un file utilizzando le opzioni di salvataggio specificate. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Salva il progetto come modello in un flusso specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Salva il progetto come modello nel percorso file specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Salva il progetto come modello in un flusso specificato. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Salva il progetto come modello. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Salva il report della panoramica del progetto nello stream. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Salva il rapporto di panoramica del progetto in un file PDF. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Salva il report del progetto del tipo specificato nel flusso specificato. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Salva il report del progetto del tipo specificato in formato PDF nel percorso file specificato. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Raccoglie ricorsivamente tutte le attività figlio dell'attività radice. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mappa la proprietà specificata sul valore specificato in questo contenitore. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Mappa la proprietà specificata sul valore specificato in questo contenitore. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Salva i campi della linea di base nella linea di base specificata per l'intero progetto. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Salva i campi della linea di base nella linea di base specificata per le attività selezionate. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Imposta la linea di base per risparmiare tempo. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Aggiorna tutto funziona come completo fino a una data specificata per l'intero progetto. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Tutti gli aggiornamenti funzionano come completi fino a una data specificata per l'elenco di attività specificato. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Ottiene informazioni sul file di progetto dallo stream. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Leggi le informazioni sul file di progetto dal file. |

### Osservazioni

Il **Progetto** è una classe centrale nella libreria Aspose.Tasks.

Si può usare **Progetto** per leggere uno dei formati di gestione dei progetti supportati: MPP, MPT, MPX, XML.

Per caricare un documento esistente in uno qualsiasi dei formati supportati, passa un nome file o uno stream in uno dei file **Progetto** costruttori. Per creare un progetto vuoto, chiama il costruttore senza parametri.

Utilizzare uno degli overload del metodo Save per salvare il progetto in uno dei file[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) formati: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Layout fisso: PDF; Immagini: JPEG, PNG, BMP, TIFF, SVG; Testo: TXT; Altri: HTML.

Per stampare il progetto, utilizzare uno dei file[`Print`](./print) sovraccarichi di metodo.

Il **Progetto** memorizza informazioni a livello di progetto come[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , e[`ExtendedAttributes`](./extendedattributes) . La maggior parte di questi oggetti è accessibile tramite le proprietà corrispondenti di **Progetto** classe.

Il **Progetto** è un'entità radice che contiene punti di ingresso per manipolare altre entità di progetto, come[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) e[`Calendar`](../calendar).

Il **Progetto** è possibile accedere alle entità tramite raccolte tipizzate, ad esempio[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , ecc.

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
