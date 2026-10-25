---
title: "Aspose::Tasks::Task 클래스"
linktitle: "Task"
articleTitle: "Task"
second_title: "C++용 Aspose.Tasks"
description: "프로젝트의 작업을 나타냅니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

프로젝트의 작업을 나타냅니다.

Task는 하나의 원자적 작업 단위를 나타냅니다.

Task를 사용하여 작업을 생성하고 적절한 리소스를 할당함으로써 프로젝트를 계획할 수 있습니다. 프로젝트의 작업은 루트 작업과 하위 작업 트리로 구성된 계층적 트리 구조로 조직됩니다.

작업 트리를 구축하려면 Project::RootTask 속성에 접근하여 특수 컬렉션 Aspose::Tasks::TaskCollection을 사용할 수 있습니다. 예:

```cpp
Project project = new Project();
 
// 새 작업 추가
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
 
// 프로젝트를 사용 가능한 형식 중 하나로 저장합니다
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Clone](./clone/) | 하위 작업 없이 작업의 전체 복사본을 생성합니다. |
| [Delete](./delete/) | 부모 프로젝트 작업 컬렉션에서 작업을 삭제하고 해당 할당을 모두 제거합니다. |
| [Equals (2 overloads)](./equals/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [Get](./get/) | 이 컨테이너에서 속성이 매핑되는 값을 반환합니다. |
| [get_ActivityId](./get_activityid/) | 활동 ID 필드를 나타냅니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. (Primavera 프로젝트에만 적용됩니다.) |
| [get_ActualCost](./get_actualcost/) | ActualCost 값을 가져옵니다. |
| [get_ActualDuration](./get_actualduration/) | ActualDuration 값을 가져옵니다. |
| [get_ActualFinish](./get_actualfinish/) | ActualFinish 의 값을 가져옵니다. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | ActualOvertimeCost의 값을 가져옵니다. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | ActualOvertimeWork의 값을 가져옵니다. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | ActualOvertimeWorkProtected의 값을 가져옵니다. |
| [get_ActualStart](./get_actualstart/) | ActualStart 의 값을 가져옵니다. |
| [get_ActualWork](./get_actualwork/) | ActualWork의 값을 가져옵니다. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | ActualWorkProtected의 값을 가져옵니다. |
| [get_ACWP](./get_acwp/) | ACWP의 값을 가져옵니다. |
| [get_Assignments](./get_assignments/) | 이 객체에 대한 리소스 할당 컬렉션을 가져옵니다. |
| [get_Baselines](./get_baselines/) | 작업의 기준값 컬렉션을 가져옵니다. |
| [get_BCWP](./get_bcwp/) | BCWP의 값을 가져옵니다. |
| [get_BCWS](./get_bcws/) | BCWS의 값을 가져옵니다. |
| [get_BudgetCost](./get_budgetcost/) | BudgetCost의 값을 가져옵니다. |
| [get_BudgetWork](./get_budgetwork/) | BudgetWork의 값을 가져옵니다. |
| [get_Calendar](./get_calendar/) | Calendar의 값을 가져옵니다. |
| [get_Children](./get_children/) | 이 객체의 하위 작업 컬렉션을 가져옵니다. 하위 작업을 나타내는 TaskCollection 객체입니다. |
| [get_CommitmentFinish](./get_commitmentfinish/) | CommitmentFinish 값을 가져옵니다. |
| [get_CommitmentStart](./get_commitmentstart/) | CommitmentStart 값을 가져옵니다. |
| [get_CommitmentType](./get_commitmenttype/) | CommitmentType 값을 가져옵니다. |
| [get_ConstraintDate](./get_constraintdate/) | ConstraintDate 값을 가져옵니다. |
| [get_ConstraintType](./get_constrainttype/) | ConstraintType 값을 가져옵니다. |
| [get_Contact](./get_contact/) | Contact 값을 가져옵니다. |
| [get_Cost](./get_cost/) | Cost의 값을 가져옵니다. |
| [get_CostVariance](./get_costvariance/) | CostVariance의 값을 가져옵니다. |
| [get_Created](./get_created/) | Created의 값을 가져옵니다. |
| [get_CV](./get_cv/) | CV의 값을 가져옵니다. |
| [get_Deadline](./get_deadline/) | Deadline 값을 가져옵니다. |
| [get_DisplayAsSummary](./get_displayassummary/) | DisplayAsSummary가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | DisplayOnTimeline이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_Duration](./get_duration/) | Duration 값을 가져옵니다. |
| [get_DurationFormat](./get_durationformat/) | DurationFormat의 값을 가져옵니다. |
| [get_DurationText](./get_durationtext/) | DurationText 값을 가져옵니다. |
| [get_DurationVariance](./get_durationvariance/) | DurationVariance 값을 가져옵니다. |
| [get_EarlyFinish](./get_earlyfinish/) | EarlyFinish 값을 가져옵니다. |
| [get_EarlyStart](./get_earlystart/) | EarlyStart 값을 가져옵니다. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod의 값을 가져옵니다. |
| [get_ExtendedAttributes](./get_extendedattributes/) | 확장 속성의 값을 포함하는 ExtendedAttributeCollection 객체를 가져옵니다. |
| [get_ExternalId](./get_externalid/) | ExternalId 값을 가져옵니다. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | ExternalTaskProject 값을 가져옵니다. |
| [get_ExternalUid](./get_externaluid/) | 작업이 외부인 경우 외부 작업의 고유 식별자를 가져오거나 설정합니다. |
| [get_Finish](./get_finish/) | Finish의 값을 가져옵니다. |
| [get_FinishSlack](./get_finishslack/) | FinishSlack 값을 가져옵니다. |
| [get_FinishText](./get_finishtext/) | FinishText 값을 가져옵니다. |
| [get_FinishVariance](./get_finishvariance/) | FinishVariance 의 값을 가져옵니다. |
| [get_FixedCost](./get_fixedcost/) | FixedCost 값을 가져옵니다. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | FixedCostAccrual 값을 가져옵니다. |
| [get_FreeSlack](./get_freeslack/) | FreeSlack 값을 가져옵니다. |
| [get_Guid](./get_guid/) | Guid의 값을 가져옵니다. |
| [get_HideBar](./get_hidebar/) | HideBar가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_Hyperlink](./get_hyperlink/) | 작업과 연결된 하이퍼링크의 제목 또는 설명 텍스트를 가져옵니다. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | 작업과 연결된 하이퍼링크의 주소를 가져옵니다. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | 작업과 연결된 하이퍼링크의 문서 내 특정 위치를 가져옵니다. |
| [get_Id](./get_id/) | Id의 값을 가져옵니다. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | IgnoreResourceCalendar가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | IgnoreWarnings가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsActive](./get_isactive/) | IsActive가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsCritical](./get_iscritical/) | IsCritical가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsEffortDriven](./get_iseffortdriven/) | IsEffortDriven가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsEstimated](./get_isestimated/) | IsEstimated가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsExpanded](./get_isexpanded/) | IsExpanded가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsExternalTask](./get_isexternaltask/) | IsExternalTask가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsManual](./get_ismanual/) | IsManual이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsMarked](./get_ismarked/) | IsMarked가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsMilestone](./get_ismilestone/) | IsMilestone이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsNull](./get_isnull/) | IsNull이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsOverallocated](./get_isoverallocated/) | IsOverallocated가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsPublished](./get_ispublished/) | IsPublished가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsRecurring](./get_isrecurring/) | IsRecurring이 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsResumeValid](./get_isresumevalid/) | IsResumeValid가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsRollup](./get_isrollup/) | IsRollup이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsSubproject](./get_issubproject/) | IsSubproject가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | IsSubprojectReadOnly가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_IsSummary](./get_issummary/) | IsSummary이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_LateFinish](./get_latefinish/) | LateFinish 값을 가져옵니다. |
| [get_LateStart](./get_latestart/) | LateStart 값을 가져옵니다. |
| [get_LevelAssignments](./get_levelassignments/) | LevelAssignments가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | LevelingCanSplit이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_LevelingDelay](./get_levelingdelay/) | LevelingDelay의 값을 가져옵니다. |
| [get_ManualDuration](./get_manualduration/) | ManualDuration 값을 가져옵니다. |
| [get_ManualFinish](./get_manualfinish/) | ManualFinish 값을 가져옵니다. |
| [get_ManualStart](./get_manualstart/) | ManualStart 값을 가져옵니다. |
| [get_Name](./get_name/) | Name의 값을 가져옵니다. |
| [get_NotesRTF](./get_notesrtf/) | NotesRTF의 값을 가져옵니다. |
| [get_NotesText](./get_notestext/) | NotesText의 값을 가져옵니다. |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeCollection 객체를 가져옵니다. |
| [get_OutlineLevel](./get_outlinelevel/) | OutlineLevel 값을 가져옵니다. |
| [get_OutlineNumber](./get_outlinenumber/) | OutlineNumber 값을 가져옵니다. |
| [get_OvertimeCost](./get_overtimecost/) | OvertimeCost 값을 가져옵니다. |
| [get_OvertimeWork](./get_overtimework/) | OvertimeWork 값을 가져옵니다. |
| [get_ParentProject](./get_parentproject/) | 작업의 상위 프로젝트를 가져옵니다. |
| [get_ParentTask](./get_parenttask/) | 작업의 상위 작업을 가져옵니다. |
| [get_PercentComplete](./get_percentcomplete/) | PercentComplete 값을 가져옵니다. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | PercentWorkComplete 값을 가져옵니다. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | PhysicalPercentComplete 값을 가져옵니다. |
| [get_Predecessors](./get_predecessors/) | 이 Task 객체의 모든 선행 작업을 포함하는 TaskCollection 객체를 가져옵니다. |
| [get_PreleveledFinish](./get_preleveledfinish/) | PreleveledFinish 값을 가져옵니다. |
| [get_PreleveledStart](./get_preleveledstart/) | PreleveledStart 값을 가져옵니다. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera 파일에서 읽은 작업에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
| [get_Priority](./get_priority/) | Priority 값을 가져옵니다. |
| [get_RecurringInfo](./get_recurringinfo/) | 반복 작업인 작업에 대한 RecurringTaskInfo 클래스 인스턴스를 가져옵니다; 작업이 반복 작업이 아니면 null을 반환합니다; |
| [get_RegularWork](./get_regularwork/) | RegularWork 값을 가져옵니다. |
| [get_RemainingCost](./get_remainingcost/) | RemainingCost 값을 가져옵니다. |
| [get_RemainingDuration](./get_remainingduration/) | RemainingDuration 값을 가져옵니다. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | RemainingOvertimeCost 값을 가져옵니다. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | RemainingOvertimeWork 값을 가져옵니다. |
| [get_RemainingWork](./get_remainingwork/) | RemainingWork 값을 가져옵니다. |
| [get_Resume](./get_resume/) | Resume의 값을 가져옵니다. |
| [get_SplitParts](./get_splitparts/) | 작업의 부분을 나타내는 SplitPart 컬렉션을 가져옵니다. |
| [get_Start](./get_start/) | Start 값을 가져옵니다. |
| [get_StartSlack](./get_startslack/) | StartSlack 값을 가져옵니다. |
| [get_StartText](./get_starttext/) | StartText 값을 가져옵니다. |
| [get_StartVariance](./get_startvariance/) | StartVariance의 값을 가져옵니다. |
| [get_Status](./get_status/) | 작업 상태를 가져옵니다. |
| [get_StatusManager](./get_statusmanager/) | StatusManager 값을 가져옵니다. |
| [get_Stop](./get_stop/) | Stop의 값을 가져옵니다. |
| [get_SubprojectName](./get_subprojectname/) | SubprojectName 값을 가져옵니다. |
| [get_Successors](./get_successors/) | 이 Task 객체의 모든 후속 작업을 포함하는 TaskCollection 객체를 가져옵니다. |
| [get_SV](./get_sv/) | 프로젝트 상태 날짜까지의 획득 가치 일정 편차. 일정 편차(SV)는 BCWP와 BCWS 사이의 차이입니다. |
| [get_TimephasedData](./get_timephaseddata/) | 이 작업의 TimephasedDataCollection 객체를 가져옵니다. 작업과 연결된 시간 구분 데이터 블록입니다. |
| [get_TotalSlack](./get_totalslack/) | TotalSlack 값을 가져옵니다. |
| [get_Type](./get_type/) | Type 값을 가져옵니다. |
| [get_Uid](./get_uid/) | Uid 값을 가져옵니다. |
| [get_Warning](./get_warning/) | Warning이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [get_WBS](./get_wbs/) | WBS 값을 가져옵니다. |
| [get_WBSLevel](./get_wbslevel/) | WBSLevel 값을 가져옵니다. |
| [get_Work](./get_work/) | Work 값을 가져옵니다. |
| [get_WorkVariance](./get_workvariance/) | WorkVariance의 값을 가져옵니다. |
| [GetHashCode](./gethashcode/) | 이 Task에 대한 해시 코드 값을 반환합니다. |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | 주어진 시작 및 종료 날짜 범위 내의 TimephasedData 값을 포함하는 TimephasedDataCollection 객체를 반환합니다. |
| [MoveToSibling (2 overloads)](./movetosibling/) | 현재 작업을 동일한 Outline Level에서 지정된 작업 앞에 이동합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(이렇게 하면 모든 프로젝트 작업(시작/완료 날짜, 조기/지연 날짜 설정)이 재조정되고, 슬랙, 작업 및 비용 필드, Outline Level과 같은 종속 필드가 계산됩니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, Outline Level 및 Outline 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/완료 날짜, 조기/지연 날짜 설정, 슬랙, 작업 및 비용 필드 계산, ID와 Outline Level 재계산). |
| [OutlineIndent](./outlineindent/) | 작업을 개요에서 들여쓰기합니다. |
| [OutlineOutdent](./outlineoutdent/) | 작업을 개요에서 승격합니다. |
| [SelectAllChildTasks](./selectallchildtasks/) | 이 작업의 모든 하위 작업을 재귀적으로 수집합니다. |
| [Set](./set/) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [set_ActivityId](./set_activityid/) | 활동 ID 필드를 나타냅니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. (Primavera 프로젝트에만 적용됩니다.) |
| [set_ActualCost](./set_actualcost/) | ActualCost의 값을 설정합니다. |
| [set_ActualDuration](./set_actualduration/) | ActualDuration 값을 설정합니다. |
| [set_ActualFinish](./set_actualfinish/) | ActualFinish의 값을 설정합니다. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | ActualOvertimeCost의 값을 설정합니다. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | ActualOvertimeWork의 값을 설정합니다. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | ActualOvertimeWorkProtected의 값을 설정합니다. |
| [set_ActualStart](./set_actualstart/) | ActualStart의 값을 설정합니다. |
| [set_ActualWork](./set_actualwork/) | ActualWork의 값을 설정합니다. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | ActualWorkProtected의 값을 설정합니다. |
| [set_ACWP](./set_acwp/) | ACWP의 값을 설정합니다. |
| [set_Baselines](./set_baselines/) | 작업의 기준값 컬렉션을 설정합니다. |
| [set_BCWP](./set_bcwp/) | BCWP의 값을 설정합니다. |
| [set_BCWS](./set_bcws/) | BCWS의 값을 설정합니다. |
| [set_BudgetCost](./set_budgetcost/) | BudgetCost의 값을 설정합니다. |
| [set_BudgetWork](./set_budgetwork/) | BudgetWork의 값을 설정합니다. |
| [set_Calendar](./set_calendar/) | Calendar의 값을 설정합니다. |
| [set_CommitmentFinish](./set_commitmentfinish/) | CommitmentFinish 값을 설정합니다. |
| [set_CommitmentStart](./set_commitmentstart/) | CommitmentStart 값을 설정합니다. |
| [set_CommitmentType](./set_commitmenttype/) | CommitmentType 값을 설정합니다. |
| [set_ConstraintDate](./set_constraintdate/) | ConstraintDate 값을 설정합니다. |
| [set_ConstraintType](./set_constrainttype/) | ConstraintType 값을 설정합니다. |
| [set_Contact](./set_contact/) | Contact의 값을 설정합니다. |
| [set_Cost](./set_cost/) | Cost의 값을 설정합니다. |
| [set_CostVariance](./set_costvariance/) | CostVariance의 값을 설정합니다. |
| [set_Created](./set_created/) | Created의 값을 설정합니다. |
| [set_CV](./set_cv/) | CV의 값을 설정합니다. |
| [set_Deadline](./set_deadline/) | Deadline의 값을 설정합니다. |
| [set_DisplayAsSummary](./set_displayassummary/) | DisplayAsSummary가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | DisplayOnTimeline이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Duration](./set_duration/) | Duration의 값을 설정합니다. |
| [set_DurationFormat](./set_durationformat/) | DurationFormat의 값을 설정합니다. |
| [set_DurationText](./set_durationtext/) | DurationText의 값을 설정합니다. |
| [set_DurationVariance](./set_durationvariance/) | DurationVariance의 값을 설정합니다. |
| [set_EarlyFinish](./set_earlyfinish/) | EarlyFinish의 값을 설정합니다. |
| [set_EarlyStart](./set_earlystart/) | EarlyStart의 값을 설정합니다. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod의 값을 설정합니다. |
| [set_ExternalId](./set_externalid/) | ExternalId의 값을 설정합니다. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | ExternalTaskProject의 값을 설정합니다. |
| [set_ExternalUid](./set_externaluid/) | 작업이 외부인 경우 외부 작업의 고유 식별자를 가져오거나 설정합니다. |
| [set_Finish](./set_finish/) | Finish의 값을 설정합니다. |
| [set_FinishSlack](./set_finishslack/) | FinishSlack의 값을 설정합니다. |
| [set_FinishText](./set_finishtext/) | FinishText의 값을 설정합니다. |
| [set_FinishVariance](./set_finishvariance/) | FinishVariance의 값을 설정합니다. |
| [set_FixedCost](./set_fixedcost/) | FixedCost의 값을 설정합니다. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | FixedCostAccrual의 값을 설정합니다. |
| [set_FreeSlack](./set_freeslack/) | FreeSlack의 값을 설정합니다. |
| [set_Guid](./set_guid/) | Guid의 값을 설정합니다. |
| [set_HideBar](./set_hidebar/) | HideBar가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_Hyperlink](./set_hyperlink/) | 작업과 연결된 하이퍼링크의 제목 또는 설명 텍스트를 설정합니다. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | 작업과 연결된 하이퍼링크의 주소를 설정합니다. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | 작업과 연결된 하이퍼링크의 문서 내 특정 위치를 설정합니다. |
| [set_Id](./set_id/) | Id의 값을 설정합니다. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | IgnoreResourceCalendar가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | IgnoreWarnings가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsActive](./set_isactive/) | IsActive가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsCritical](./set_iscritical/) | IsCritical가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsEffortDriven](./set_iseffortdriven/) | IsEffortDriven가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsEstimated](./set_isestimated/) | IsEstimated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsExpanded](./set_isexpanded/) | IsExpanded가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsExternalTask](./set_isexternaltask/) | IsExternalTask가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsManual](./set_ismanual/) | IsManual가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsMarked](./set_ismarked/) | IsMarked가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsMilestone](./set_ismilestone/) | IsMilestone가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsNull](./set_isnull/) | IsNull가 설정되어 있는지 여부를 나타내는 값을 설정합니다. |
| [set_IsOverallocated](./set_isoverallocated/) | IsOverallocated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsPublished](./set_ispublished/) | IsPublished가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsRecurring](./set_isrecurring/) | IsRecurring가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsResumeValid](./set_isresumevalid/) | IsResumeValid가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsRollup](./set_isrollup/) | IsRollup가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsSubproject](./set_issubproject/) | IsSubproject가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | IsSubprojectReadOnly가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_IsSummary](./set_issummary/) | IsSummary가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_LateFinish](./set_latefinish/) | LateFinish 값을 설정합니다. |
| [set_LateStart](./set_latestart/) | LateStart 값을 설정합니다. |
| [set_LevelAssignments](./set_levelassignments/) | LevelAssignments가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | LevelingCanSplit가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_LevelingDelay](./set_levelingdelay/) | LevelingDelay의 값을 설정합니다. |
| [set_ManualDuration](./set_manualduration/) | ManualDuration 값을 설정합니다. |
| [set_ManualFinish](./set_manualfinish/) | ManualFinish 값을 설정합니다. |
| [set_ManualStart](./set_manualstart/) | ManualStart 값을 설정합니다. |
| [set_Name](./set_name/) | Name의 값을 설정합니다. |
| [set_NotesRTF](./set_notesrtf/) | NotesRTF의 값을 설정합니다. |
| [set_NotesText](./set_notestext/) | NotesText의 값을 설정합니다. |
| [set_OutlineCodes](./set_outlinecodes/) | OutlineCodeCollection 객체를 설정합니다. |
| [set_OutlineLevel](./set_outlinelevel/) | OutlineLevel 값을 설정합니다. |
| [set_OutlineNumber](./set_outlinenumber/) | OutlineNumber 값을 설정합니다. |
| [set_OvertimeCost](./set_overtimecost/) | OvertimeCost의 값을 설정합니다. |
| [set_OvertimeWork](./set_overtimework/) | OvertimeWork의 값을 설정합니다. |
| [set_PercentComplete](./set_percentcomplete/) | PercentComplete 값을 설정합니다. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | PercentWorkComplete의 값을 설정합니다. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | PhysicalPercentComplete의 값을 설정합니다. |
| [set_PreleveledFinish](./set_preleveledfinish/) | PreleveledFinish의 값을 설정합니다. |
| [set_PreleveledStart](./set_preleveledstart/) | PreleveledStart의 값을 설정합니다. |
| [set_Priority](./set_priority/) | Priority의 값을 설정합니다. |
| [set_RegularWork](./set_regularwork/) | RegularWork의 값을 설정합니다. |
| [set_RemainingCost](./set_remainingcost/) | RemainingCost의 값을 설정합니다. |
| [set_RemainingDuration](./set_remainingduration/) | RemainingDuration의 값을 설정합니다. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | RemainingOvertimeCost의 값을 설정합니다. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | RemainingOvertimeWork의 값을 설정합니다. |
| [set_RemainingWork](./set_remainingwork/) | RemainingWork의 값을 설정합니다. |
| [set_Resume](./set_resume/) | Resume의 값을 설정합니다. |
| [set_Start](./set_start/) | Start의 값을 설정합니다. |
| [set_StartSlack](./set_startslack/) | StartSlack의 값을 설정합니다. |
| [set_StartText](./set_starttext/) | StartText의 값을 설정합니다. |
| [set_StartVariance](./set_startvariance/) | StartVariance의 값을 설정합니다. |
| [set_StatusManager](./set_statusmanager/) | StatusManager의 값을 설정합니다. |
| [set_Stop](./set_stop/) | Stop의 값을 설정합니다. |
| [set_SubprojectName](./set_subprojectname/) | SubprojectName의 값을 설정합니다. |
| [set_SV](./set_sv/) | 프로젝트 상태 날짜까지의 획득 가치 일정 편차. 일정 편차(SV)는 BCWP와 BCWS 사이의 차이입니다. |
| [set_TimephasedData](./set_timephaseddata/) | 이 작업의 TimephasedDataCollection 객체를 설정합니다. 작업과 연결된 시간 단계 데이터 블록입니다. |
| [set_TotalSlack](./set_totalslack/) | TotalSlack의 값을 설정합니다. |
| [set_Type](./set_type/) | Type의 값을 설정합니다. |
| [set_Uid](./set_uid/) | Uid의 값을 설정합니다. |
| [set_Warning](./set_warning/) | Warning이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [set_WBS](./set_wbs/) | WBS의 값을 설정합니다. |
| [set_WBSLevel](./set_wbslevel/) | WBSLevel의 값을 설정합니다. |
| [set_Work](./set_work/) | Work의 값을 설정합니다. |
| [set_WorkVariance](./set_workvariance/) | WorkVariance의 값을 설정합니다. |
| [ToString](./tostring/) | 작업의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다. |

