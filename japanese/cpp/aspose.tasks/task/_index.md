---
title: "Aspose::Tasks::Task クラス"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks for C++"
description: "プロジェクト内のタスクを表します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

プロジェクト内のタスクを表します。

Task は作業の単一の原子的なチャンクを表します。

Task を使用してタスクを作成し、適切なリソースを割り当てることでプロジェクトを計画できます。プロジェクト内のタスクは、ルートタスクと子タスクのサブツリーからなる階層的なツリー構造として構成されます。

タスクのツリーを構築するには、Project::RootTask プロパティにアクセスして、専門のコレクション Aspose::Tasks::TaskCollection を使用できます。例:

```cpp
Project project = new Project();
 
// 新しいタスクを追加する
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
 
// 利用可能な形式のいずれかでプロジェクトを保存する
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Clone](./clone/) | サブタスクなしでタスクの完全なコピーを作成します。 |
| [Delete](./delete/) | 親プロジェクトのタスクコレクションからタスクとそのすべての割り当てを削除します。 |
| [Equals (2 overloads)](./equals/) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [Get](./get/) | このコンテナ内でプロパティがマッピングされている値を返します。 |
| [get_ActivityId](./get_activityid/) | アクティビティ ID フィールドを表します - Primavera で使用されるタスクの固有識別子です。（Primavera プロジェクトにのみ適用されます） |
| [get_ActualCost](./get_actualcost/) | ActualCost の値を取得します。 |
| [get_ActualDuration](./get_actualduration/) | ActualDuration の値を取得します。 |
| [get_ActualFinish](./get_actualfinish/) | ActualFinish の値を取得します。 |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | ActualOvertimeCost の値を取得します。 |
| [get_ActualOvertimeWork](./get_actualovertimework/) | ActualOvertimeWork の値を取得します。 |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | ActualOvertimeWorkProtected の値を取得します。 |
| [get_ActualStart](./get_actualstart/) | ActualStart の値を取得します。 |
| [get_ActualWork](./get_actualwork/) | ActualWork の値を取得します。 |
| [get_ActualWorkProtected](./get_actualworkprotected/) | ActualWorkProtected の値を取得します。 |
| [get_ACWP](./get_acwp/) | ACWP の値を取得します。 |
| [get_Assignments](./get_assignments/) | このオブジェクトのリソース割り当てのコレクションを取得します。 |
| [get_Baselines](./get_baselines/) | タスクのベースライン値のコレクションを取得します。 |
| [get_BCWP](./get_bcwp/) | BCWP の値を取得します。 |
| [get_BCWS](./get_bcws/) | BCWS の値を取得します。 |
| [get_BudgetCost](./get_budgetcost/) | BudgetCost の値を取得します。 |
| [get_BudgetWork](./get_budgetwork/) | BudgetWork の値を取得します。 |
| [get_Calendar](./get_calendar/) | Calendar の値を取得します。 |
| [get_Children](./get_children/) | このオブジェクトの子タスクコレクションを取得します。子タスクを表す TaskCollection オブジェクトです。 |
| [get_CommitmentFinish](./get_commitmentfinish/) | CommitmentFinish の値を取得します。 |
| [get_CommitmentStart](./get_commitmentstart/) | CommitmentStart の値を取得します。 |
| [get_CommitmentType](./get_commitmenttype/) | CommitmentType の値を取得します。 |
| [get_ConstraintDate](./get_constraintdate/) | ConstraintDate の値を取得します。 |
| [get_ConstraintType](./get_constrainttype/) | ConstraintType の値を取得します。 |
| [get_Contact](./get_contact/) | Contact の値を取得します。 |
| [get_Cost](./get_cost/) | Cost の値を取得します。 |
| [get_CostVariance](./get_costvariance/) | CostVariance の値を取得します。 |
| [get_Created](./get_created/) | Created の値を取得します。 |
| [get_CV](./get_cv/) | CV の値を取得します。 |
| [get_Deadline](./get_deadline/) | Deadline の値を取得します。 |
| [get_DisplayAsSummary](./get_displayassummary/) | DisplayAsSummary が設定されているかどうかを示す値を取得します。 |
| [get_DisplayOnTimeline](./get_displayontimeline/) | DisplayOnTimeline が設定されているかどうかを示す値を取得します。 |
| [get_Duration](./get_duration/) | Duration の値を取得します。 |
| [get_DurationFormat](./get_durationformat/) | DurationFormat の値を取得します。 |
| [get_DurationText](./get_durationtext/) | DurationText の値を取得します。 |
| [get_DurationVariance](./get_durationvariance/) | DurationVariance の値を取得します。 |
| [get_EarlyFinish](./get_earlyfinish/) | EarlyFinish の値を取得します。 |
| [get_EarlyStart](./get_earlystart/) | EarlyStart の値を取得します。 |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod の値を取得します。 |
| [get_ExtendedAttributes](./get_extendedattributes/) | 拡張属性の値を含む ExtendedAttributeCollection オブジェクトを取得します。 |
| [get_ExternalId](./get_externalid/) | ExternalId の値を取得します。 |
| [get_ExternalTaskProject](./get_externaltaskproject/) | ExternalTaskProject の値を取得します。 |
| [get_ExternalUid](./get_externaluid/) | 外部タスクが外部の場合に、外部タスクの一意の識別子を取得または設定します。 |
| [get_Finish](./get_finish/) | Finish の値を取得します。 |
| [get_FinishSlack](./get_finishslack/) | FinishSlack の値を取得します。 |
| [get_FinishText](./get_finishtext/) | FinishText の値を取得します。 |
| [get_FinishVariance](./get_finishvariance/) | FinishVariance の値を取得します。 |
| [get_FixedCost](./get_fixedcost/) | FixedCost の値を取得します。 |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | FixedCostAccrual の値を取得します。 |
| [get_FreeSlack](./get_freeslack/) | FreeSlack の値を取得します。 |
| [get_Guid](./get_guid/) | Guid の値を取得します。 |
| [get_HideBar](./get_hidebar/) | HideBar が設定されているかどうかを示す値を取得します。 |
| [get_Hyperlink](./get_hyperlink/) | タスクに関連付けられたハイパーリンクのタイトルまたは説明テキストを取得します。 |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | タスクに関連付けられたハイパーリンクのアドレスを取得します。 |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | タスクに関連付けられたハイパーリンク内のドキュメントの特定の場所を取得します。 |
| [get_Id](./get_id/) | Id の値を取得します。 |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | IgnoreResourceCalendar が設定されているかどうかを示す値を取得します。 |
| [get_IgnoreWarnings](./get_ignorewarnings/) | IgnoreWarnings が設定されているかどうかを示す値を取得します。 |
| [get_IsActive](./get_isactive/) | IsActive が設定されているかどうかを示す値を取得します。 |
| [get_IsCritical](./get_iscritical/) | IsCritical が設定されているかどうかを示す値を取得します。 |
| [get_IsEffortDriven](./get_iseffortdriven/) | IsEffortDriven が設定されているかどうかを示す値を取得します。 |
| [get_IsEstimated](./get_isestimated/) | IsEstimated が設定されているかどうかを示す値を取得します。 |
| [get_IsExpanded](./get_isexpanded/) | IsExpanded が設定されているかどうかを示す値を取得します。 |
| [get_IsExternalTask](./get_isexternaltask/) | IsExternalTask が設定されているかどうかを示す値を取得します。 |
| [get_IsManual](./get_ismanual/) | IsManual が設定されているかどうかを示す値を取得します。 |
| [get_IsMarked](./get_ismarked/) | IsMarked が設定されているかどうかを示す値を取得します。 |
| [get_IsMilestone](./get_ismilestone/) | IsMilestone が設定されているかどうかを示す値を取得します。 |
| [get_IsNull](./get_isnull/) | IsNull が設定されているかどうかを示す値を取得します。 |
| [get_IsOverallocated](./get_isoverallocated/) | IsOverallocated が設定されているかどうかを示す値を取得します。 |
| [get_IsPublished](./get_ispublished/) | IsPublished が設定されているかどうかを示す値を取得します。 |
| [get_IsRecurring](./get_isrecurring/) | IsRecurring が設定されているかどうかを示す値を取得します。 |
| [get_IsResumeValid](./get_isresumevalid/) | IsResumeValid が設定されているかどうかを示す値を取得します。 |
| [get_IsRollup](./get_isrollup/) | IsRollup が設定されているかどうかを示す値を取得します。 |
| [get_IsSubproject](./get_issubproject/) | IsSubproject が設定されているかどうかを示す値を取得します。 |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | IsSubprojectReadOnly が設定されているかどうかを示す値を取得します。 |
| [get_IsSummary](./get_issummary/) | IsSummary が設定されているかどうかを示す値を取得します。 |
| [get_LateFinish](./get_latefinish/) | LateFinish の値を取得します。 |
| [get_LateStart](./get_latestart/) | LateStart の値を取得します。 |
| [get_LevelAssignments](./get_levelassignments/) | LevelAssignments が設定されているかどうかを示す値を取得します。 |
| [get_LevelingCanSplit](./get_levelingcansplit/) | LevelingCanSplit が設定されているかどうかを示す値を取得します。 |
| [get_LevelingDelay](./get_levelingdelay/) | LevelingDelay の値を取得します。 |
| [get_ManualDuration](./get_manualduration/) | ManualDuration の値を取得します。 |
| [get_ManualFinish](./get_manualfinish/) | ManualFinish の値を取得します。 |
| [get_ManualStart](./get_manualstart/) | ManualStart の値を取得します。 |
| [get_Name](./get_name/) | Name の値を取得します。 |
| [get_NotesRTF](./get_notesrtf/) | NotesRTF の値を取得します。 |
| [get_NotesText](./get_notestext/) | NotesText の値を取得します。 |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeCollection オブジェクトを取得します。 |
| [get_OutlineLevel](./get_outlinelevel/) | OutlineLevel の値を取得します。 |
| [get_OutlineNumber](./get_outlinenumber/) | OutlineNumber の値を取得します。 |
| [get_OvertimeCost](./get_overtimecost/) | OvertimeCost の値を取得します。 |
| [get_OvertimeWork](./get_overtimework/) | OvertimeWork の値を取得します。 |
| [get_ParentProject](./get_parentproject/) | タスクの親プロジェクトを取得します。 |
| [get_ParentTask](./get_parenttask/) | タスクの親タスクを取得します。 |
| [get_PercentComplete](./get_percentcomplete/) | PercentComplete の値を取得します。 |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | PercentWorkComplete の値を取得します。 |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | PhysicalPercentComplete の値を取得します。 |
| [get_Predecessors](./get_predecessors/) | この Task オブジェクトのすべての前任タスクを含む TaskCollection オブジェクトを取得します。 |
| [get_PreleveledFinish](./get_preleveledfinish/) | PreleveledFinish の値を取得します。 |
| [get_PreleveledStart](./get_preleveledstart/) | PreleveledStart の値を取得します。 |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera ファイルから読み取ったタスクの Primavera 固有プロパティを含むオブジェクトを取得します。 |
| [get_Priority](./get_priority/) | Priority の値を取得します。 |
| [get_RecurringInfo](./get_recurringinfo/) | 繰り返しタスクであるタスクの RecurringTaskInfo クラスのインスタンスを取得します；タスクが繰り返しタスクでない場合は null を返します； |
| [get_RegularWork](./get_regularwork/) | RegularWork の値を取得します。 |
| [get_RemainingCost](./get_remainingcost/) | RemainingCost の値を取得します。 |
| [get_RemainingDuration](./get_remainingduration/) | RemainingDuration の値を取得します。 |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | RemainingOvertimeCost の値を取得します。 |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | RemainingOvertimeWork の値を取得します。 |
| [get_RemainingWork](./get_remainingwork/) | RemainingWork の値を取得します。 |
| [get_Resume](./get_resume/) | Resume の値を取得します。 |
| [get_SplitParts](./get_splitparts/) | タスクの部分を表す SplitPart コレクションを取得します。 |
| [get_Start](./get_start/) | Start の値を取得します。 |
| [get_StartSlack](./get_startslack/) | StartSlack の値を取得します。 |
| [get_StartText](./get_starttext/) | StartText の値を取得します。 |
| [get_StartVariance](./get_startvariance/) | StartVariance の値を取得します。 |
| [get_Status](./get_status/) | タスクのステータスを取得します。 |
| [get_StatusManager](./get_statusmanager/) | StatusManager の値を取得します。 |
| [get_Stop](./get_stop/) | Stop の値を取得します。 |
| [get_SubprojectName](./get_subprojectname/) | SubprojectName の値を取得します。 |
| [get_Successors](./get_successors/) | この Task オブジェクトのすべての後続タスクを含む TaskCollection オブジェクトを取得します。 |
| [get_SV](./get_sv/) | プロジェクトのステータス日までの実績価値スケジュール差異。スケジュール差異（SV）は BCWP と BCWS の差です。 |
| [get_TimephasedData](./get_timephaseddata/) | このタスクの TimephasedDataCollection オブジェクトを取得します。タスクに関連付けられた時間フェーズデータブロックです。 |
| [get_TotalSlack](./get_totalslack/) | TotalSlack の値を取得します。 |
| [get_Type](./get_type/) | Type の値を取得します。 |
| [get_Uid](./get_uid/) | Uid の値を取得します。 |
| [get_Warning](./get_warning/) | Warning が設定されているかどうかを示す値を取得します。 |
| [get_WBS](./get_wbs/) | WBS の値を取得します。 |
| [get_WBSLevel](./get_wbslevel/) | WBSLevel の値を取得します。 |
| [get_Work](./get_work/) | Work の値を取得します。 |
| [get_WorkVariance](./get_workvariance/) | WorkVariance の値を取得します。 |
| [GetHashCode](./gethashcode/) | この Task のハッシュコード値を返します。 |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | 指定された開始日と終了日の範囲内の TimephasedData 値を含む TimephasedDataCollection オブジェクトを返します。 |
| [MoveToSibling (2 overloads)](./movetosibling/) | 現在のタスクを同じアウトラインレベルで指定されたタスクの前に移動します。ParentProject.CalculationMode が None の場合、このメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクトタスク（開始/終了日、早期/遅延日を設定）を再スケジュールし、スラック、作業、コストフィールド、アウトラインレベルなどの依存フィールドを計算します）。ParentProject.CalculationMode が Manual の場合、メソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。ParentProject.CalculationMode が Automatic の場合、メソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします（開始/終了日、早期/遅延日を設定し、スラック、作業、コストフィールドを計算し、ID とアウトラインレベルを再計算します）。 |
| [OutlineIndent](./outlineindent/) | アウトラインでタスクをインデントします。 |
| [OutlineOutdent](./outlineoutdent/) | アウトラインでタスクを昇格させます。 |
| [SelectAllChildTasks](./selectallchildtasks/) | このタスクのすべての子タスクを再帰的に収集します。 |
| [Set](./set/) | このコンテナ内で、指定されたプロパティを指定された値にマップします。 |
| [set_ActivityId](./set_activityid/) | アクティビティ ID フィールドを表します - Primavera で使用されるタスクの固有識別子です。（Primavera プロジェクトにのみ適用されます） |
| [set_ActualCost](./set_actualcost/) | ActualCost の値を設定します。 |
| [set_ActualDuration](./set_actualduration/) | ActualDuration の値を設定します。 |
| [set_ActualFinish](./set_actualfinish/) | ActualFinish の値を設定します。 |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | ActualOvertimeCost の値を設定します。 |
| [set_ActualOvertimeWork](./set_actualovertimework/) | ActualOvertimeWork の値を設定します。 |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | ActualOvertimeWorkProtected の値を設定します。 |
| [set_ActualStart](./set_actualstart/) | ActualStart の値を設定します。 |
| [set_ActualWork](./set_actualwork/) | ActualWork の値を設定します。 |
| [set_ActualWorkProtected](./set_actualworkprotected/) | ActualWorkProtected の値を設定します。 |
| [set_ACWP](./set_acwp/) | ACWP の値を設定します。 |
| [set_Baselines](./set_baselines/) | タスクのベースライン値のコレクションを設定します。 |
| [set_BCWP](./set_bcwp/) | BCWP の値を設定します。 |
| [set_BCWS](./set_bcws/) | BCWS の値を設定します。 |
| [set_BudgetCost](./set_budgetcost/) | BudgetCost の値を設定します。 |
| [set_BudgetWork](./set_budgetwork/) | BudgetWork の値を設定します。 |
| [set_Calendar](./set_calendar/) | Calendar の値を設定します。 |
| [set_CommitmentFinish](./set_commitmentfinish/) | CommitmentFinish の値を設定します。 |
| [set_CommitmentStart](./set_commitmentstart/) | CommitmentStart の値を設定します。 |
| [set_CommitmentType](./set_commitmenttype/) | CommitmentType の値を設定します。 |
| [set_ConstraintDate](./set_constraintdate/) | ConstraintDate の値を設定します。 |
| [set_ConstraintType](./set_constrainttype/) | ConstraintType の値を設定します。 |
| [set_Contact](./set_contact/) | Contact の値を設定します。 |
| [set_Cost](./set_cost/) | Cost の値を設定します。 |
| [set_CostVariance](./set_costvariance/) | CostVariance の値を設定します。 |
| [set_Created](./set_created/) | Created の値を設定します。 |
| [set_CV](./set_cv/) | CV の値を設定します。 |
| [set_Deadline](./set_deadline/) | Deadline の値を設定します。 |
| [set_DisplayAsSummary](./set_displayassummary/) | DisplayAsSummary が設定されているかどうかを示す値を設定します。 |
| [set_DisplayOnTimeline](./set_displayontimeline/) | DisplayOnTimeline が設定されているかどうかを示す値を設定します。 |
| [set_Duration](./set_duration/) | Duration の値を設定します。 |
| [set_DurationFormat](./set_durationformat/) | DurationFormat の値を設定します。 |
| [set_DurationText](./set_durationtext/) | DurationText の値を設定します。 |
| [set_DurationVariance](./set_durationvariance/) | DurationVariance の値を設定します。 |
| [set_EarlyFinish](./set_earlyfinish/) | EarlyFinish の値を設定します。 |
| [set_EarlyStart](./set_earlystart/) | EarlyStart の値を設定します。 |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod の値を設定します。 |
| [set_ExternalId](./set_externalid/) | ExternalId の値を設定します。 |
| [set_ExternalTaskProject](./set_externaltaskproject/) | ExternalTaskProject の値を設定します。 |
| [set_ExternalUid](./set_externaluid/) | 外部タスクが外部の場合に、外部タスクの一意の識別子を取得または設定します。 |
| [set_Finish](./set_finish/) | Finish の値を設定します。 |
| [set_FinishSlack](./set_finishslack/) | FinishSlack の値を設定します。 |
| [set_FinishText](./set_finishtext/) | FinishText の値を設定します。 |
| [set_FinishVariance](./set_finishvariance/) | FinishVariance の値を設定します。 |
| [set_FixedCost](./set_fixedcost/) | FixedCost の値を設定します。 |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | FixedCostAccrual の値を設定します。 |
| [set_FreeSlack](./set_freeslack/) | FreeSlack の値を設定します。 |
| [set_Guid](./set_guid/) | Guid の値を設定します。 |
| [set_HideBar](./set_hidebar/) | HideBar が設定されているかどうかを示す値を設定します。 |
| [set_Hyperlink](./set_hyperlink/) | タスクに関連付けられたハイパーリンクのタイトルまたは説明テキストを設定します。 |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | タスクに関連付けられたハイパーリンクのアドレスを設定します。 |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | タスクに関連付けられたハイパーリンク内のドキュメントの特定の場所を設定します。 |
| [set_Id](./set_id/) | Id の値を設定します。 |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | IgnoreResourceCalendar が設定されているかどうかを示す値を設定します。 |
| [set_IgnoreWarnings](./set_ignorewarnings/) | IgnoreWarnings が設定されているかどうかを示す値を設定します。 |
| [set_IsActive](./set_isactive/) | IsActive が設定されているかどうかを示す値を設定します。 |
| [set_IsCritical](./set_iscritical/) | IsCritical が設定されているかどうかを示す値を設定します。 |
| [set_IsEffortDriven](./set_iseffortdriven/) | IsEffortDriven が設定されているかどうかを示す値を設定します。 |
| [set_IsEstimated](./set_isestimated/) | IsEstimated が設定されているかどうかを示す値を設定します。 |
| [set_IsExpanded](./set_isexpanded/) | IsExpanded が設定されているかどうかを示す値を設定します。 |
| [set_IsExternalTask](./set_isexternaltask/) | IsExternalTask が設定されているかどうかを示す値を設定します。 |
| [set_IsManual](./set_ismanual/) | IsManual が設定されているかどうかを示す値を設定します。 |
| [set_IsMarked](./set_ismarked/) | IsMarked が設定されているかどうかを示す値を設定します。 |
| [set_IsMilestone](./set_ismilestone/) | IsMilestone が設定されているかどうかを示す値を設定します。 |
| [set_IsNull](./set_isnull/) | IsNull が設定されているかどうかを示す値を設定します。 |
| [set_IsOverallocated](./set_isoverallocated/) | IsOverallocated が設定されているかどうかを示す値を設定します。 |
| [set_IsPublished](./set_ispublished/) | IsPublished が設定されているかどうかを示す値を設定します。 |
| [set_IsRecurring](./set_isrecurring/) | IsRecurring が設定されているかどうかを示す値を設定します。 |
| [set_IsResumeValid](./set_isresumevalid/) | IsResumeValid が設定されているかどうかを示す値を設定します。 |
| [set_IsRollup](./set_isrollup/) | IsRollup が設定されているかどうかを示す値を設定します。 |
| [set_IsSubproject](./set_issubproject/) | IsSubproject が設定されているかどうかを示す値を設定します。 |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | IsSubprojectReadOnly が設定されているかどうかを示す値を設定します。 |
| [set_IsSummary](./set_issummary/) | IsSummary が設定されているかどうかを示す値を設定します。 |
| [set_LateFinish](./set_latefinish/) | LateFinish の値を設定します。 |
| [set_LateStart](./set_latestart/) | LateStart の値を設定します。 |
| [set_LevelAssignments](./set_levelassignments/) | LevelAssignments が設定されているかどうかを示す値を設定します。 |
| [set_LevelingCanSplit](./set_levelingcansplit/) | LevelingCanSplit が設定されているかどうかを示す値を設定します。 |
| [set_LevelingDelay](./set_levelingdelay/) | LevelingDelay の値を設定します。 |
| [set_ManualDuration](./set_manualduration/) | ManualDuration の値を設定します。 |
| [set_ManualFinish](./set_manualfinish/) | ManualFinish の値を設定します。 |
| [set_ManualStart](./set_manualstart/) | ManualStart の値を設定します。 |
| [set_Name](./set_name/) | Name の値を設定します。 |
| [set_NotesRTF](./set_notesrtf/) | NotesRTF の値を設定します。 |
| [set_NotesText](./set_notestext/) | NotesText の値を設定します。 |
| [set_OutlineCodes](./set_outlinecodes/) | OutlineCodeCollection オブジェクトを設定します。 |
| [set_OutlineLevel](./set_outlinelevel/) | OutlineLevel の値を設定します。 |
| [set_OutlineNumber](./set_outlinenumber/) | OutlineNumber の値を設定します。 |
| [set_OvertimeCost](./set_overtimecost/) | OvertimeCost の値を設定します。 |
| [set_OvertimeWork](./set_overtimework/) | OvertimeWork の値を設定します。 |
| [set_PercentComplete](./set_percentcomplete/) | PercentComplete の値を設定します。 |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | PercentWorkComplete の値を設定します。 |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | PhysicalPercentComplete の値を設定します。 |
| [set_PreleveledFinish](./set_preleveledfinish/) | PreleveledFinish の値を設定します。 |
| [set_PreleveledStart](./set_preleveledstart/) | PreleveledStart の値を設定します。 |
| [set_Priority](./set_priority/) | Priority の値を設定します。 |
| [set_RegularWork](./set_regularwork/) | RegularWork の値を設定します。 |
| [set_RemainingCost](./set_remainingcost/) | RemainingCost の値を設定します。 |
| [set_RemainingDuration](./set_remainingduration/) | RemainingDuration の値を設定します。 |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | RemainingOvertimeCost の値を設定します。 |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | RemainingOvertimeWork の値を設定します。 |
| [set_RemainingWork](./set_remainingwork/) | RemainingWork の値を設定します。 |
| [set_Resume](./set_resume/) | Resume の値を設定します。 |
| [set_Start](./set_start/) | Start の値を設定します。 |
| [set_StartSlack](./set_startslack/) | StartSlack の値を設定します。 |
| [set_StartText](./set_starttext/) | StartText の値を設定します。 |
| [set_StartVariance](./set_startvariance/) | StartVariance の値を設定します。 |
| [set_StatusManager](./set_statusmanager/) | StatusManager の値を設定します。 |
| [set_Stop](./set_stop/) | Stop の値を設定します。 |
| [set_SubprojectName](./set_subprojectname/) | SubprojectName の値を設定します。 |
| [set_SV](./set_sv/) | プロジェクトのステータス日までの実績価値スケジュール差異。スケジュール差異（SV）は BCWP と BCWS の差です。 |
| [set_TimephasedData](./set_timephaseddata/) | このタスクの TimephasedDataCollection オブジェクトを設定します。タスクに関連付けられた時間別データブロックです。 |
| [set_TotalSlack](./set_totalslack/) | TotalSlack の値を設定します。 |
| [set_Type](./set_type/) | Type の値を設定します。 |
| [set_Uid](./set_uid/) | Uid の値を設定します。 |
| [set_Warning](./set_warning/) | Warning が設定されているかどうかを示す値を設定します。 |
| [set_WBS](./set_wbs/) | WBS の値を設定します。 |
| [set_WBSLevel](./set_wbslevel/) | WBSLevel の値を設定します。 |
| [set_Work](./set_work/) | Work の値を設定します。 |
| [set_WorkVariance](./set_workvariance/) | WorkVariance の値を設定します。 |
| [ToString](./tostring/) | タスクの短い文字列表現を返します。表現の正確な詳細は未定義で、変更される可能性があります。 |

