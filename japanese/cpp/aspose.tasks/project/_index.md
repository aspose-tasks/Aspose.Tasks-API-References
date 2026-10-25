---
title: "Aspose::Tasks::Project クラス"
linktitle: "プロジェクト"
articleTitle: "プロジェクト"
second_title: "Aspose.Tasks for C++"
description: "プロジェクトを表します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/project/
---

## Project class

プロジェクトを表します。

Project は Aspose.Tasks ライブラリの中心クラスです。

Project を使用して、サポートされているプロジェクト管理フォーマットのいずれか（MPP、MPT、MPX、XML）を読み取ることができます。

サポートされているいずれかの形式で既存のドキュメントを読み込むには、ファイル名またはストリームを Project のコンストラクタのいずれかに渡します。空のプロジェクトを作成するには、パラメータなしコンストラクタを呼び出します。

Save メソッドのオーバーロードのいずれかを使用して、プロジェクトを Aspose::Tasks::Saving::SaveFileFormat の形式で保存します：Primavera: P6 XML、PM XER；Microsoft Excel: XLSX、XML；固定レイアウト: PDF；画像: JPEG、PNG、BMP、TIFF、SVG；テキスト: TXT；その他: HTML。

Project は、Aspose::Tasks::Project::Views、Aspose::Tasks::Project::BuiltInProps、Aspose::Tasks::Project::CustomProps、Aspose::Tasks::Project::ExtendedAttributes などのプロジェクト全体の情報を格納します。これらのオブジェクトのほとんどは、Project クラスの対応するプロパティを介してアクセスできます。

Project は、Aspose::Tasks::Task、Aspose::Tasks::Resource、Aspose::Tasks::ResourceAssignment、Aspose::Tasks::ExtendedAttribute、Aspose::Tasks::Calendar などの他のプロジェクトエンティティを操作するためのエントリポイントを含むルートエンティティです。

Project エンティティは、型付きコレクションを介してアクセスできます。例として Aspose::Tasks::Task::Children、Aspose::Tasks::Project::Resources、Aspose::Tasks::Project::ResourceAssignments などがあります。

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Project (13 overloads)](./project/) | Project クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。 |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | ルートタスクを含むプロジェクトのすべてのタスクを再帰的に列挙します。 |
| [Get](./get/) | このコンテナ内でプロパティがマッピングされている値を返します。 |
| [get_ActualsInSync](./get_actualsinsync/) | ActualsInSync が設定されているかどうかを示す値を取得します。 |
| [get_AdminProject](./get_adminproject/) | AdminProject が設定されているかどうかを示す値を取得します。 |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | AreEditableActualCosts が設定されているかどうかを示す値を取得します。 |
| [get_Author](./get_author/) | Author の値を取得します。 |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を取得します。 |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算すべきかどうかを取得します。 |
| [get_Autolink](./get_autolink/) | Autolink が設定されているかどうかを示す値を取得します。 |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | BaselineForEarnedValue の値を取得します。 |
| [get_BuiltInProps](./get_builtinprops/) | プロジェクトの組み込みプロパティコレクションを取得します。 |
| [get_CalculationMode](./get_calculationmode/) | プロジェクトの計算モードを取得します。CalculationMode 列挙体の値のいずれかです。 |
| [get_Calendar](./get_calendar/) | Calendar の値を取得します。 |
| [get_Calendars](./get_calendars/) | この Project インスタンスの CalendarCollection オブジェクトを取得します。 |
| [get_Category](./get_category/) | Category の値を取得します。 |
| [get_Comments](./get_comments/) | Comments の値を取得します。 |
| [get_Company](./get_company/) | Company の値を取得します。 |
| [get_CreationDate](./get_creationdate/) | CreationDate の値を取得します。 |
| [get_CriticalPath](./get_criticalpath/) | このプロジェクトのクリティカルパスを構成するクリティカルタスクのリストを含むコレクションを取得します。 |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | CriticalSlackLimit の値を取得します。 |
| [get_CurrencyCode](./get_currencycode/) | CurrencyCode の値を取得します。 |
| [get_CurrencyDigits](./get_currencydigits/) | CurrencyDigits の値を取得します。 |
| [get_CurrencySymbol](./get_currencysymbol/) | CurrencySymbol の値を取得します。 |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | CurrencySymbolPosition の値を取得します。 |
| [get_CurrentDate](./get_currentdate/) | CurrentDate の値を取得します。 |
| [get_CustomDateFormat](./get_customdateformat/) | CustomDateFormat の値を取得します。 |
| [get_CustomProps](./get_customprops/) | プロジェクトのカスタム プロパティ コレクションを取得します。 |
| [get_DateFormat](./get_dateformat/) | DateFormat の値を取得します。 |
| [get_DaysPerMonth](./get_dayspermonth/) | DaysPerMonth の値を取得します。 |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | DefaultFinishTime の値を取得します。 |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | DefaultFixedCostAccrual の値を取得します。 |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | DefaultOvertimeRate の値を取得します。 |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | DefaultStandardRate の値を取得します。 |
| [get_DefaultStartTime](./get_defaultstarttime/) | DefaultStartTime の値を取得します。 |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | DefaultTaskEVMethod の値を取得します。 |
| [get_DefaultTaskType](./get_defaulttasktype/) | DefaultTaskType の値を取得します。 |
| [get_DefaultView](./get_defaultview/) | プロジェクトのデフォルトビューを取得します。 |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | WeekDayCollection クラスのインスタンスを取得します。このクラスはプロジェクトのデフォルトの週の稼働日と稼働時間のコレクションを表します。 |
| [get_DisplayOptions](./get_displayoptions/) | ProjectDisplayOptions クラスのインスタンスを取得します。 |
| [get_DurationFormat](./get_durationformat/) | DurationFormat の値を取得します。 |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod の値を取得します。 |
| [get_ExtendedAttributes](./get_extendedattributes/) | ExtendedAttributeDefinitionCollection オブジェクトを取得します。これは、プロジェクトに関連付けられた拡張属性（カスタム フィールド）定義のコレクションです。 |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | ExtendedCreationDate の値を取得します。 |
| [get_FinishDate](./get_finishdate/) | FinishDate の値を取得します。 |
| [get_FiscalYearStart](./get_fiscalyearstart/) | FiscalYearStart が設定されているかどうかを示す値を取得します。 |
| [get_FyStartDate](./get_fystartdate/) | FyStartDate の値を取得します。 |
| [get_Guid](./get_guid/) | Guid の値を取得します。 |
| [get_HonorConstraints](./get_honorconstraints/) | HonorConstraints が設定されているかどうかを示す値を取得します。 |
| [get_HyperlinkBase](./get_hyperlinkbase/) | HyperlinkBase の値を取得します。 |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | InsertedProjectsLikeSummary が設定されているかどうかを示す値を取得します。 |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を取得します。 |
| [get_Keywords](./get_keywords/) | Keywords の値を取得します。 |
| [get_LastAuthor](./get_lastauthor/) | LastAuthor の値を取得します。 |
| [get_LastPrinted](./get_lastprinted/) | LastPrinted の値を取得します。 |
| [get_LastSaved](./get_lastsaved/) | LastSaved の値を取得します。 |
| [get_Manager](./get_manager/) | Manager の値を取得します。 |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | MicrosoftProjectServerURL が設定されているかどうかを示す値を取得します。 |
| [get_MinutesPerDay](./get_minutesperday/) | MinutesPerDay の値を取得します。 |
| [get_MinutesPerWeek](./get_minutesperweek/) | MinutesPerWeek の値を取得します。 |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | MoveCompletedEndsBack が設定されているかどうかを示す値を取得します。 |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | MoveCompletedEndsForward が設定されているかどうかを示す値を取得します。 |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | MoveRemainingStartsBack が設定されているかどうかを示す値を取得します。 |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | MoveRemainingStartsForward が設定されているかどうかを示す値を取得します。 |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | MultipleCriticalPaths が設定されているかどうかを示す値を取得します。 |
| [get_Name](./get_name/) | Name の値を取得します。 |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | NewTasksAreManual が設定されているかどうかを示す値を取得します。 |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | NewTasksEffortDriven が設定されているかどうかを示す値を取得します。 |
| [get_NewTasksEstimated](./get_newtasksestimated/) | NewTasksEstimated が設定されているかどうかを示す値を取得します。 |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | NewTaskStartDate の値を取得します。 |
| [get_OleObjects](./get_oleobjects/) | このプロジェクト ファイルにリンクまたは埋め込まれている OleObject クラスのインスタンスを含むコレクションを取得します。 |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeDefinitionCollection オブジェクトを取得します。プロジェクトに関連付けられたアウトライン コード定義のコレクションです。 |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera ファイルから読み取ったプロジェクトの Primavera 固有プロパティを含むオブジェクトを取得します。 |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | ProjectExternallyEdited が設定されているかどうかを示す値を取得します。 |
| [get_RemoveFileProperties](./get_removefileproperties/) | RemoveFileProperties が設定されているかどうかを示す値を取得します。 |
| [get_ResourceAssignments](./get_resourceassignments/) | ResourceAssignmentCollection オブジェクトを取得します。 |
| [get_ResourceFilters](./get_resourcefilters/) | リソースベースのフィルタ定義をすべて取得します。ResourceFilters は Filter オブジェクトのコレクションです。 |
| [get_ResourceGroups](./get_resourcegroups/) | リソースベースのグループ定義をすべて取得します。ResourceGroups は Group オブジェクトのコレクションです。 |
| [get_Resources](./get_resources/) | ResourceCollection オブジェクトを取得します。 |
| [get_Revision](./get_revision/) | Revision の値を取得します。 |
| [get_RootTask](./get_roottask/) | タスクツリーのルートを取得します。 |
| [get_SaveVersion](./get_saveversion/) | SaveVersion の値を取得します。 |
| [get_ScheduleFromStart](./get_schedulefromstart/) | ScheduleFromStart が設定されているかどうかを示す値を取得します。 |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | ShowProjectSummaryTask が設定されているかどうかを示す値を取得します。 |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | SplitsInProgressTasks が設定されているかどうかを示す値を取得します。 |
| [get_SpreadActualCost](./get_spreadactualcost/) | SpreadActualCost が設定されているかどうかを示す値を取得します。 |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | SpreadPercentComplete が設定されているかどうかを示す値を取得します。 |
| [get_StartDate](./get_startdate/) | StartDate の値を取得します。 |
| [get_StatusDate](./get_statusdate/) | StatusDate の値を取得します。 |
| [get_Subject](./get_subject/) | Subject の値を取得します。 |
| [get_Tables](./get_tables/) | Table オブジェクトのリストを取得します。 |
| [get_TaskFilters](./get_taskfilters/) | タスクベースのフィルタ定義をすべて取得します。TaskFilters は Filter オブジェクトのコレクションです。 |
| [get_TaskGroups](./get_taskgroups/) | タスクベースのグループ定義をすべて取得します。TaskGroups は Group オブジェクトのコレクションです。 |
| [get_TaskLinks](./get_tasklinks/) | TaskLinkCollection オブジェクトを取得します。 |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | TaskUpdatesResource が設定されているかどうかを示す値を取得します。 |
| [get_Template](./get_template/) | Template の値を取得します。 |
| [get_TimescaleFinish](./get_timescalefinish/) | TimescaleFinish の値を取得します。 |
| [get_TimescaleStart](./get_timescalestart/) | TimescaleStart の値を取得します。 |
| [get_Title](./get_title/) | Title の値を取得します。 |
| [get_Uid](./get_uid/) | Uid の値を取得します。 |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks が設定されているかどうかを示す値を取得します。 |
| [get_VbaProject](./get_vbaproject/) | VbaProject クラスのインスタンスを取得します。 |
| [get_Views](./get_views/) | View オブジェクトのリストを取得します。 |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | プロジェクトの WBS コード定義を取得します。 |
| [get_WeekStartDay](./get_weekstartday/) | WeekStartDay の値を取得します。 |
| [get_WorkFormat](./get_workformat/) | WorkFormat の値を取得します。 |
| [GetBaselineSaveTime](./getbaselinesavetime/) | ベースラインの保存時刻を返します。 |
| [GetDuration (3 overloads)](./getduration/) | プロジェクトの設定 Prj::DurationFormat で定義されたデフォルトの期間形式と、指定された単位数を持つ Duration オブジェクトを取得します。 |
| [GetPageCount (7 overloads)](./getpagecount/) | デフォルトの Timescale（Days）を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [GetPredecessors](./getpredecessors/) | 指定されたタスクの前任タスクリンクのコレクションを返します。 |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | ストリームからプロジェクト ファイル情報を取得します。 |
| [GetWork](./getwork/) | 指定された double 値とデフォルトの作業形式を持つ Duration オブジェクトを取得します。 |
| [Recalculate (2 overloads)](./recalculate/) | すべてのプロジェクト タスクの ID、アウトライン レベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、余裕時間、作業およびコスト フィールドを計算します。 |
| [RecalculateResourceFields](./recalculateresourcefields/) | リソースの Id、開始日、終了日を再計算します。 |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | リソースの開始日と終了日を再計算します。 |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | プロジェクトのリソース割り当てリストから無効なリソース割り当てを除外します。 |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | すべてのタスクの WBS コードを再番号付けします。 |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | 未完了のプロジェクト作業を指定された日付以降に開始するように再スケジュールします。 |
| [Save (5 overloads)](./save/) | 指定された保存オプションを使用してプロジェクトをストリームに保存します。 |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | プロジェクトをテンプレートとして指定されたストリームに保存します。 |
| [SaveReport (4 overloads)](./savereport/) | プロジェクト概要レポートをストリームに保存します。 |
| [SelectAllChildTasks](./selectallchildtasks/) | ルート タスクのすべての子タスクを再帰的に収集します。 |
| [Set (2 overloads)](./set/) | このコンテナ内で、指定されたプロパティを指定された値にマップします。 |
| [set_ActualsInSync](./set_actualsinsync/) | ActualsInSync が設定されているかどうかを示す値を設定します。 |
| [set_AdminProject](./set_adminproject/) | AdminProject が設定されているかどうかを示す値を設定します。 |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | AreEditableActualCosts が設定されているかどうかを示す値を設定します。 |
| [set_Author](./set_author/) | Author の値を設定します。 |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を設定します。 |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動計算するかどうかを設定します。 |
| [set_Autolink](./set_autolink/) | Autolink が設定されているかどうかを示す値を設定します。 |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | BaselineForEarnedValue の値を設定します。 |
| [set_CalculationMode](./set_calculationmode/) | プロジェクトの計算モードを設定します。CalculationMode 列挙体の値のいずれかを指定できます。 |
| [set_Calendar](./set_calendar/) | Calendar の値を設定します。 |
| [set_Category](./set_category/) | Category の値を設定します。 |
| [set_Comments](./set_comments/) | Comments の値を設定します。 |
| [set_Company](./set_company/) | Company の値を設定します。 |
| [set_CreationDate](./set_creationdate/) | CreationDate の値を設定します。 |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | CriticalSlackLimit の値を設定します。 |
| [set_CurrencyCode](./set_currencycode/) | CurrencyCode の値を設定します。 |
| [set_CurrencyDigits](./set_currencydigits/) | CurrencyDigits の値を設定します。 |
| [set_CurrencySymbol](./set_currencysymbol/) | CurrencySymbol の値を設定します。 |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | CurrencySymbolPosition の値を設定します。 |
| [set_CurrentDate](./set_currentdate/) | CurrentDate の値を設定します。 |
| [set_CustomDateFormat](./set_customdateformat/) | CustomDateFormat の値を設定します。 |
| [set_DateFormat](./set_dateformat/) | DateFormat の値を設定します。 |
| [set_DaysPerMonth](./set_dayspermonth/) | DaysPerMonth の値を設定します。 |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | DefaultFinishTime の値を設定します。 |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | DefaultFixedCostAccrual の値を設定します。 |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | DefaultOvertimeRate の値を設定します。 |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | DefaultStandardRate の値を設定します。 |
| [set_DefaultStartTime](./set_defaultstarttime/) | DefaultStartTime の値を設定します。 |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | DefaultTaskEVMethod の値を設定します。 |
| [set_DefaultTaskType](./set_defaulttasktype/) | DefaultTaskType の値を設定します。 |
| [set_DefaultView](./set_defaultview/) | プロジェクトのデフォルトビューを設定します。 |
| [set_DurationFormat](./set_durationformat/) | DurationFormat の値を設定します。 |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod の値を設定します。 |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | ExtendedCreationDate の値を設定します。 |
| [set_FinishDate](./set_finishdate/) | FinishDate の値を設定します。 |
| [set_FiscalYearStart](./set_fiscalyearstart/) | FiscalYearStart が設定されているかどうかを示す値を設定します。 |
| [set_FyStartDate](./set_fystartdate/) | FyStartDate の値を設定します。 |
| [set_Guid](./set_guid/) | Guid の値を設定します。 |
| [set_HonorConstraints](./set_honorconstraints/) | HonorConstraints が設定されているかどうかを示す値を設定します。 |
| [set_HyperlinkBase](./set_hyperlinkbase/) | HyperlinkBase の値を設定します。 |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | InsertedProjectsLikeSummary が設定されているかどうかを示す値を設定します。 |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を設定します。 |
| [set_Keywords](./set_keywords/) | Keywords の値を設定します。 |
| [set_LastAuthor](./set_lastauthor/) | LastAuthor の値を設定します。 |
| [set_LastPrinted](./set_lastprinted/) | LastPrinted の値を設定します。 |
| [set_LastSaved](./set_lastsaved/) | LastSaved の値を設定します。 |
| [set_Manager](./set_manager/) | Manager の値を設定します。 |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | MicrosoftProjectServerURL が設定されているかどうかを示す値を設定します。 |
| [set_MinutesPerDay](./set_minutesperday/) | MinutesPerDay の値を設定します。 |
| [set_MinutesPerWeek](./set_minutesperweek/) | MinutesPerWeek の値を設定します。 |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | MoveCompletedEndsBack が設定されているかどうかを示す値を設定します。 |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | MoveCompletedEndsForward が設定されているかどうかを示す値を設定します。 |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | MoveRemainingStartsBack が設定されているかどうかを示す値を設定します。 |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | MoveRemainingStartsForward が設定されているかどうかを示す値を設定します。 |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | MultipleCriticalPaths が設定されているかどうかを示す値を設定します。 |
| [set_Name](./set_name/) | Name の値を設定します。 |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | NewTasksAreManual が設定されているかどうかを示す値を設定します。 |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | NewTasksEffortDriven が設定されているかどうかを示す値を設定します。 |
| [set_NewTasksEstimated](./set_newtasksestimated/) | NewTasksEstimated が設定されているかどうかを示す値を設定します。 |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | NewTaskStartDate の値を設定します。 |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | ProjectExternallyEdited が設定されているかどうかを示す値を設定します。 |
| [set_RemoveFileProperties](./set_removefileproperties/) | RemoveFileProperties が設定されているかどうかを示す値を設定します。 |
| [set_Revision](./set_revision/) | Revision の値を設定します。 |
| [set_SaveVersion](./set_saveversion/) | SaveVersion の値を設定します。 |
| [set_ScheduleFromStart](./set_schedulefromstart/) | ScheduleFromStart が設定されているかどうかを示す値を設定します。 |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | ShowProjectSummaryTask が設定されているかどうかを示す値を設定します。 |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | SplitsInProgressTasks が設定されているかどうかを示す値を設定します。 |
| [set_SpreadActualCost](./set_spreadactualcost/) | SpreadActualCost が設定されているかどうかを示す値を設定します。 |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | SpreadPercentComplete が設定されているかどうかを示す値を設定します。 |
| [set_StartDate](./set_startdate/) | StartDate の値を設定します。 |
| [set_StatusDate](./set_statusdate/) | StatusDate の値を設定します。 |
| [set_Subject](./set_subject/) | Subject の値を設定します。 |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | TaskUpdatesResource が設定されているかどうかを示す値を設定します。 |
| [set_Template](./set_template/) | Template の値を設定します。 |
| [set_TimescaleFinish](./set_timescalefinish/) | TimescaleFinish の値を設定します。 |
| [set_TimescaleStart](./set_timescalestart/) | TimescaleStart の値を設定します。 |
| [set_Title](./set_title/) | Title の値を設定します。 |
| [set_Uid](./set_uid/) | Uid の値を設定します。 |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks が設定されているかどうかを示す値を設定します。 |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | プロジェクトの WBS Code Definition を設定します。 |
| [set_WeekStartDay](./set_weekstartday/) | WeekStartDay の値を設定します。 |
| [set_WorkFormat](./set_workformat/) | WorkFormat の値を設定します。 |
| [SetBaseline (2 overloads)](./setbaseline/) | プロジェクト全体の指定されたベースラインにベースライン フィールドを保存します。 |
| [SetBaselineSaveTime](./setbaselinesavetime/) | ベースライン保存時刻を設定します。 |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | プロジェクト全体の指定された日付まで、すべての作業を完了として更新します。 |

