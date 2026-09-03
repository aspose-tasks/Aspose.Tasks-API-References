---
title: "Класс Aspose::Tasks::Task"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks для C++"
description: "Представляет задачу в проекте."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Представляет задачу в проекте.

Task представляет собой один атомарный блок работы.

Можно использовать Task для планирования проекта, создавая задачи и назначая им соответствующие ресурсы. Задачи в проекте организованы в корневую иерархическую структуру дерева, с корневой задачей и поддеревьями дочерних задач.

Чтобы построить дерево задач, можно использовать специализированную коллекцию Aspose::Tasks::TaskCollection, получая доступ к свойству Project::RootTask, например:

```cpp
Project project = new Project();
 
// добавить новые задачи
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
 
// сохранить проект в одном из доступных форматов
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Методы

| Имя | Описание |
| --- | --- |
| [Clone](./clone/) | Создаёт полную копию задачи без подзадач. |
| [Delete](./delete/) | Удаляет задачу из коллекции задач родительского проекта и все её назначения. |
| [Equals (2 overloads)](./equals/) | Возвращает значение, указывающее, равен ли этот экземпляр заданному объекту. |
| [Get](./get/) | Возвращает значение, к которому свойство сопоставлено в этом контейнере. |
| [get_ActivityId](./get_activityid/) | Представляет поле идентификатора активности — уникальный идентификатор задачи, используемый в Primavera. (применимо только к проектам Primavera). |
| [get_ActualCost](./get_actualcost/) | Получает значение ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Получает значение ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Получает значение ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Получает значение ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Получает значение ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Получает значение ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Получает значение ActualStart. |
| [get_ActualWork](./get_actualwork/) | Получает значение ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Получает значение ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Получает значение ACWP. |
| [get_Assignments](./get_assignments/) | Получает коллекцию назначений ресурсов для этого объекта. |
| [get_Baselines](./get_baselines/) | Получает коллекцию базовых значений задачи. |
| [get_BCWP](./get_bcwp/) | Получает значение BCWP. |
| [get_BCWS](./get_bcws/) | Получает значение BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Получает значение BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Получает значение BudgetWork. |
| [get_Calendar](./get_calendar/) | Получает значение Calendar. |
| [get_Children](./get_children/) | Получает коллекцию дочерних задач этого объекта. Объект TaskCollection, представляющий дочерние задачи. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Получает значение CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Получает значение CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Получает значение CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Получает значение ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Получает значение ConstraintType. |
| [get_Contact](./get_contact/) | Получает значение Contact. |
| [get_Cost](./get_cost/) | Получает значение Cost. |
| [get_CostVariance](./get_costvariance/) | Получает значение CostVariance. |
| [get_Created](./get_created/) | Получает значение Created. |
| [get_CV](./get_cv/) | Получает значение CV. |
| [get_Deadline](./get_deadline/) | Получает значение Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Получает значение, указывающее, установлен ли DisplayAsSummary. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Получает значение, указывающее, установлен ли DisplayOnTimeline. |
| [get_Duration](./get_duration/) | Получает значение Duration. |
| [get_DurationFormat](./get_durationformat/) | Получает значение DurationFormat. |
| [get_DurationText](./get_durationtext/) | Получает значение DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Получает значение DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Получает значение EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Получает значение EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Получает значение EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Получает объект ExtendedAttributeCollection, содержащий значения расширенного атрибута. |
| [get_ExternalId](./get_externalid/) | Получает значение ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Получает значение ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Получает или задает уникальный идентификатор внешней задачи, когда задача является внешней. |
| [get_Finish](./get_finish/) | Получает значение Finish. |
| [get_FinishSlack](./get_finishslack/) | Получает значение FinishSlack. |
| [get_FinishText](./get_finishtext/) | Получает значение FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Получает значение FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Получает значение FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Получает значение FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Получает значение FreeSlack. |
| [get_Guid](./get_guid/) | Получает значение Guid. |
| [get_HideBar](./get_hidebar/) | Получает значение, указывающее, установлен ли HideBar. |
| [get_Hyperlink](./get_hyperlink/) | Получает заголовок или пояснительный текст для гиперссылки, связанной с задачей. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Получает адрес гиперссылки, связанной с задачей. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Получает конкретное местоположение в документе в гиперссылке, связанной с задачей. |
| [get_Id](./get_id/) | Получает значение Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Получает значение, указывающее, установлен ли IgnoreResourceCalendar. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Получает значение, указывающее, установлен ли IgnoreWarnings. |
| [get_IsActive](./get_isactive/) | Получает значение, указывающее, установлен ли IsActive. |
| [get_IsCritical](./get_iscritical/) | Получает значение, указывающее, установлен ли IsCritical. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Получает значение, указывающее, установлен ли IsEffortDriven. |
| [get_IsEstimated](./get_isestimated/) | Получает значение, указывающее, установлен ли IsEstimated. |
| [get_IsExpanded](./get_isexpanded/) | Получает значение, указывающее, установлен ли IsExpanded. |
| [get_IsExternalTask](./get_isexternaltask/) | Получает значение, указывающее, установлен ли IsExternalTask. |
| [get_IsManual](./get_ismanual/) | Получает значение, указывающее, установлен ли IsManual. |
| [get_IsMarked](./get_ismarked/) | Получает значение, указывающее, установлен ли IsMarked. |
| [get_IsMilestone](./get_ismilestone/) | Получает значение, указывающее, установлен ли IsMilestone. |
| [get_IsNull](./get_isnull/) | Получает значение, указывающее, установлен ли IsNull. |
| [get_IsOverallocated](./get_isoverallocated/) | Получает значение, указывающее, установлен ли IsOverallocated. |
| [get_IsPublished](./get_ispublished/) | Получает значение, указывающее, установлен ли IsPublished. |
| [get_IsRecurring](./get_isrecurring/) | Получает значение, указывающее, установлен ли IsRecurring. |
| [get_IsResumeValid](./get_isresumevalid/) | Получает значение, указывающее, установлен ли IsResumeValid. |
| [get_IsRollup](./get_isrollup/) | Возвращает значение, указывающее, установлен ли IsRollup, или нет. |
| [get_IsSubproject](./get_issubproject/) | Возвращает значение, указывающее, установлен ли IsSubproject, или нет. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Возвращает значение, указывающее, установлен ли IsSubprojectReadOnly, или нет. |
| [get_IsSummary](./get_issummary/) | Возвращает значение, указывающее, установлен ли IsSummary, или нет. |
| [get_LateFinish](./get_latefinish/) | Возвращает значение LateFinish. |
| [get_LateStart](./get_latestart/) | Возвращает значение LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Возвращает значение, указывающее, установлен ли LevelAssignments, или нет. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Возвращает значение, указывающее, установлен ли LevelingCanSplit, или нет. |
| [get_LevelingDelay](./get_levelingdelay/) | Получает значение LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Возвращает значение ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Возвращает значение ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Возвращает значение ManualStart. |
| [get_Name](./get_name/) | Получает значение Name. |
| [get_NotesRTF](./get_notesrtf/) | Получает значение NotesRTF. |
| [get_NotesText](./get_notestext/) | Получает значение NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Возвращает объект OutlineCodeCollection. |
| [get_OutlineLevel](./get_outlinelevel/) | Возвращает значение OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Возвращает значение OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Получает значение OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Получает значение OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Возвращает родительский проект задачи. |
| [get_ParentTask](./get_parenttask/) | Возвращает родительскую задачу задачи. |
| [get_PercentComplete](./get_percentcomplete/) | Возвращает значение PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Получает значение PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Возвращает значение PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Возвращает объект TaskCollection, содержащий всех предшественников данного объекта Task. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Возвращает значение PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Возвращает значение PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Возвращает объект, содержащий свойства, специфичные для Primavera, задачи, считанные из файла Primavera. |
| [get_Priority](./get_priority/) | Возвращает значение Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Возвращает экземпляр класса RecurringTaskInfo для задачи, которая является повторяющейся; если задача не является повторяющейся, возвращает null; |
| [get_RegularWork](./get_regularwork/) | Получает значение RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Получает значение RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Возвращает значение RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Получает значение RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Получает значение RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Получает значение RemainingWork. |
| [get_Resume](./get_resume/) | Получает значение Resume. |
| [get_SplitParts](./get_splitparts/) | Получает коллекцию SplitPart, представляющую части задачи. |
| [get_Start](./get_start/) | Получает значение Start. |
| [get_StartSlack](./get_startslack/) | Получает значение StartSlack. |
| [get_StartText](./get_starttext/) | Получает значение StartText. |
| [get_StartVariance](./get_startvariance/) | Получает значение StartVariance. |
| [get_Status](./get_status/) | Получает статус задачи. |
| [get_StatusManager](./get_statusmanager/) | Получает значение StatusManager. |
| [get_Stop](./get_stop/) | Получает значение Stop. |
| [get_SubprojectName](./get_subprojectname/) | Получает значение SubprojectName. |
| [get_Successors](./get_successors/) | Получает объект TaskCollection, содержащий всех последователей этого объекта Task. |
| [get_SV](./get_sv/) | Отклонение графика заработанной стоимости до текущей даты статуса проекта. Отклонение графика (SV) — это разница между BCWP и BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Получает объект TimephasedDataCollection этой задачи. Блок данных, разбитых по времени, связанный с задачей. |
| [get_TotalSlack](./get_totalslack/) | Получает значение TotalSlack. |
| [get_Type](./get_type/) | Получает значение Type. |
| [get_Uid](./get_uid/) | Получает значение Uid. |
| [get_Warning](./get_warning/) | Получает значение, указывающее, установлен ли Warning. |
| [get_WBS](./get_wbs/) | Получает значение WBS. |
| [get_WBSLevel](./get_wbslevel/) | Получает значение WBSLevel. |
| [get_Work](./get_work/) | Получает значение Work. |
| [get_WorkVariance](./get_workvariance/) | Получает значение WorkVariance. |
| [GetHashCode](./gethashcode/) | Возвращает значение хеш-кода для этой задачи. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Возвращает объект TimephasedDataCollection со значениями TimephasedData в указанных начальной и конечной датах. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Перемещает текущую задачу на том же уровне Outline перед указанной задачей. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и стоимость, уровни Outline). Если ParentProject.CalculationMode имеет значение Manual, метод автоматически вычислит только идентификатор задачи, уровень Outline и номера Outline. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенесёт все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и стоимость, пересчитывает идентификаторы и уровни Outline). |
| [OutlineIndent](./outlineindent/) | Устанавливает отступ задачи в структуре outline. |
| [OutlineOutdent](./outlineoutdent/) | Поднимает задачу в структуре outline. |
| [SelectAllChildTasks](./selectallchildtasks/) | Рекурсивно собирает все дочерние задачи этой задачи. |
| [Set](./set/) | Отображает указанное свойство на указанное значение в этом контейнере. |
| [set_ActivityId](./set_activityid/) | Представляет поле идентификатора активности — уникальный идентификатор задачи, используемый в Primavera. (применимо только к проектам Primavera). |
| [set_ActualCost](./set_actualcost/) | Устанавливает значение ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Устанавливает значение ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Устанавливает значение ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Устанавливает значение ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Устанавливает значение ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Устанавливает значение ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Устанавливает значение ActualStart. |
| [set_ActualWork](./set_actualwork/) | Устанавливает значение ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Устанавливает значение ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Устанавливает значение ACWP. |
| [set_Baselines](./set_baselines/) | Устанавливает коллекцию базовых значений задачи. |
| [set_BCWP](./set_bcwp/) | Устанавливает значение BCWP. |
| [set_BCWS](./set_bcws/) | Устанавливает значение BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Устанавливает значение BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Устанавливает значение BudgetWork. |
| [set_Calendar](./set_calendar/) | Устанавливает значение Calendar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | Устанавливает значение CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Устанавливает значение CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Устанавливает значение CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Устанавливает значение ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Устанавливает значение ConstraintType. |
| [set_Contact](./set_contact/) | Устанавливает значение Contact. |
| [set_Cost](./set_cost/) | Устанавливает значение Cost. |
| [set_CostVariance](./set_costvariance/) | Устанавливает значение CostVariance. |
| [set_Created](./set_created/) | Устанавливает значение Created. |
| [set_CV](./set_cv/) | Устанавливает значение CV. |
| [set_Deadline](./set_deadline/) | Устанавливает значение Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Устанавливает значение, указывающее, установлен ли DisplayAsSummary или нет. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Устанавливает значение, указывающее, установлен ли DisplayOnTimeline или нет. |
| [set_Duration](./set_duration/) | Устанавливает значение Duration. |
| [set_DurationFormat](./set_durationformat/) | Устанавливает значение DurationFormat. |
| [set_DurationText](./set_durationtext/) | Устанавливает значение DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Устанавливает значение DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Устанавливает значение EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Устанавливает значение EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Устанавливает значение EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Устанавливает значение ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Устанавливает значение ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Получает или задает уникальный идентификатор внешней задачи, когда задача является внешней. |
| [set_Finish](./set_finish/) | Устанавливает значение Finish. |
| [set_FinishSlack](./set_finishslack/) | Устанавливает значение FinishSlack. |
| [set_FinishText](./set_finishtext/) | Устанавливает значение FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Устанавливает значение FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Устанавливает значение FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Устанавливает значение FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Устанавливает значение FreeSlack. |
| [set_Guid](./set_guid/) | Устанавливает значение Guid. |
| [set_HideBar](./set_hidebar/) | Устанавливает значение, указывающее, установлен ли HideBar или нет. |
| [set_Hyperlink](./set_hyperlink/) | Устанавливает заголовок или пояснительный текст для гиперссылки, связанной с задачей. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Устанавливает адрес гиперссылки, связанной с задачей. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Устанавливает конкретное место в документе в гиперссылке, связанной с задачей. |
| [set_Id](./set_id/) | Устанавливает значение Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Устанавливает значение, указывающее, установлен ли IgnoreResourceCalendar или нет. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Устанавливает значение, указывающее, установлен ли IgnoreWarnings или нет. |
| [set_IsActive](./set_isactive/) | Устанавливает значение, указывающее, установлен ли IsActive или нет. |
| [set_IsCritical](./set_iscritical/) | Устанавливает значение, указывающее, установлен ли IsCritical или нет. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Устанавливает значение, указывающее, установлен ли IsEffortDriven или нет. |
| [set_IsEstimated](./set_isestimated/) | Устанавливает значение, указывающее, установлен ли IsEstimated, или нет. |
| [set_IsExpanded](./set_isexpanded/) | Устанавливает значение, указывающее, установлен ли IsExpanded, или нет. |
| [set_IsExternalTask](./set_isexternaltask/) | Устанавливает значение, указывающее, установлен ли IsExternalTask, или нет. |
| [set_IsManual](./set_ismanual/) | Устанавливает значение, указывающее, установлен ли IsManual, или нет. |
| [set_IsMarked](./set_ismarked/) | Устанавливает значение, указывающее, установлен ли IsMarked, или нет. |
| [set_IsMilestone](./set_ismilestone/) | Устанавливает значение, указывающее, установлен ли IsMilestone, или нет. |
| [set_IsNull](./set_isnull/) | Устанавливает значение, указывающее, установлен ли IsNull или нет. |
| [set_IsOverallocated](./set_isoverallocated/) | Устанавливает значение, указывающее, установлен ли IsOverallocated, или нет. |
| [set_IsPublished](./set_ispublished/) | Устанавливает значение, указывающее, установлен ли IsPublished, или нет. |
| [set_IsRecurring](./set_isrecurring/) | Устанавливает значение, указывающее, установлен ли IsRecurring, или нет. |
| [set_IsResumeValid](./set_isresumevalid/) | Устанавливает значение, указывающее, установлен ли IsResumeValid, или нет. |
| [set_IsRollup](./set_isrollup/) | Устанавливает значение, указывающее, установлен ли IsRollup, или нет. |
| [set_IsSubproject](./set_issubproject/) | Устанавливает значение, указывающее, установлен ли IsSubproject, или нет. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Устанавливает значение, указывающее, установлен ли IsSubprojectReadOnly, или нет. |
| [set_IsSummary](./set_issummary/) | Устанавливает значение, указывающее, установлен ли IsSummary, или нет. |
| [set_LateFinish](./set_latefinish/) | Устанавливает значение LateFinish. |
| [set_LateStart](./set_latestart/) | Устанавливает значение LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Устанавливает значение, указывающее, установлен ли LevelAssignments, или нет. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Устанавливает значение, указывающее, установлен ли LevelingCanSplit, или нет. |
| [set_LevelingDelay](./set_levelingdelay/) | Устанавливает значение LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Устанавливает значение ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Устанавливает значение ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Устанавливает значение ManualStart. |
| [set_Name](./set_name/) | Устанавливает значение Name. |
| [set_NotesRTF](./set_notesrtf/) | Устанавливает значение NotesRTF. |
| [set_NotesText](./set_notestext/) | Устанавливает значение NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Устанавливает объект OutlineCodeCollection. |
| [set_OutlineLevel](./set_outlinelevel/) | Устанавливает значение OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Устанавливает значение OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Устанавливает значение OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Устанавливает значение OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Устанавливает значение PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Устанавливает значение PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Устанавливает значение PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Устанавливает значение PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Устанавливает значение PreleveledStart. |
| [set_Priority](./set_priority/) | Устанавливает значение Priority. |
| [set_RegularWork](./set_regularwork/) | Устанавливает значение RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Устанавливает значение RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Устанавливает значение RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Устанавливает значение RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Устанавливает значение RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Устанавливает значение RemainingWork. |
| [set_Resume](./set_resume/) | Устанавливает значение Resume. |
| [set_Start](./set_start/) | Устанавливает значение Start. |
| [set_StartSlack](./set_startslack/) | Устанавливает значение StartSlack. |
| [set_StartText](./set_starttext/) | Устанавливает значение StartText. |
| [set_StartVariance](./set_startvariance/) | Устанавливает значение StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Устанавливает значение StatusManager. |
| [set_Stop](./set_stop/) | Устанавливает значение Stop. |
| [set_SubprojectName](./set_subprojectname/) | Устанавливает значение SubprojectName. |
| [set_SV](./set_sv/) | Отклонение графика заработанной стоимости до текущей даты статуса проекта. Отклонение графика (SV) — это разница между BCWP и BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Устанавливает объект TimephasedDataCollection для этой задачи. Блок данных, разбитый по времени, связанный с задачей. |
| [set_TotalSlack](./set_totalslack/) | Устанавливает значение TotalSlack. |
| [set_Type](./set_type/) | Устанавливает значение Type. |
| [set_Uid](./set_uid/) | Устанавливает значение Uid. |
| [set_Warning](./set_warning/) | Устанавливает значение, указывающее, установлен ли Warning. |
| [set_WBS](./set_wbs/) | Устанавливает значение WBS. |
| [set_WBSLevel](./set_wbslevel/) | Устанавливает значение WBSLevel. |
| [set_Work](./set_work/) | Устанавливает значение Work. |
| [set_WorkVariance](./set_workvariance/) | Устанавливает значение WorkVariance. |
| [ToString](./tostring/) | Возвращает короткое строковое представление задачи. Точные детали представления не указаны и могут изменяться. |

