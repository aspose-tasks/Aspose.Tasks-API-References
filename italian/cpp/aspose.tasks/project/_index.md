---
title: "Classe Aspose::Tasks::Project"
linktitle: "Progetto"
articleTitle: "Progetto"
second_title: "Aspose.Tasks per C++"
description: "Rappresenta un progetto."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/project/
---

## Project class

Rappresenta un progetto.

Il Progetto è una classe centrale nella libreria Aspose.Tasks.

È possibile utilizzare Project per leggere uno dei formati di gestione progetti supportati: MPP, MPT, MPX, XML.

Per caricare un documento esistente in uno dei formati supportati, passare un nome file o uno stream a uno dei costruttori di Project. Per creare un progetto vuoto, chiamare il costruttore senza parametri.

Utilizzare una delle sovraccariche del metodo Save per salvare il progetto in uno dei formati Aspose::Tasks::Saving::SaveFileFormat: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Layout fisso: PDF; Immagini: JPEG, PNG, BMP, TIFF, SVG; Testo: TXT; Altri: HTML.

Il Project memorizza informazioni a livello di progetto come Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps e Aspose::Tasks::Project::ExtendedAttributes. La maggior parte di questi oggetti è accessibile tramite le proprietà corrispondenti della classe Project.

Il Project è un'entità radice che contiene punti di ingresso per manipolare altre entità del progetto, come Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute e Aspose::Tasks::Calendar.

Le entità Project possono essere accessibili tramite collezioni tipizzate, ad esempio Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments, ecc.

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Project (13 overloads)](./project/) | Inizializza una nuova istanza della classe Project. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Copia i dati principali e le proprietà del progetto in un altro progetto. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Enumera ricorsivamente tutte le attività del progetto, inclusa l'attività radice. |
| [Get](./get/) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [get_ActualsInSync](./get_actualsinsync/) | Restituisce un valore che indica se ActualsInSync è impostato o meno. |
| [get_AdminProject](./get_adminproject/) | Restituisce un valore che indica se AdminProject è impostato o meno. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Restituisce un valore che indica se AreEditableActualCosts è impostato o meno. |
| [get_Author](./get_author/) | Restituisce il valore di Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Restituisce un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Restituisce se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [get_Autolink](./get_autolink/) | Restituisce un valore che indica se Autolink è impostato o meno. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Restituisce il valore di BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Restituisce la collezione delle proprietà integrate del progetto. |
| [get_CalculationMode](./get_calculationmode/) | Restituisce la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione CalculationMode. |
| [get_Calendar](./get_calendar/) | Ottiene un valore di Calendar. |
| [get_Calendars](./get_calendars/) | Restituisce l'oggetto CalendarCollection di questa istanza di Project. |
| [get_Category](./get_category/) | Restituisce il valore di Category. |
| [get_Comments](./get_comments/) | Restituisce il valore di Comments. |
| [get_Company](./get_company/) | Restituisce il valore di Company. |
| [get_CreationDate](./get_creationdate/) | Restituisce il valore di CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Restituisce una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Ottiene un valore di CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Ottiene un valore di CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Ottiene un valore di CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Ottiene un valore di CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Ottiene un valore di CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Ottiene un valore di CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Ottiene un valore di CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Ottiene la collezione delle proprietà personalizzate del progetto. |
| [get_DateFormat](./get_dateformat/) | Ottiene un valore di DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Ottiene un valore di DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Ottiene un valore di DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Ottiene un valore di DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Ottiene un valore di DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Ottiene un valore di DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Ottiene un valore di DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Ottiene un valore di DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Ottiene un valore di DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Ottiene la vista predefinita del progetto. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Ottiene l'istanza della classe WeekDayCollection che rappresenta una collezione dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro. |
| [get_DisplayOptions](./get_displayoptions/) | Ottiene un'istanza della classe ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Ottiene un valore di DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Ottiene un valore di EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La collezione delle definizioni di attributi estesi (campi personalizzati) associate a un progetto. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Ottiene un valore di ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Ottiene un valore di FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Ottiene un valore che indica se FiscalYearStart è impostato o meno. |
| [get_FyStartDate](./get_fystartdate/) | Ottiene un valore di FyStartDate. |
| [get_Guid](./get_guid/) | Ottiene un valore di Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Ottiene un valore che indica se HonorConstraints è impostato o meno. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Ottiene un valore di HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Ottiene un valore che indica se InsertedProjectsLikeSummary è impostato o meno. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Ottiene un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno. |
| [get_Keywords](./get_keywords/) | Ottiene un valore di Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Ottiene un valore di LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Ottiene un valore di LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Ottiene un valore di LastSaved. |
| [get_Manager](./get_manager/) | Ottiene un valore di Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Ottiene un valore che indica se MicrosoftProjectServerURL è impostato o meno. |
| [get_MinutesPerDay](./get_minutesperday/) | Ottiene un valore di MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Ottiene un valore di MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Ottiene un valore che indica se MoveCompletedEndsBack è impostato o meno. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Ottiene un valore che indica se MoveCompletedEndsForward è impostato o meno. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Ottiene un valore che indica se MoveRemainingStartsBack è impostato o meno. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Ottiene un valore che indica se MoveRemainingStartsForward è impostato o meno. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Ottiene un valore che indica se MultipleCriticalPaths è impostato o meno. |
| [get_Name](./get_name/) | Ottiene un valore di Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Ottiene un valore che indica se NewTasksAreManual è impostato o meno. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Ottiene un valore che indica se NewTasksEffortDriven è impostato o meno. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Ottiene un valore che indica se NewTasksEstimated è impostato o meno. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Ottiene un valore di NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Ottiene una collezione contenente le istanze della classe OleObject che sono collegate o incorporate in questo file di progetto. |
| [get_OutlineCodes](./get_outlinecodes/) | Ottiene l'oggetto OutlineCodeDefinitionCollection. La collezione delle definizioni di codice di struttura associate a un progetto. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Ottiene un oggetto contenente proprietà specifiche di Primavera per un progetto letto dal file Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Ottiene un valore che indica se ProjectExternallyEdited è impostato o meno. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Ottiene un valore che indica se RemoveFileProperties è impostato o meno. |
| [get_ResourceAssignments](./get_resourceassignments/) | Ottiene l'oggetto ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Ottiene tutte le definizioni di filtro basate sulle risorse. ResourceFilters è una collezione di oggetti Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Ottiene tutte le definizioni di gruppo basate sulle risorse. ResourceGroups è una collezione di oggetti Group. |
| [get_Resources](./get_resources/) | Ottiene l'oggetto ResourceCollection. |
| [get_Revision](./get_revision/) | Ottiene un valore di Revision. |
| [get_RootTask](./get_roottask/) | Ottiene la radice dell'albero delle attività. |
| [get_SaveVersion](./get_saveversion/) | Ottiene un valore di SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Ottiene un valore che indica se ScheduleFromStart è impostato o meno. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Ottiene un valore che indica se ShowProjectSummaryTask è impostato o meno. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Ottiene un valore che indica se SplitsInProgressTasks è impostato o meno. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Ottiene un valore che indica se SpreadActualCost è impostato o meno. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Ottiene un valore che indica se SpreadPercentComplete è impostato o meno. |
| [get_StartDate](./get_startdate/) | Ottiene un valore di StartDate. |
| [get_StatusDate](./get_statusdate/) | Ottiene un valore di StatusDate. |
| [get_Subject](./get_subject/) | Ottiene un valore di Subject. |
| [get_Tables](./get_tables/) | Ottiene un elenco di oggetti Table. |
| [get_TaskFilters](./get_taskfilters/) | Ottiene tutte le definizioni di filtro basate sulle attività. TaskFilters è una collezione di oggetti Filter. |
| [get_TaskGroups](./get_taskgroups/) | Ottiene tutte le definizioni di gruppo basate sulle attività. TaskGroups è una collezione di oggetti Group. |
| [get_TaskLinks](./get_tasklinks/) | Ottiene l'oggetto TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Ottiene un valore che indica se TaskUpdatesResource è impostato o meno. |
| [get_Template](./get_template/) | Ottiene un valore di Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Ottiene un valore di TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Ottiene un valore di TimescaleStart. |
| [get_Title](./get_title/) | Ottiene un valore di Title. |
| [get_Uid](./get_uid/) | Restituisce un valore di Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Ottiene un valore che indica se UpdateManuallyScheduledTasksWhenEditingLinks è impostato o meno. |
| [get_VbaProject](./get_vbaproject/) | Ottiene un'istanza della classe VbaProject. |
| [get_Views](./get_views/) | Ottiene un elenco di oggetti View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Ottiene la definizione del codice WBS per il progetto. |
| [get_WeekStartDay](./get_weekstartday/) | Ottiene un valore di WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Ottiene un valore di WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Restituisce il tempo di salvataggio della baseline. |
| [GetDuration (3 overloads)](./getduration/) | Ottiene l'oggetto Duration con il numero specificato di unità e il formato di durata predefinito definito nelle impostazioni del progetto Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Restituisce il conteggio delle pagine per il progetto da renderizzare usando la Timescale predefinita (Giorni). |
| [GetPredecessors](./getpredecessors/) | Restituisce una raccolta di collegamenti di attività che sono predecessori dell'attività specificata. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Ottiene le informazioni del file di progetto dallo stream. |
| [GetWork](./getwork/) | Ottiene l'oggetto Duration con il valore double specificato e il formato di lavoro predefinito. |
| [Recalculate (2 overloads)](./recalculate/) | Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Ricalcola ID, Inizio e Fine delle risorse. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Ricalcola Inizio e Fine delle risorse. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Rinumerare il codice WBS di tutte le attività. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Riprogramma il lavoro non completato del progetto per iniziare dopo una data specificata. |
| [Save (5 overloads)](./save/) | Salva il progetto su uno stream usando le opzioni di salvataggio specificate. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Salva il progetto come modello su uno stream specificato. |
| [SaveReport (4 overloads)](./savereport/) | Salva il report di panoramica del progetto sullo stream. |
| [SelectAllChildTasks](./selectallchildtasks/) | Raccoglie ricorsivamente tutte le attività figlio dell'attività radice. |
| [Set (2 overloads)](./set/) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [set_ActualsInSync](./set_actualsinsync/) | Imposta un valore che indica se ActualsInSync è impostato o meno. |
| [set_AdminProject](./set_adminproject/) | Imposta un valore che indica se AdminProject è impostato o meno. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Imposta un valore che indica se AreEditableActualCosts è impostato o meno. |
| [set_Author](./set_author/) | Imposta un valore per Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Imposta un valore che indica se AutoAddNewResourcesAndTasks è impostato o meno. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Imposta se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente utilizzando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [set_Autolink](./set_autolink/) | Imposta un valore che indica se Autolink è impostato o meno. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Imposta un valore per BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Imposta la modalità di calcolo di un progetto. Può essere uno dei valori dell'enumerazione CalculationMode. |
| [set_Calendar](./set_calendar/) | Imposta un valore di Calendar . |
| [set_Category](./set_category/) | Imposta un valore per Category. |
| [set_Comments](./set_comments/) | Imposta un valore per Comments. |
| [set_Company](./set_company/) | Imposta un valore per Company. |
| [set_CreationDate](./set_creationdate/) | Imposta un valore per CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Imposta un valore per CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Imposta un valore per CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Imposta un valore per CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Imposta un valore per CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Imposta un valore per CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Imposta un valore per CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Imposta un valore per CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Imposta un valore per DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Imposta un valore per DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Imposta un valore per DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Imposta un valore per DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Imposta un valore per DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Imposta un valore per DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Imposta un valore di DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Imposta un valore di DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Imposta un valore di DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Imposta la vista predefinita del progetto. |
| [set_DurationFormat](./set_durationformat/) | Imposta un valore di DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Imposta un valore di EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Imposta un valore di ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Imposta un valore di FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Imposta un valore che indica se FiscalYearStart è impostato o meno. |
| [set_FyStartDate](./set_fystartdate/) | Imposta un valore di FyStartDate. |
| [set_Guid](./set_guid/) | Imposta un valore di Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Imposta un valore che indica se HonorConstraints è impostato o meno. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Imposta un valore di HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Imposta un valore che indica se InsertedProjectsLikeSummary è impostato o meno. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Imposta un valore che indica se KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled è impostato o meno. |
| [set_Keywords](./set_keywords/) | Imposta un valore di Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Imposta un valore di LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Imposta un valore di LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Imposta un valore di LastSaved. |
| [set_Manager](./set_manager/) | Imposta un valore di Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Imposta un valore che indica se MicrosoftProjectServerURL è impostato o meno. |
| [set_MinutesPerDay](./set_minutesperday/) | Imposta un valore di MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Imposta un valore di MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Imposta un valore che indica se MoveCompletedEndsBack è impostato o meno. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Imposta un valore che indica se MoveCompletedEndsForward è impostato o meno. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Imposta un valore che indica se MoveRemainingStartsBack è impostato o meno. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Imposta un valore che indica se MoveRemainingStartsForward è impostato o meno. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Imposta un valore che indica se MultipleCriticalPaths è impostato o meno. |
| [set_Name](./set_name/) | Imposta un valore di Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Imposta un valore che indica se NewTasksAreManual è impostato o meno. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Imposta un valore che indica se NewTasksEffortDriven è impostato o meno. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Imposta un valore che indica se NewTasksEstimated è impostato o meno. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Imposta un valore di NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Imposta un valore che indica se ProjectExternallyEdited è impostato o meno. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Imposta un valore che indica se RemoveFileProperties è impostato o meno. |
| [set_Revision](./set_revision/) | Imposta un valore di Revision. |
| [set_SaveVersion](./set_saveversion/) | Imposta un valore di SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Imposta un valore che indica se ScheduleFromStart è impostato o meno. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Imposta un valore che indica se ShowProjectSummaryTask è impostato o meno. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Imposta un valore che indica se SplitsInProgressTasks è impostato o meno. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Imposta un valore che indica se SpreadActualCost è impostato o meno. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Imposta un valore che indica se SpreadPercentComplete è impostato o meno. |
| [set_StartDate](./set_startdate/) | Imposta un valore di StartDate. |
| [set_StatusDate](./set_statusdate/) | Imposta un valore di StatusDate. |
| [set_Subject](./set_subject/) | Imposta un valore di Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Imposta un valore che indica se TaskUpdatesResource è impostato o meno. |
| [set_Template](./set_template/) | Imposta un valore di Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Imposta un valore di TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Imposta un valore di TimescaleStart. |
| [set_Title](./set_title/) | Imposta un valore di Title. |
| [set_Uid](./set_uid/) | Imposta un valore di Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Imposta un valore che indica se UpdateManuallyScheduledTasksWhenEditingLinks è impostato o meno. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Imposta la definizione del codice WBS per il progetto. |
| [set_WeekStartDay](./set_weekstartday/) | Imposta un valore di WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Imposta un valore di WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Salva i campi di baseline nella baseline specificata per l'intero progetto. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Imposta l'ora di salvataggio della baseline. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto. |

