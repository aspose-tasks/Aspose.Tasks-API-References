---
title: "Aspose::Tasks::Task classe"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks pour C++"
description: "Représente une tâche dans un projet."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Représente une tâche dans un projet.

La Task représente un morceau atomique de travail.

On peut utiliser Task pour planifier un projet en créant des tâches et en affectant les ressources appropriées à celles‑ci. Les tâches d'un projet sont organisées sous forme d'une structure arborescente hiérarchique enracinée, avec une tâche racine et des sous‑arbres de tâches enfants.

Pour créer un arbre de tâches, on peut utiliser une collection spécialisée Aspose::Tasks::TaskCollection en accédant à la propriété Project::RootTask, par exemple :

```cpp
Project project = new Project();
 
// ajouter de nouvelles tâches
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
 
// enregistrer le projet dans l'un des formats disponibles
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Clone](./clone/) | Crée une copie complète d'une tâche sans sous‑tâches. |
| [Delete](./delete/) | Supprime une tâche de la collection de tâches du projet parent ainsi que toutes ses affectations. |
| [Equals (2 overloads)](./equals/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [Get](./get/) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [get_ActivityId](./get_activityid/) | Représente le champ d'identifiant d'activité - l'identifiant unique d'une tâche utilisé par Primavera. (applicable uniquement aux projets Primavera). |
| [get_ActualCost](./get_actualcost/) | Obtient la valeur de ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Obtient la valeur de ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Obtient une valeur de ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Obtient une valeur de ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Obtient une valeur de ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Obtient une valeur de ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Obtient une valeur de ActualStart. |
| [get_ActualWork](./get_actualwork/) | Obtient une valeur de ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Obtient une valeur de ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Obtient une valeur de ACWP. |
| [get_Assignments](./get_assignments/) | Obtient une collection d'affectations de ressources pour cet objet. |
| [get_Baselines](./get_baselines/) | Obtient la collection des valeurs de base de la tâche. |
| [get_BCWP](./get_bcwp/) | Obtient une valeur de BCWP. |
| [get_BCWS](./get_bcws/) | Obtient une valeur de BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Obtient une valeur de BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Obtient une valeur de BudgetWork. |
| [get_Calendar](./get_calendar/) | Obtient une valeur de Calendar. |
| [get_Children](./get_children/) | Obtient une collection de sous‑tâches de cet objet. Objet TaskCollection qui représente les tâches enfants. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Obtient la valeur de CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Obtient la valeur de CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Obtient la valeur de CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Obtient la valeur de ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Obtient la valeur de ConstraintType. |
| [get_Contact](./get_contact/) | Obtient la valeur de Contact. |
| [get_Cost](./get_cost/) | Obtient une valeur de Cost. |
| [get_CostVariance](./get_costvariance/) | Obtient une valeur de CostVariance. |
| [get_Created](./get_created/) | Obtient une valeur de Created. |
| [get_CV](./get_cv/) | Obtient une valeur de CV. |
| [get_Deadline](./get_deadline/) | Obtient la valeur de Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Obtient une valeur indiquant si DisplayAsSummary est défini ou non. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Obtient une valeur indiquant si DisplayOnTimeline est défini ou non. |
| [get_Duration](./get_duration/) | Obtient la valeur de Duration. |
| [get_DurationFormat](./get_durationformat/) | Obtient une valeur de DurationFormat. |
| [get_DurationText](./get_durationtext/) | Obtient la valeur de DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Obtient la valeur de DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Obtient la valeur de EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Obtient la valeur de EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Obtient une valeur de EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Obtient l'objet ExtendedAttributeCollection contenant les valeurs d'un attribut étendu. |
| [get_ExternalId](./get_externalid/) | Obtient la valeur de ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Obtient la valeur de ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Obtient ou définit l'identifiant unique de la tâche externe lorsque la tâche est externe. |
| [get_Finish](./get_finish/) | Obtient une valeur de Finish. |
| [get_FinishSlack](./get_finishslack/) | Obtient une valeur de FinishSlack. |
| [get_FinishText](./get_finishtext/) | Obtient une valeur de FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Obtient une valeur de FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Obtient une valeur de FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Obtient une valeur de FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Obtient une valeur de FreeSlack. |
| [get_Guid](./get_guid/) | Obtient une valeur de Guid. |
| [get_HideBar](./get_hidebar/) | Obtient une valeur indiquant si HideBar est défini ou non. |
| [get_Hyperlink](./get_hyperlink/) | Obtient le titre ou le texte explicatif d'un hyperlien associé à une tâche. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Obtient l'adresse d'un hyperlien associé à une tâche. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Obtient l'emplacement spécifique dans un document d'un hyperlien associé à une tâche. |
| [get_Id](./get_id/) | Obtient une valeur de Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Obtient une valeur indiquant si IgnoreResourceCalendar est défini ou non. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Obtient une valeur indiquant si IgnoreWarnings est défini ou non. |
| [get_IsActive](./get_isactive/) | Obtient une valeur indiquant si IsActive est défini ou non. |
| [get_IsCritical](./get_iscritical/) | Obtient une valeur indiquant si IsCritical est défini ou non. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Obtient une valeur indiquant si IsEffortDriven est défini ou non. |
| [get_IsEstimated](./get_isestimated/) | Obtient une valeur indiquant si IsEstimated est défini ou non. |
| [get_IsExpanded](./get_isexpanded/) | Obtient une valeur indiquant si IsExpanded est défini ou non. |
| [get_IsExternalTask](./get_isexternaltask/) | Obtient une valeur indiquant si IsExternalTask est défini ou non. |
| [get_IsManual](./get_ismanual/) | Obtient une valeur indiquant si IsManual est défini ou non. |
| [get_IsMarked](./get_ismarked/) | Obtient une valeur indiquant si IsMarked est défini ou non. |
| [get_IsMilestone](./get_ismilestone/) | Obtient une valeur indiquant si IsMilestone est défini ou non. |
| [get_IsNull](./get_isnull/) | Obtient une valeur indiquant si IsNull est défini ou non. |
| [get_IsOverallocated](./get_isoverallocated/) | Obtient une valeur indiquant si IsOverallocated est défini ou non. |
| [get_IsPublished](./get_ispublished/) | Obtient une valeur indiquant si IsPublished est défini ou non. |
| [get_IsRecurring](./get_isrecurring/) | Obtient une valeur indiquant si IsRecurring est défini ou non. |
| [get_IsResumeValid](./get_isresumevalid/) | Obtient une valeur indiquant si IsResumeValid est défini ou non. |
| [get_IsRollup](./get_isrollup/) | Obtient une valeur indiquant si IsRollup est défini ou non. |
| [get_IsSubproject](./get_issubproject/) | Obtient une valeur indiquant si IsSubproject est défini ou non. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Obtient une valeur indiquant si IsSubprojectReadOnly est défini ou non. |
| [get_IsSummary](./get_issummary/) | Obtient une valeur indiquant si IsSummary est défini ou non. |
| [get_LateFinish](./get_latefinish/) | Obtient une valeur de LateFinish. |
| [get_LateStart](./get_latestart/) | Obtient une valeur de LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Obtient une valeur indiquant si LevelAssignments est défini ou non. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Obtient une valeur indiquant si LevelingCanSplit est défini ou non. |
| [get_LevelingDelay](./get_levelingdelay/) | Obtient une valeur de LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Obtient une valeur de ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Obtient une valeur de ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Obtient une valeur de ManualStart. |
| [get_Name](./get_name/) | Obtient une valeur de Name. |
| [get_NotesRTF](./get_notesrtf/) | Obtient une valeur de NotesRTF. |
| [get_NotesText](./get_notestext/) | Obtient une valeur de NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Obtient l'objet OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Obtient une valeur de OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Obtient une valeur de OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Obtient une valeur de OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Obtient une valeur de OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Obtient le projet parent d'une tâche. |
| [get_ParentTask](./get_parenttask/) | Obtient la tâche parente d'une tâche. |
| [get_PercentComplete](./get_percentcomplete/) | Obtient une valeur de PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Obtient une valeur de PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Obtient une valeur de PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Obtient un objet TaskCollection qui contient tous les prédécesseurs de cet objet Task. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Obtient une valeur de PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Obtient une valeur de PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Obtient un objet contenant les propriétés spécifiques à Primavera pour une tâche lues depuis le fichier Primavera. |
| [get_Priority](./get_priority/) | Obtient une valeur de Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Obtient l'instance de la classe RecurringTaskInfo pour la tâche qui est récurrente ; si la tâche n'est pas récurrente, alors renvoie null ; |
| [get_RegularWork](./get_regularwork/) | Obtient une valeur de RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Obtient une valeur de RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Obtient une valeur de RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Obtient une valeur de RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Obtient une valeur de RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Obtient une valeur de RemainingWork. |
| [get_Resume](./get_resume/) | Obtient une valeur de Resume. |
| [get_SplitParts](./get_splitparts/) | Obtient une collection SplitPart qui représente les parties d'une tâche. |
| [get_Start](./get_start/) | Obtient une valeur de Start. |
| [get_StartSlack](./get_startslack/) | Obtient une valeur de StartSlack. |
| [get_StartText](./get_starttext/) | Obtient une valeur de StartText. |
| [get_StartVariance](./get_startvariance/) | Obtient une valeur de StartVariance. |
| [get_Status](./get_status/) | Obtient le statut de la tâche. |
| [get_StatusManager](./get_statusmanager/) | Obtient une valeur de StatusManager. |
| [get_Stop](./get_stop/) | Obtient une valeur de Stop. |
| [get_SubprojectName](./get_subprojectname/) | Obtient une valeur de SubprojectName. |
| [get_Successors](./get_successors/) | Obtient un objet TaskCollection qui contient tous les successeurs de cet objet Task. |
| [get_SV](./get_sv/) | La variance d'échéancier de la valeur acquise, jusqu'à la date d'état du projet. La variance d'échéancier (SV) est la différence entre le BCWP et le BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Obtient un objet TimephasedDataCollection de cette tâche. Le bloc de données temporelles associé à une tâche. |
| [get_TotalSlack](./get_totalslack/) | Obtient une valeur de TotalSlack. |
| [get_Type](./get_type/) | Obtient une valeur de Type. |
| [get_Uid](./get_uid/) | Obtient une valeur de Uid. |
| [get_Warning](./get_warning/) | Obtient une valeur indiquant si Warning est défini ou non. |
| [get_WBS](./get_wbs/) | Obtient une valeur de WBS. |
| [get_WBSLevel](./get_wbslevel/) | Obtient une valeur de WBSLevel. |
| [get_Work](./get_work/) | Obtient une valeur de Work. |
| [get_WorkVariance](./get_workvariance/) | Obtient une valeur de WorkVariance. |
| [GetHashCode](./gethashcode/) | Renvoie une valeur de code de hachage pour cette Task. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Renvoie un objet TimephasedDataCollection avec les valeurs TimephasedData entre les dates de début et de fin données. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Déplace la tâche actuelle au même niveau de plan (Outline Level) avant la tâche spécifiée. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates au plus tôt/au plus tard) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les niveaux de plan). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'ID de la tâche, le niveau de plan et les numéros de plan automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates au plus tôt/au plus tard, calcule les marges, le travail et les champs de coût, recalculera les IDs et les niveaux de plan). |
| [OutlineIndent](./outlineindent/) | Indente une tâche dans le plan. |
| [OutlineOutdent](./outlineoutdent/) | Promouvoir une tâche dans le plan. |
| [SelectAllChildTasks](./selectallchildtasks/) | Collecte récursivement toutes les sous‑tâches de cette tâche. |
| [Set](./set/) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [set_ActivityId](./set_activityid/) | Représente le champ d'identifiant d'activité - l'identifiant unique d'une tâche utilisé par Primavera. (applicable uniquement aux projets Primavera). |
| [set_ActualCost](./set_actualcost/) | Définit une valeur de ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Définit une valeur de ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Définit une valeur de ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Définit une valeur de ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Définit une valeur de ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Définit une valeur de ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Définit une valeur de ActualStart. |
| [set_ActualWork](./set_actualwork/) | Définit une valeur de ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Définit une valeur de ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Définit une valeur de ACWP. |
| [set_Baselines](./set_baselines/) | Définit la collection des valeurs de référence de la tâche. |
| [set_BCWP](./set_bcwp/) | Définit une valeur de BCWP. |
| [set_BCWS](./set_bcws/) | Définit une valeur de BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Définit une valeur de BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Définit une valeur de BudgetWork. |
| [set_Calendar](./set_calendar/) | Définit une valeur de Calendar. |
| [set_CommitmentFinish](./set_commitmentfinish/) | Définit une valeur de CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Définit une valeur de CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Définit une valeur de CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Définit une valeur de ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Définit une valeur de ConstraintType. |
| [set_Contact](./set_contact/) | Définit une valeur de Contact. |
| [set_Cost](./set_cost/) | Définit une valeur de Cost. |
| [set_CostVariance](./set_costvariance/) | Définit une valeur de CostVariance. |
| [set_Created](./set_created/) | Définit une valeur de Created. |
| [set_CV](./set_cv/) | Définit une valeur de CV. |
| [set_Deadline](./set_deadline/) | Définit une valeur de Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Définit une valeur indiquant si DisplayAsSummary est défini ou non. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Définit une valeur indiquant si DisplayOnTimeline est défini ou non. |
| [set_Duration](./set_duration/) | Définit une valeur de Duration. |
| [set_DurationFormat](./set_durationformat/) | Définit une valeur de DurationFormat. |
| [set_DurationText](./set_durationtext/) | Définit une valeur de DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Définit une valeur de DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Définit une valeur de EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Définit une valeur de EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Définit une valeur de EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Définit une valeur de ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Définit une valeur de ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Obtient ou définit l'identifiant unique de la tâche externe lorsque la tâche est externe. |
| [set_Finish](./set_finish/) | Définit une valeur de Finish. |
| [set_FinishSlack](./set_finishslack/) | Définit une valeur de FinishSlack. |
| [set_FinishText](./set_finishtext/) | Définit une valeur de FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Définit une valeur de FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Définit une valeur de FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Définit une valeur de FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Définit une valeur de FreeSlack. |
| [set_Guid](./set_guid/) | Définit une valeur de Guid. |
| [set_HideBar](./set_hidebar/) | Définit une valeur indiquant si HideBar est défini ou non. |
| [set_Hyperlink](./set_hyperlink/) | Définit le titre ou le texte explicatif d’un hyperlien associé à une tâche. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Définit l’adresse d’un hyperlien associé à une tâche. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Définit l’emplacement spécifique dans un document d’un hyperlien associé à une tâche. |
| [set_Id](./set_id/) | Définit une valeur de Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Définit une valeur indiquant si IgnoreResourceCalendar est défini ou non. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Définit une valeur indiquant si IgnoreWarnings est défini ou non. |
| [set_IsActive](./set_isactive/) | Définit une valeur indiquant si IsActive est défini ou non. |
| [set_IsCritical](./set_iscritical/) | Définit une valeur indiquant si IsCritical est défini ou non. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Définit une valeur indiquant si IsEffortDriven est défini ou non. |
| [set_IsEstimated](./set_isestimated/) | Définit une valeur indiquant si IsEstimated est défini ou non. |
| [set_IsExpanded](./set_isexpanded/) | Définit une valeur indiquant si IsExpanded est défini ou non. |
| [set_IsExternalTask](./set_isexternaltask/) | Définit une valeur indiquant si IsExternalTask est défini ou non. |
| [set_IsManual](./set_ismanual/) | Définit une valeur indiquant si IsManual est défini ou non. |
| [set_IsMarked](./set_ismarked/) | Définit une valeur indiquant si IsMarked est défini ou non. |
| [set_IsMilestone](./set_ismilestone/) | Définit une valeur indiquant si IsMilestone est défini ou non. |
| [set_IsNull](./set_isnull/) | Définit une valeur indiquant si IsNull est défini ou non. |
| [set_IsOverallocated](./set_isoverallocated/) | Définit une valeur indiquant si IsOverallocated est défini ou non. |
| [set_IsPublished](./set_ispublished/) | Définit une valeur indiquant si IsPublished est défini ou non. |
| [set_IsRecurring](./set_isrecurring/) | Définit une valeur indiquant si IsRecurring est défini ou non. |
| [set_IsResumeValid](./set_isresumevalid/) | Définit une valeur indiquant si IsResumeValid est défini ou non. |
| [set_IsRollup](./set_isrollup/) | Définit une valeur indiquant si IsRollup est défini ou non. |
| [set_IsSubproject](./set_issubproject/) | Définit une valeur indiquant si IsSubproject est défini ou non. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Définit une valeur indiquant si IsSubprojectReadOnly est défini ou non. |
| [set_IsSummary](./set_issummary/) | Définit une valeur indiquant si IsSummary est défini ou non. |
| [set_LateFinish](./set_latefinish/) | Définit une valeur de LateFinish. |
| [set_LateStart](./set_latestart/) | Définit une valeur de LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Définit une valeur indiquant si LevelAssignments est défini ou non. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Définit une valeur indiquant si LevelingCanSplit est défini ou non. |
| [set_LevelingDelay](./set_levelingdelay/) | Définit une valeur de LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Définit une valeur de ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Définit une valeur de ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Définit une valeur de ManualStart. |
| [set_Name](./set_name/) | Définit une valeur de Name. |
| [set_NotesRTF](./set_notesrtf/) | Définit une valeur de NotesRTF. |
| [set_NotesText](./set_notestext/) | Définit une valeur de NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Définit l'objet OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Définit une valeur de OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Définit une valeur de OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Définit une valeur de OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Définit une valeur de OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Définit une valeur de PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Définit une valeur de PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Définit une valeur de PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Définit une valeur de PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Définit une valeur de PreleveledStart. |
| [set_Priority](./set_priority/) | Définit une valeur de Priority. |
| [set_RegularWork](./set_regularwork/) | Définit une valeur de RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Définit une valeur de RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Définit une valeur de RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Définit une valeur de RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Définit une valeur de RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Définit une valeur de RemainingWork. |
| [set_Resume](./set_resume/) | Définit une valeur de Resume. |
| [set_Start](./set_start/) | Définit une valeur de Start. |
| [set_StartSlack](./set_startslack/) | Définit une valeur de StartSlack. |
| [set_StartText](./set_starttext/) | Définit une valeur de StartText. |
| [set_StartVariance](./set_startvariance/) | Définit une valeur de StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Définit une valeur de StatusManager. |
| [set_Stop](./set_stop/) | Définit une valeur de Stop. |
| [set_SubprojectName](./set_subprojectname/) | Définit une valeur de SubprojectName. |
| [set_SV](./set_sv/) | La variance d'échéancier de la valeur acquise, jusqu'à la date d'état du projet. La variance d'échéancier (SV) est la différence entre le BCWP et le BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Définit un objet TimephasedDataCollection de cette tâche. Le bloc de données temporelles associé à une tâche. |
| [set_TotalSlack](./set_totalslack/) | Définit une valeur de TotalSlack. |
| [set_Type](./set_type/) | Définit une valeur de Type. |
| [set_Uid](./set_uid/) | Définit une valeur de Uid. |
| [set_Warning](./set_warning/) | Définit une valeur indiquant si Warning est défini ou non. |
| [set_WBS](./set_wbs/) | Définit une valeur de WBS. |
| [set_WBSLevel](./set_wbslevel/) | Définit une valeur de WBSLevel. |
| [set_Work](./set_work/) | Définit une valeur de Work. |
| [set_WorkVariance](./set_workvariance/) | Définit une valeur de WorkVariance. |
| [ToString](./tostring/) | Renvoie une représentation courte sous forme de chaîne d’une tâche. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer. |

