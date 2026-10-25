---
title: "classe Aspose::Tasks::Task"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks per C++"
description: "Rappresenta un'attività in un progetto."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Rappresenta un'attività in un progetto.

Il Task rappresenta un singolo blocco atomico di lavoro.

Si può usare Task per pianificare un progetto creando task e assegnando le risorse appropriate a essi. I task in un progetto sono organizzati come una struttura ad albero gerarchico radicato, con un task radice e sottoalberi di task figli.

Per costruire un albero di attività è possibile utilizzare una collezione specializzata Aspose::Tasks::TaskCollection accedendo alla proprietà Project::RootTask, ad esempio:

```cpp
Project project = new Project();
 
// aggiungi nuove attività
Task task1 = project.RootTask.Children.Add(); // a parent task with empty name is added
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserts a task before the childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));
 
// salva il progetto in uno dei formati disponibili
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clone](./clone/) | Crea una copia completa di un'attività senza sotto‑attività. |
| [Delete](./delete/) | Elimina un'attività dalla collezione di attività del progetto principale e tutte le sue assegnazioni. |
| [Equals (2 overloads)](./equals/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [Get](./get/) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [get_ActivityId](./get_activityid/) | Rappresenta il campo ID attività - l'identificatore univoco di un compito utilizzato da Primavera. (applicabile solo ai progetti Primavera). |
| [get_ActualCost](./get_actualcost/) | Ottiene un valore di ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Ottiene il valore di ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Ottiene un valore di ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Ottiene un valore di ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Ottiene un valore di ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Ottiene un valore di ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Ottiene un valore di ActualStart. |
| [get_ActualWork](./get_actualwork/) | Ottiene un valore di ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Ottiene un valore di ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Ottiene un valore di ACWP. |
| [get_Assignments](./get_assignments/) | Ottiene una collezione di assegnazioni di risorse per questo oggetto. |
| [get_Baselines](./get_baselines/) | Ottiene la collezione dei valori di baseline dell'attività. |
| [get_BCWP](./get_bcwp/) | Ottiene un valore di BCWP. |
| [get_BCWS](./get_bcws/) | Ottiene un valore di BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Ottiene un valore di BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Ottiene un valore di BudgetWork. |
| [get_Calendar](./get_calendar/) | Ottiene un valore di Calendar. |
| [get_Children](./get_children/) | Ottiene una collezione di attività figlio di questo oggetto. Oggetto TaskCollection che rappresenta le attività figlio. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Ottiene il valore di CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Ottiene il valore di CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Ottiene il valore di CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Ottiene il valore di ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Ottiene il valore di ConstraintType. |
| [get_Contact](./get_contact/) | Ottiene il valore di Contact. |
| [get_Cost](./get_cost/) | Ottiene un valore di Cost. |
| [get_CostVariance](./get_costvariance/) | Ottiene un valore di CostVariance. |
| [get_Created](./get_created/) | Ottiene un valore di Created. |
| [get_CV](./get_cv/) | Ottiene un valore di CV. |
| [get_Deadline](./get_deadline/) | Ottiene il valore di Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Ottiene un valore che indica se DisplayAsSummary è impostato o meno. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Ottiene un valore che indica se DisplayOnTimeline è impostato o meno. |
| [get_Duration](./get_duration/) | Ottiene il valore di Duration. |
| [get_DurationFormat](./get_durationformat/) | Ottiene un valore di DurationFormat. |
| [get_DurationText](./get_durationtext/) | Ottiene il valore di DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Ottiene il valore di DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Ottiene il valore di EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Ottiene il valore di EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Ottiene un valore di EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Ottiene l'oggetto ExtendedAttributeCollection contenente i valori di un attributo esteso. |
| [get_ExternalId](./get_externalid/) | Ottiene il valore di ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Ottiene il valore di ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Ottiene o imposta l'identificatore univoco dell'attività esterna quando l'attività è esterna. |
| [get_Finish](./get_finish/) | Ottiene un valore di Finish. |
| [get_FinishSlack](./get_finishslack/) | Ottiene il valore di FinishSlack. |
| [get_FinishText](./get_finishtext/) | Ottiene il valore di FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Ottiene un valore di FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Ottiene il valore di FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Ottiene il valore di FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Ottiene il valore di FreeSlack. |
| [get_Guid](./get_guid/) | Ottiene un valore di Guid. |
| [get_HideBar](./get_hidebar/) | Ottiene un valore che indica se HideBar è impostato o meno. |
| [get_Hyperlink](./get_hyperlink/) | Ottiene il titolo o il testo esplicativo per un collegamento ipertestuale associato a un'attività. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Ottiene l'indirizzo per un collegamento ipertestuale associato a un'attività. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Ottiene la posizione specifica in un documento in un collegamento ipertestuale associato a un'attività. |
| [get_Id](./get_id/) | Ottiene un valore di Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Ottiene un valore che indica se IgnoreResourceCalendar è impostato o meno. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Ottiene un valore che indica se IgnoreWarnings è impostato o meno. |
| [get_IsActive](./get_isactive/) | Ottiene un valore che indica se IsActive è impostato o meno. |
| [get_IsCritical](./get_iscritical/) | Ottiene un valore che indica se IsCritical è impostato o meno. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Ottiene un valore che indica se IsEffortDriven è impostato o meno. |
| [get_IsEstimated](./get_isestimated/) | Ottiene un valore che indica se IsEstimated è impostato o meno. |
| [get_IsExpanded](./get_isexpanded/) | Ottiene un valore che indica se IsExpanded è impostato o meno. |
| [get_IsExternalTask](./get_isexternaltask/) | Ottiene un valore che indica se IsExternalTask è impostato o meno. |
| [get_IsManual](./get_ismanual/) | Ottiene un valore che indica se IsManual è impostato o meno. |
| [get_IsMarked](./get_ismarked/) | Ottiene un valore che indica se IsMarked è impostato o meno. |
| [get_IsMilestone](./get_ismilestone/) | Ottiene un valore che indica se IsMilestone è impostato o meno. |
| [get_IsNull](./get_isnull/) | Ottiene un valore che indica se IsNull è impostato o meno. |
| [get_IsOverallocated](./get_isoverallocated/) | Ottiene un valore che indica se IsOverallocated è impostato o meno. |
| [get_IsPublished](./get_ispublished/) | Ottiene un valore che indica se IsPublished è impostato o meno. |
| [get_IsRecurring](./get_isrecurring/) | Ottiene un valore che indica se IsRecurring è impostato o meno. |
| [get_IsResumeValid](./get_isresumevalid/) | Ottiene un valore che indica se IsResumeValid è impostato o meno. |
| [get_IsRollup](./get_isrollup/) | Restituisce un valore che indica se IsRollup è impostato o meno. |
| [get_IsSubproject](./get_issubproject/) | Restituisce un valore che indica se IsSubproject è impostato o meno. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Restituisce un valore che indica se IsSubprojectReadOnly è impostato o meno. |
| [get_IsSummary](./get_issummary/) | Restituisce un valore che indica se IsSummary è impostato o meno. |
| [get_LateFinish](./get_latefinish/) | Restituisce un valore di LateFinish. |
| [get_LateStart](./get_latestart/) | Restituisce un valore di LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Restituisce un valore che indica se LevelAssignments è impostato o meno. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Restituisce un valore che indica se LevelingCanSplit è impostato o meno. |
| [get_LevelingDelay](./get_levelingdelay/) | Ottiene un valore di LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Restituisce un valore di ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Restituisce un valore di ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Restituisce un valore di ManualStart. |
| [get_Name](./get_name/) | Ottiene un valore di Name. |
| [get_NotesRTF](./get_notesrtf/) | Ottiene un valore di NotesRTF. |
| [get_NotesText](./get_notestext/) | Ottiene un valore di NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Restituisce l'oggetto OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Restituisce un valore di OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Restituisce un valore di OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Restituisce un valore di OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Restituisce un valore di OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Restituisce il progetto padre di un'attività. |
| [get_ParentTask](./get_parenttask/) | Restituisce l'attività padre di un'attività. |
| [get_PercentComplete](./get_percentcomplete/) | Restituisce un valore di PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Restituisce un valore di PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Restituisce un valore di PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Restituisce un oggetto TaskCollection che contiene tutti i predecessori di questo oggetto Task. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Restituisce un valore di PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Restituisce un valore di PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Restituisce un oggetto contenente le proprietà specifiche di Primavera per un'attività letta dal file Primavera. |
| [get_Priority](./get_priority/) | Restituisce un valore di Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Restituisce l'istanza della classe RecurringTaskInfo per l'attività che è un'attività ricorrente; se l'attività non è ricorrente restituisce null; |
| [get_RegularWork](./get_regularwork/) | Restituisce un valore di RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Restituisce un valore di RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Restituisce un valore di RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Restituisce un valore di RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Restituisce un valore di RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Restituisce un valore di RemainingWork. |
| [get_Resume](./get_resume/) | Ottiene un valore di Resume. |
| [get_SplitParts](./get_splitparts/) | Ottiene una collezione SplitPart che rappresenta le parti di un'attività. |
| [get_Start](./get_start/) | Restituisce un valore di Start. |
| [get_StartSlack](./get_startslack/) | Ottiene un valore di StartSlack. |
| [get_StartText](./get_starttext/) | Ottiene un valore di StartText. |
| [get_StartVariance](./get_startvariance/) | Ottiene un valore di StartVariance. |
| [get_Status](./get_status/) | Ottiene lo stato dell'attività. |
| [get_StatusManager](./get_statusmanager/) | Ottiene un valore di StatusManager. |
| [get_Stop](./get_stop/) | Ottiene un valore di Stop. |
| [get_SubprojectName](./get_subprojectname/) | Ottiene un valore di SubprojectName. |
| [get_Successors](./get_successors/) | Ottiene un oggetto TaskCollection che contiene tutti i successori di questo oggetto Task. |
| [get_SV](./get_sv/) | La varianza di programmazione del valore guadagnato, fino alla data di stato del progetto. La varianza di programmazione (SV) è la differenza tra BCWP e BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Ottiene un oggetto TimephasedDataCollection di questa attività. Il blocco di dati temporizzati associato a un'attività. |
| [get_TotalSlack](./get_totalslack/) | Ottiene un valore di TotalSlack. |
| [get_Type](./get_type/) | Restituisce un valore di Type. |
| [get_Uid](./get_uid/) | Restituisce un valore di Uid. |
| [get_Warning](./get_warning/) | Ottiene un valore che indica se Warning è impostato o meno. |
| [get_WBS](./get_wbs/) | Ottiene un valore di WBS. |
| [get_WBSLevel](./get_wbslevel/) | Ottiene un valore di WBSLevel. |
| [get_Work](./get_work/) | Restituisce un valore di Work. |
| [get_WorkVariance](./get_workvariance/) | Ottiene un valore di WorkVariance. |
| [GetHashCode](./gethashcode/) | Restituisce un valore di hash code per questo Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Restituisce un oggetto TimephasedDataCollection con i valori TimephasedData compresi tra le date di inizio e fine specificate. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Sposta l'attività corrente allo stesso livello di outline prima dell'attività specificata. Se ParentProject.CalculationMode è None, l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come slacks, lavoro e costi, i livelli di outline). Se ParentProject.CalculationMode è Manual, il metodo calcolerà automaticamente solo l'ID dell'attività, il livello di outline e i numeri di outline. Se ParentProject.CalculationMode è Automatic, il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, lavoro e costi, ricalcola gli ID e i livelli di outline). |
| [OutlineIndent](./outlineindent/) | Aumenta l'indentazione di un'attività nell'outline. |
| [OutlineOutdent](./outlineoutdent/) | Promuove un'attività nell'outline. |
| [SelectAllChildTasks](./selectallchildtasks/) | Raccoglie ricorsivamente tutti i task figli di questa attività. |
| [Set](./set/) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [set_ActivityId](./set_activityid/) | Rappresenta il campo ID attività - l'identificatore univoco di un compito utilizzato da Primavera. (applicabile solo ai progetti Primavera). |
| [set_ActualCost](./set_actualcost/) | Imposta un valore di ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Imposta un valore di ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Imposta un valore di ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Imposta un valore di ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Imposta un valore di ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Imposta un valore di ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Imposta un valore di ActualStart. |
| [set_ActualWork](./set_actualwork/) | Imposta un valore di ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Imposta un valore di ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Imposta un valore di ACWP. |
| [set_Baselines](./set_baselines/) | Imposta la collezione dei valori baseline dell'attività. |
| [set_BCWP](./set_bcwp/) | Imposta un valore di BCWP. |
| [set_BCWS](./set_bcws/) | Imposta un valore di BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Imposta un valore di BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Imposta un valore di BudgetWork. |
| [set_Calendar](./set_calendar/) | Imposta un valore di Calendar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | Imposta un valore di CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Imposta un valore di CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Imposta un valore di CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Imposta un valore di ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Imposta un valore di ConstraintType. |
| [set_Contact](./set_contact/) | Imposta un valore di Contact. |
| [set_Cost](./set_cost/) | Imposta un valore di Cost. |
| [set_CostVariance](./set_costvariance/) | Imposta un valore di CostVariance. |
| [set_Created](./set_created/) | Imposta un valore di Created. |
| [set_CV](./set_cv/) | Imposta un valore di CV. |
| [set_Deadline](./set_deadline/) | Imposta un valore di Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Imposta un valore che indica se DisplayAsSummary è impostato o meno. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Imposta un valore che indica se DisplayOnTimeline è impostato o meno. |
| [set_Duration](./set_duration/) | Imposta un valore di Duration. |
| [set_DurationFormat](./set_durationformat/) | Imposta un valore di DurationFormat. |
| [set_DurationText](./set_durationtext/) | Imposta un valore di DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Imposta un valore di DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Imposta un valore di EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Imposta un valore di EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Imposta un valore di EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Imposta un valore di ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Imposta un valore di ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Ottiene o imposta l'identificatore univoco dell'attività esterna quando l'attività è esterna. |
| [set_Finish](./set_finish/) | Imposta un valore di Finish. |
| [set_FinishSlack](./set_finishslack/) | Imposta un valore di FinishSlack. |
| [set_FinishText](./set_finishtext/) | Imposta un valore di FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Imposta un valore di FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Imposta un valore di FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Imposta un valore di FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Imposta un valore di FreeSlack. |
| [set_Guid](./set_guid/) | Imposta un valore di Guid. |
| [set_HideBar](./set_hidebar/) | Imposta un valore che indica se HideBar è impostato o meno. |
| [set_Hyperlink](./set_hyperlink/) | Imposta il titolo o il testo esplicativo per un collegamento ipertestuale associato a un'attività. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Imposta l'indirizzo per un collegamento ipertestuale associato a un'attività. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Imposta la posizione specifica in un documento in un collegamento ipertestuale associato a un'attività. |
| [set_Id](./set_id/) | Imposta un valore di Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Imposta un valore che indica se IgnoreResourceCalendar è impostato o meno. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Imposta un valore che indica se IgnoreWarnings è impostato o meno. |
| [set_IsActive](./set_isactive/) | Imposta un valore che indica se IsActive è impostato o meno. |
| [set_IsCritical](./set_iscritical/) | Imposta un valore che indica se IsCritical è impostato o meno. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Imposta un valore che indica se IsEffortDriven è impostato o meno. |
| [set_IsEstimated](./set_isestimated/) | Imposta un valore che indica se IsEstimated è impostato o meno. |
| [set_IsExpanded](./set_isexpanded/) | Imposta un valore che indica se IsExpanded è impostato o meno. |
| [set_IsExternalTask](./set_isexternaltask/) | Imposta un valore che indica se IsExternalTask è impostato o meno. |
| [set_IsManual](./set_ismanual/) | Imposta un valore che indica se IsManual è impostato o meno. |
| [set_IsMarked](./set_ismarked/) | Imposta un valore che indica se IsMarked è impostato o meno. |
| [set_IsMilestone](./set_ismilestone/) | Imposta un valore che indica se IsMilestone è impostato o meno. |
| [set_IsNull](./set_isnull/) | Imposta un valore che indica se IsNull è impostato o meno. |
| [set_IsOverallocated](./set_isoverallocated/) | Imposta un valore che indica se IsOverallocated è impostato o meno. |
| [set_IsPublished](./set_ispublished/) | Imposta un valore che indica se IsPublished è impostato o meno. |
| [set_IsRecurring](./set_isrecurring/) | Imposta un valore che indica se IsRecurring è impostato o meno. |
| [set_IsResumeValid](./set_isresumevalid/) | Imposta un valore che indica se IsResumeValid è impostato o meno. |
| [set_IsRollup](./set_isrollup/) | Imposta un valore che indica se IsRollup è impostato o meno. |
| [set_IsSubproject](./set_issubproject/) | Imposta un valore che indica se IsSubproject è impostato o meno. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Imposta un valore che indica se IsSubprojectReadOnly è impostato o meno. |
| [set_IsSummary](./set_issummary/) | Imposta un valore che indica se IsSummary è impostato o meno. |
| [set_LateFinish](./set_latefinish/) | Imposta un valore di LateFinish. |
| [set_LateStart](./set_latestart/) | Imposta un valore di LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Imposta un valore che indica se LevelAssignments è impostato o meno. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Imposta un valore che indica se LevelingCanSplit è impostato o meno. |
| [set_LevelingDelay](./set_levelingdelay/) | Imposta un valore di LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Imposta un valore di ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Imposta un valore di ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Imposta un valore di ManualStart. |
| [set_Name](./set_name/) | Imposta un valore di Name. |
| [set_NotesRTF](./set_notesrtf/) | Imposta un valore di NotesRTF. |
| [set_NotesText](./set_notestext/) | Imposta un valore di NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Imposta l'oggetto OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Imposta un valore di OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Imposta un valore di OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Imposta un valore di OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Imposta un valore di OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Imposta un valore di PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Imposta un valore di PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Imposta un valore di PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Imposta un valore di PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Imposta un valore di PreleveledStart. |
| [set_Priority](./set_priority/) | Imposta un valore di Priority. |
| [set_RegularWork](./set_regularwork/) | Imposta un valore di RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Imposta un valore di RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Imposta un valore di RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Imposta un valore di RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Imposta un valore di RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Imposta un valore di RemainingWork. |
| [set_Resume](./set_resume/) | Imposta un valore di Resume. |
| [set_Start](./set_start/) | Imposta un valore di Start. |
| [set_StartSlack](./set_startslack/) | Imposta un valore di StartSlack. |
| [set_StartText](./set_starttext/) | Imposta un valore di StartText. |
| [set_StartVariance](./set_startvariance/) | Imposta un valore di StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Imposta un valore di StatusManager. |
| [set_Stop](./set_stop/) | Imposta un valore di Stop. |
| [set_SubprojectName](./set_subprojectname/) | Imposta un valore di SubprojectName. |
| [set_SV](./set_sv/) | La varianza di programmazione del valore guadagnato, fino alla data di stato del progetto. La varianza di programmazione (SV) è la differenza tra BCWP e BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Imposta un oggetto TimephasedDataCollection per questa attività. Il blocco di dati temporizzati associato a un'attività. |
| [set_TotalSlack](./set_totalslack/) | Imposta un valore di TotalSlack. |
| [set_Type](./set_type/) | Imposta un valore di Type. |
| [set_Uid](./set_uid/) | Imposta un valore di Uid. |
| [set_Warning](./set_warning/) | Imposta un valore che indica se Warning è impostato o meno. |
| [set_WBS](./set_wbs/) | Imposta un valore di WBS. |
| [set_WBSLevel](./set_wbslevel/) | Imposta un valore di WBSLevel. |
| [set_Work](./set_work/) | Imposta un valore di Work. |
| [set_WorkVariance](./set_workvariance/) | Imposta un valore di WorkVariance. |
| [ToString](./tostring/) | Restituisce una rappresentazione stringa breve di un'attività. I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche. |

