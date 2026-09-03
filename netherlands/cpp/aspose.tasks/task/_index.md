---
title: "Aspose::Tasks::Task class"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks voor C++"
description: "Vertegenwoordigt een taak in een project."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Vertegenwoordigt een taak in een project.

De Task vertegenwoordigt een enkel atomair werkdeel.

Men kan Task gebruiken om een project te plannen door taken te maken en geschikte resources aan hen toe te wijzen. Taken in een project zijn georganiseerd als een wortel‑hiërarchische boomstructuur, met een hoofdtaak en subbomen van onderliggende taken.

Om een boom van taken te bouwen kan men een gespecialiseerde collectie Aspose::Tasks::TaskCollection gebruiken door de eigenschap Project::RootTask te benaderen, bijv.:

```cpp
Project project = new Project();
 
// voeg nieuwe taken toe
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
 
// sla het project op in een van de beschikbare formaten
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Clone](./clone/) | Maakt een volledige kopie van een taak zonder subtaken. |
| [Delete](./delete/) | Verwijdert een taak uit de takenverzameling van het bovenliggende project en al zijn toewijzingen. |
| [Equals (2 overloads)](./equals/) | Geeft een waarde terug die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [Get](./get/) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [get_ActivityId](./get_activityid/) | Stelt het activity‑id‑veld voor – een unieke taakidentificatie die door Primavera wordt gebruikt. (alleen van toepassing op Primavera‑projecten). |
| [get_ActualCost](./get_actualcost/) | Haalt een waarde van ActualCost op. |
| [get_ActualDuration](./get_actualduration/) | Haalt een waarde op van ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Haalt een waarde op van ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Haalt een waarde op van ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Haalt een waarde op van ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Haalt een waarde op van ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Haalt een waarde op van ActualStart. |
| [get_ActualWork](./get_actualwork/) | Haalt een waarde op van ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Haalt een waarde op van ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Haalt een waarde op van ACWP. |
| [get_Assignments](./get_assignments/) | Haalt een verzameling van resource‑toewijzingen op voor dit object. |
| [get_Baselines](./get_baselines/) | Haalt de verzameling op van baseline-waarden van de taak. |
| [get_BCWP](./get_bcwp/) | Haalt een waarde op van BCWP. |
| [get_BCWS](./get_bcws/) | Haalt een waarde op van BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Haalt een waarde op van BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Haalt een waarde op van BudgetWork. |
| [get_Calendar](./get_calendar/) | Haalt een waarde op van Calendar. |
| [get_Children](./get_children/) | Haalt een verzameling van onderliggende taken op van dit object. TaskCollection-object dat onderliggende taken vertegenwoordigt. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Haalt een waarde op van CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Haalt een waarde op van CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Haalt een waarde op van CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Haalt een waarde op van ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Haalt een waarde op van ConstraintType. |
| [get_Contact](./get_contact/) | Haalt een waarde op van Contact. |
| [get_Cost](./get_cost/) | Haalt een waarde op van Cost. |
| [get_CostVariance](./get_costvariance/) | Haalt een waarde op van CostVariance. |
| [get_Created](./get_created/) | Haalt een waarde van Created op. |
| [get_CV](./get_cv/) | Haalt een waarde van CV op. |
| [get_Deadline](./get_deadline/) | Haalt een waarde op van Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Haalt een waarde op die aangeeft of DisplayAsSummary is ingesteld of niet. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Haalt een waarde op die aangeeft of DisplayOnTimeline is ingesteld of niet. |
| [get_Duration](./get_duration/) | Haalt een waarde op van Duration. |
| [get_DurationFormat](./get_durationformat/) | Haalt een waarde op van DurationFormat. |
| [get_DurationText](./get_durationtext/) | Haalt een waarde op van DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Haalt een waarde op van DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Haalt een waarde op van EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Haalt een waarde op van EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Haalt een waarde op van EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Haalt het ExtendedAttributeCollection-object op dat de waarden van een uitgebreid attribuut bevat. |
| [get_ExternalId](./get_externalid/) | Haalt een waarde op van ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Haalt een waarde op van ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Haalt op of stelt de unieke identifier van de externe taak in wanneer de taak extern is. |
| [get_Finish](./get_finish/) | Haalt een waarde van Finish op. |
| [get_FinishSlack](./get_finishslack/) | Haalt een waarde van FinishSlack op. |
| [get_FinishText](./get_finishtext/) | Haalt een waarde van FinishText op. |
| [get_FinishVariance](./get_finishvariance/) | Haalt een waarde op van FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Haalt een waarde van FixedCost op. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Haalt een waarde van FixedCostAccrual op. |
| [get_FreeSlack](./get_freeslack/) | Haalt een waarde van FreeSlack op. |
| [get_Guid](./get_guid/) | Haalt een waarde van Guid op. |
| [get_HideBar](./get_hidebar/) | Haalt een waarde op die aangeeft of HideBar is ingesteld of niet. |
| [get_Hyperlink](./get_hyperlink/) | Haalt de titel of toelichtende tekst op voor een hyperlink die aan een taak is gekoppeld. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Haalt het adres op voor een hyperlink die aan een taak is gekoppeld. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Haalt de specifieke locatie in een document op in een hyperlink die aan een taak is gekoppeld. |
| [get_Id](./get_id/) | Haalt een waarde van Id op. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Haalt een waarde op die aangeeft of IgnoreResourceCalendar is ingesteld of niet. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Haalt een waarde op die aangeeft of IgnoreWarnings is ingesteld of niet. |
| [get_IsActive](./get_isactive/) | Haalt een waarde op die aangeeft of IsActive is ingesteld of niet. |
| [get_IsCritical](./get_iscritical/) | Haalt een waarde op die aangeeft of IsCritical is ingesteld of niet. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Haalt een waarde op die aangeeft of IsEffortDriven is ingesteld of niet. |
| [get_IsEstimated](./get_isestimated/) | Haalt een waarde op die aangeeft of IsEstimated is ingesteld of niet. |
| [get_IsExpanded](./get_isexpanded/) | Haalt een waarde op die aangeeft of IsExpanded is ingesteld of niet. |
| [get_IsExternalTask](./get_isexternaltask/) | Haalt een waarde op die aangeeft of IsExternalTask is ingesteld of niet. |
| [get_IsManual](./get_ismanual/) | Haalt een waarde op die aangeeft of IsManual is ingesteld of niet. |
| [get_IsMarked](./get_ismarked/) | Haalt een waarde op die aangeeft of IsMarked is ingesteld of niet. |
| [get_IsMilestone](./get_ismilestone/) | Haalt een waarde op die aangeeft of IsMilestone is ingesteld of niet. |
| [get_IsNull](./get_isnull/) | Haalt een waarde op die aangeeft of IsNull is ingesteld of niet. |
| [get_IsOverallocated](./get_isoverallocated/) | Haalt een waarde op die aangeeft of IsOverallocated is ingesteld of niet. |
| [get_IsPublished](./get_ispublished/) | Haalt een waarde op die aangeeft of IsPublished is ingesteld of niet. |
| [get_IsRecurring](./get_isrecurring/) | Haalt een waarde op die aangeeft of IsRecurring is ingesteld of niet. |
| [get_IsResumeValid](./get_isresumevalid/) | Haalt een waarde op die aangeeft of IsResumeValid is ingesteld of niet. |
| [get_IsRollup](./get_isrollup/) | Haalt een waarde op die aangeeft of IsRollup is ingesteld of niet. |
| [get_IsSubproject](./get_issubproject/) | Haalt een waarde op die aangeeft of IsSubproject is ingesteld of niet. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Haalt een waarde op die aangeeft of IsSubprojectReadOnly is ingesteld of niet. |
| [get_IsSummary](./get_issummary/) | Haalt een waarde op die aangeeft of IsSummary is ingesteld of niet. |
| [get_LateFinish](./get_latefinish/) | Haalt een waarde van LateFinish op. |
| [get_LateStart](./get_latestart/) | Haalt een waarde van LateStart op. |
| [get_LevelAssignments](./get_levelassignments/) | Haalt een waarde op die aangeeft of LevelAssignments is ingesteld of niet. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Haalt een waarde op die aangeeft of LevelingCanSplit is ingesteld of niet. |
| [get_LevelingDelay](./get_levelingdelay/) | Haalt een waarde van LevelingDelay op. |
| [get_ManualDuration](./get_manualduration/) | Haalt een waarde van ManualDuration op. |
| [get_ManualFinish](./get_manualfinish/) | Haalt een waarde van ManualFinish op. |
| [get_ManualStart](./get_manualstart/) | Haalt een waarde van ManualStart op. |
| [get_Name](./get_name/) | Haalt een waarde van Name op. |
| [get_NotesRTF](./get_notesrtf/) | Haalt een waarde van NotesRTF op. |
| [get_NotesText](./get_notestext/) | Haalt een waarde van NotesText op. |
| [get_OutlineCodes](./get_outlinecodes/) | Haalt OutlineCodeCollection-object op. |
| [get_OutlineLevel](./get_outlinelevel/) | Haalt een waarde van OutlineLevel op. |
| [get_OutlineNumber](./get_outlinenumber/) | Haalt een waarde van OutlineNumber op. |
| [get_OvertimeCost](./get_overtimecost/) | Haalt een waarde van OvertimeCost op. |
| [get_OvertimeWork](./get_overtimework/) | Haalt een waarde van OvertimeWork op. |
| [get_ParentProject](./get_parentproject/) | Haalt het bovenliggende project van een taak op. |
| [get_ParentTask](./get_parenttask/) | Haalt de bovenliggende taak van een taak op. |
| [get_PercentComplete](./get_percentcomplete/) | Haalt een waarde van PercentComplete op. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Haalt een waarde van PercentWorkComplete op. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Haalt een waarde van PhysicalPercentComplete op. |
| [get_Predecessors](./get_predecessors/) | Haalt een TaskCollection-object op dat alle voorgangers van dit Task-object bevat. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Haalt een waarde van PreleveledFinish op. |
| [get_PreleveledStart](./get_preleveledstart/) | Haalt een waarde van PreleveledStart op. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Haalt een object op dat Primavera-specifieke eigenschappen voor een taak bevat, gelezen uit een Primavera-bestand. |
| [get_Priority](./get_priority/) | Haalt een waarde van Priority op. |
| [get_RecurringInfo](./get_recurringinfo/) | Haalt de instantie van de RecurringTaskInfo-klasse op voor de taak die een terugkerende taak is; als de taak geen terugkerende taak is, wordt null geretourneerd; |
| [get_RegularWork](./get_regularwork/) | Haalt een waarde van RegularWork op. |
| [get_RemainingCost](./get_remainingcost/) | Haalt een waarde van RemainingCost op. |
| [get_RemainingDuration](./get_remainingduration/) | Haalt een waarde van RemainingDuration op. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Haalt een waarde van RemainingOvertimeCost op. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Haalt een waarde van RemainingOvertimeWork op. |
| [get_RemainingWork](./get_remainingwork/) | Haalt een waarde van RemainingWork op. |
| [get_Resume](./get_resume/) | Haalt een waarde van Resume op. |
| [get_SplitParts](./get_splitparts/) | Haalt een SplitPart-collectie op die de delen van een taak weergeeft. |
| [get_Start](./get_start/) | Haalt een waarde van Start op. |
| [get_StartSlack](./get_startslack/) | Haalt een waarde van StartSlack op. |
| [get_StartText](./get_starttext/) | Haalt een waarde van StartText op. |
| [get_StartVariance](./get_startvariance/) | Haalt een waarde van StartVariance op. |
| [get_Status](./get_status/) | Haalt de status van de taak op. |
| [get_StatusManager](./get_statusmanager/) | Haalt een waarde van StatusManager op. |
| [get_Stop](./get_stop/) | Haalt een waarde van Stop op. |
| [get_SubprojectName](./get_subprojectname/) | Haalt een waarde van SubprojectName op. |
| [get_Successors](./get_successors/) | Haalt een TaskCollection-object op dat alle opvolgers van dit Task-object bevat. |
| [get_SV](./get_sv/) | De verdiende waarde planningsvariantie tot de projectstatusdatum. Planningsvariantie (SV) is het verschil tussen de BCWP en de BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Haalt een TimephasedDataCollection-object van deze taak op. Het tijdgephaseerde datablock dat aan een taak is gekoppeld. |
| [get_TotalSlack](./get_totalslack/) | Haalt een waarde van TotalSlack op. |
| [get_Type](./get_type/) | Haalt een waarde van Type op. |
| [get_Uid](./get_uid/) | Haalt een waarde van Uid op. |
| [get_Warning](./get_warning/) | Haalt een waarde op die aangeeft of Warning is ingesteld of niet. |
| [get_WBS](./get_wbs/) | Haalt een waarde van WBS op. |
| [get_WBSLevel](./get_wbslevel/) | Haalt een waarde van WBSLevel op. |
| [get_Work](./get_work/) | Haalt een waarde van Work op. |
| [get_WorkVariance](./get_workvariance/) | Haalt een waarde van WorkVariance op. |
| [GetHashCode](./gethashcode/) | Retourneert een hashcode-waarde voor deze Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Retourneert een TimephasedDataCollection-object met TimephasedData-waarden binnen de opgegeven start- en einddatums. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Verplaatst de huidige taak op hetzelfde Outline-niveau vóór de opgegeven taak. Als ParentProject.CalculationMode None is, moet de gebruiker na het gebruik van deze methode Project.Recalculate() aanroepen (dit zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden zoals slack, werk- en kostengebieden, outline-niveaus berekenen). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak‑ID, outline‑niveau en outline‑nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start-/einddatums, stelt vroege/late datums in, berekent slack, werk‑ en kostengebieden, herberekent ID’s en outline‑niveaus). |
| [OutlineIndent](./outlineindent/) | Inspringt een taak in de outline. |
| [OutlineOutdent](./outlineoutdent/) | Promoveert een taak in de outline. |
| [SelectAllChildTasks](./selectallchildtasks/) | Verzamelt recursief alle onderliggende taken van deze taak. |
| [Set](./set/) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [set_ActivityId](./set_activityid/) | Stelt het activity‑id‑veld voor – een unieke taakidentificatie die door Primavera wordt gebruikt. (alleen van toepassing op Primavera‑projecten). |
| [set_ActualCost](./set_actualcost/) | Stelt een waarde in voor ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Stelt een waarde van ActualDuration in. |
| [set_ActualFinish](./set_actualfinish/) | Stelt een waarde van ActualFinish in. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Stelt een waarde in voor ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Stelt een waarde in voor ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Stelt een waarde in voor ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Stelt een waarde van ActualStart in. |
| [set_ActualWork](./set_actualwork/) | Stelt een waarde in voor ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Stelt een waarde in voor ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Stelt een waarde in voor ACWP. |
| [set_Baselines](./set_baselines/) | Stelt de collectie van baseline-waarden van de taak in. |
| [set_BCWP](./set_bcwp/) | Stelt een waarde in voor BCWP. |
| [set_BCWS](./set_bcws/) | Stelt een waarde in voor BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Stelt een waarde in voor BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Stelt een waarde in voor BudgetWork. |
| [set_Calendar](./set_calendar/) | Stelt een waarde in voor Calendar. |
| [set_CommitmentFinish](./set_commitmentfinish/) | Stelt een waarde van CommitmentFinish in. |
| [set_CommitmentStart](./set_commitmentstart/) | Stelt een waarde van CommitmentStart in. |
| [set_CommitmentType](./set_commitmenttype/) | Stelt een waarde van CommitmentType in. |
| [set_ConstraintDate](./set_constraintdate/) | Stelt een waarde van ConstraintDate in. |
| [set_ConstraintType](./set_constrainttype/) | Stelt een waarde van ConstraintType in. |
| [set_Contact](./set_contact/) | Stelt een waarde in voor Contact. |
| [set_Cost](./set_cost/) | Stelt een waarde in voor Cost. |
| [set_CostVariance](./set_costvariance/) | Stelt een waarde in voor CostVariance. |
| [set_Created](./set_created/) | Stelt een waarde in voor Created. |
| [set_CV](./set_cv/) | Stelt een waarde in voor CV. |
| [set_Deadline](./set_deadline/) | Stelt een waarde in voor Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Stelt een waarde in die aangeeft of DisplayAsSummary is ingesteld of niet. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Stelt een waarde in die aangeeft of DisplayOnTimeline is ingesteld of niet. |
| [set_Duration](./set_duration/) | Stelt een waarde in voor Duration. |
| [set_DurationFormat](./set_durationformat/) | Stelt een waarde in voor DurationFormat. |
| [set_DurationText](./set_durationtext/) | Stelt een waarde in voor DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Stelt een waarde in voor DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Stelt een waarde in voor EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Stelt een waarde in voor EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Stelt een waarde in voor EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Stelt een waarde in voor ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Stelt een waarde in voor ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Haalt op of stelt de unieke identifier van de externe taak in wanneer de taak extern is. |
| [set_Finish](./set_finish/) | Stelt een waarde in voor Finish. |
| [set_FinishSlack](./set_finishslack/) | Stelt een waarde in voor FinishSlack. |
| [set_FinishText](./set_finishtext/) | Stelt een waarde in voor FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Stelt een waarde in voor FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Stelt een waarde in voor FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Stelt een waarde in voor FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Stelt een waarde in voor FreeSlack. |
| [set_Guid](./set_guid/) | Stelt een waarde in voor Guid. |
| [set_HideBar](./set_hidebar/) | Stelt een waarde in die aangeeft of HideBar is ingesteld of niet. |
| [set_Hyperlink](./set_hyperlink/) | Stelt de titel of verklarende tekst in voor een hyperlink die aan een taak is gekoppeld. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Stelt het adres in voor een hyperlink die aan een taak is gekoppeld. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Stelt de specifieke locatie in een document in voor een hyperlink die aan een taak is gekoppeld. |
| [set_Id](./set_id/) | Stelt een waarde in voor Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Stelt een waarde in die aangeeft of IgnoreResourceCalendar is ingesteld of niet. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Stelt een waarde in die aangeeft of IgnoreWarnings is ingesteld of niet. |
| [set_IsActive](./set_isactive/) | Stelt een waarde in die aangeeft of IsActive is ingesteld of niet. |
| [set_IsCritical](./set_iscritical/) | Stelt een waarde in die aangeeft of IsCritical is ingesteld of niet. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Stelt een waarde in die aangeeft of IsEffortDriven is ingesteld of niet. |
| [set_IsEstimated](./set_isestimated/) | Stelt een waarde in die aangeeft of IsEstimated is ingesteld of niet. |
| [set_IsExpanded](./set_isexpanded/) | Stelt een waarde in die aangeeft of IsExpanded is ingesteld of niet. |
| [set_IsExternalTask](./set_isexternaltask/) | Stelt een waarde in die aangeeft of IsExternalTask is ingesteld of niet. |
| [set_IsManual](./set_ismanual/) | Stelt een waarde in die aangeeft of IsManual is ingesteld of niet. |
| [set_IsMarked](./set_ismarked/) | Stelt een waarde in die aangeeft of IsMarked is ingesteld of niet. |
| [set_IsMilestone](./set_ismilestone/) | Stelt een waarde in die aangeeft of IsMilestone is ingesteld of niet. |
| [set_IsNull](./set_isnull/) | Stelt een waarde in die aangeeft of IsNull is ingesteld of niet. |
| [set_IsOverallocated](./set_isoverallocated/) | Stelt een waarde in die aangeeft of IsOverallocated is ingesteld of niet. |
| [set_IsPublished](./set_ispublished/) | Stelt een waarde in die aangeeft of IsPublished is ingesteld of niet. |
| [set_IsRecurring](./set_isrecurring/) | Stelt een waarde in die aangeeft of IsRecurring is ingesteld of niet. |
| [set_IsResumeValid](./set_isresumevalid/) | Stelt een waarde in die aangeeft of IsResumeValid is ingesteld of niet. |
| [set_IsRollup](./set_isrollup/) | Stelt een waarde in die aangeeft of IsRollup is ingesteld of niet. |
| [set_IsSubproject](./set_issubproject/) | Stelt een waarde in die aangeeft of IsSubproject is ingesteld of niet. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Stelt een waarde in die aangeeft of IsSubprojectReadOnly is ingesteld of niet. |
| [set_IsSummary](./set_issummary/) | Stelt een waarde in die aangeeft of IsSummary is ingesteld of niet. |
| [set_LateFinish](./set_latefinish/) | Stelt een waarde in voor LateFinish. |
| [set_LateStart](./set_latestart/) | Stelt een waarde in voor LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Stelt een waarde in die aangeeft of LevelAssignments is ingesteld of niet. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Stelt een waarde in die aangeeft of LevelingCanSplit is ingesteld of niet. |
| [set_LevelingDelay](./set_levelingdelay/) | Stelt een waarde in voor LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Stelt een waarde in voor ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Stelt een waarde in voor ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Stelt een waarde in voor ManualStart. |
| [set_Name](./set_name/) | Stelt een waarde in van Name. |
| [set_NotesRTF](./set_notesrtf/) | Stelt een waarde in van NotesRTF. |
| [set_NotesText](./set_notestext/) | Stelt een waarde in van NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Stelt OutlineCodeCollection-object in. |
| [set_OutlineLevel](./set_outlinelevel/) | Stelt een waarde in voor OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Stelt een waarde in voor OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Stelt een waarde in van OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Stelt een waarde in van OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Stelt een waarde in voor PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Stelt een waarde in van PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Stelt een waarde in voor PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Stelt een waarde in voor PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Stelt een waarde in voor PreleveledStart. |
| [set_Priority](./set_priority/) | Stelt een waarde in voor Priority. |
| [set_RegularWork](./set_regularwork/) | Stelt een waarde in van RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Stelt een waarde in van RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Stelt een waarde in voor RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Stelt een waarde in van RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Stelt een waarde in van RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Stelt een waarde in van RemainingWork. |
| [set_Resume](./set_resume/) | Stelt een waarde in voor Resume. |
| [set_Start](./set_start/) | Stelt een waarde in van Start. |
| [set_StartSlack](./set_startslack/) | Stelt een waarde in voor StartSlack. |
| [set_StartText](./set_starttext/) | Stelt een waarde in voor StartText. |
| [set_StartVariance](./set_startvariance/) | Stelt een waarde in voor StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Stelt een waarde in voor StatusManager. |
| [set_Stop](./set_stop/) | Stelt een waarde in voor Stop. |
| [set_SubprojectName](./set_subprojectname/) | Stelt een waarde in voor SubprojectName. |
| [set_SV](./set_sv/) | De verdiende waarde planningsvariantie tot de projectstatusdatum. Planningsvariantie (SV) is het verschil tussen de BCWP en de BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Stelt een TimephasedDataCollection-object in voor deze taak. Het tijdgebaseerde gegevensblok dat aan een taak is gekoppeld. |
| [set_TotalSlack](./set_totalslack/) | Stelt een waarde in voor TotalSlack. |
| [set_Type](./set_type/) | Stelt een waarde in van Type. |
| [set_Uid](./set_uid/) | Stelt een waarde in van Uid. |
| [set_Warning](./set_warning/) | Stelt een waarde in die aangeeft of Warning is ingesteld of niet. |
| [set_WBS](./set_wbs/) | Stelt een waarde in voor WBS. |
| [set_WBSLevel](./set_wbslevel/) | Stelt een waarde in voor WBSLevel. |
| [set_Work](./set_work/) | Stelt een waarde in van Work. |
| [set_WorkVariance](./set_workvariance/) | Stelt een waarde in voor WorkVariance. |
| [ToString](./tostring/) | Retourneert een korte tekenreeksrepresentatie van een taak. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen. |

