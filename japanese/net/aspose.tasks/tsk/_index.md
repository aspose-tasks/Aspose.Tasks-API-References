---
title: Tsk
second_title: Aspose.Tasks for .NET API リファレンス
description: のプロパティを表しますTask./task/object.
type: docs
weight: 2310
url: /ja/net/aspose.tasks/tsk/
---
## Tsk class

のプロパティを表します[`Task`](../task/)object.

```csharp
public static class Tsk
```

## 田畑

| 名前 | 説明 |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | アクティビティ ID フィールド (Primavera が使用するタスクの一意の識別子) を表します。 (Primavera プロジェクトにのみ適用可能). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | タスクでリソースによって既に実行された作業に対して発生したコストと、そのタスクに関連して記録されたその他のコスト。 |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | スケジュールされた期間と現在の残りの作業時間または完了率に基づく、タスクの実際の作業時間の範囲. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | タスクが完了した日付。 |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | 割り当てられたリソースによってタスクで既に実行された時間外作業のために発生したコスト. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | タスクに割り当てられたリソースによって既に実行された実際の残業時間. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | 実際の時間外労働が保護される期間. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | タスクが実際に開始された日時。 |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | タスクに割り当てられたリソースによって既に完了した作業の量. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | 実際の作業が保護される期間. 読み取りは XML 形式のみサポートされています。 |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | プロジェクトの状況報告日または今日の日付までに、タスクで既に完了した作業に対して発生したコスト。 |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | タスクの完了率の累積値に時間フェーズの基準コストを掛けたもの。 |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | 状況報告日または今日の日付までの累積時系列ベースライン コスト。 |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | 予算コスト リソースの予算コスト。予算リソースは、プロジェクトのサマリー タスクにのみ割り当てられます。 |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | 予算作業と資材リソースの予算作業。予算リソースは、プロジェクトのサマリー タスクにのみ割り当てられます。 |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | タスク カレンダー。 |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | 配達の終了日.  読み取りは XML 形式のみサポートされています。 |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | 配送開始日. 読み取りは XML 形式のみサポートされています。 |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | タスクに関連付けられた配信または 関連付けられた配信への依存関係があるかどうかを決定します。 読み取りは XML 形式のみサポートされています。 |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | 制約タイプに関連付けられた特定の日付. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | タスクのスケジューリングに適用できる制約のタイプを選択できます。 |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | タスクを担当する個人の名前。 |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | 残りの作業に対して計画されたコストに加えて、タスクに割り当てられたリソースによって実行された作業に対して既に発生したコストに基づく、タスクの予定または予測されたコストの合計。 |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | タスク、リソース、または割り当ての基準コストと総コストの差。 |
| static readonly [Created](../../aspose.tasks/tsk/created/) | タスクが作成された日付。 |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | タスクのベースライン コストと総コストの差。 コスト差異 = コスト - ベースライン コスト |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | タスクがいつ完了するかを示す目標日。 |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | タスクをサマリー タスクとして表示するかどうかを決定します。 読み取りは XML 形式のみサポートされています。 |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | タスクをタイムライン ビューに表示するかどうかを指定します。 |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | 入力された、または開始日、終了日、カレンダー、およびその他のスケジュール要素に基づいて Microsoft Project によって計算された、タスクのアクティブな作業時間の合計期間。 |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat/) | タスク期間の形式. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | タスクの期間テキストを返します。 |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | タスクのベースライン期間とタスクの合計期間 (現在の見積もり) との差. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | 先行タスクと後続タスクの早期終了日、その他の制約、および平準化の遅延に基づいて、タスクが終了する可能性がある最も早い日付. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | 先行タスクと後続タスクの早期開始日およびその他の制約に基づいて、タスクを開始できる可能性のある最も早い日付. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | 実行された作業の予算コスト (BCWP) を計算するために、[% 完了] または [物理的 % 完了] フィールドを使用するかどうかを決定します。 |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | タスクが外部タスクの場合、タスクの外部 ID が含まれます。 |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | 外部タスクのソースの場所とタスク識別子. |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | タスクが外部の場合、外部タスクの一意の識別子が含まれます。 |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | タスクの終了予定日。 |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | アーリー フィニッシュとレイト フィニッシュの日付の間の期間。 |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | タスクの終了テキストを返します。 |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | タスクまたは割り当ての基準終了日と現在の終了日との差を表す時間。 |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | 非リソース タスク費用を表示します。 |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | タスクのコストに固定費をいつ、どのように請求するか、または計上するかの選択肢を決定します。 |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | 後続のタスクを遅らせることなくタスクを遅らせることができる時間。 |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | タスク用に生成された一意の識別コード. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | タスクに割り当てられたリソースが割り当てられているかどうかを示します。このリソースには、割り当てられたタスクで、通常の作業能力内で完了できるよりも多くの作業があります。 |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | Microsoft Project に表示されたときに、タスクのガント バーを非表示にするかどうかを決定します。 |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | タスクに関連付けられたハイパーリンクのタイトルまたは説明テキスト. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | タスクに関連付けられたハイパーリンクのアドレス。 |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | タスクに関連付けられたハイパーリンク内のドキュメント内の特定の場所. |
| static readonly [Id](../../aspose.tasks/tsk/id/) | タスクのリスト内のタスクの位置識別子. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | タスクのスケジューリングで、タスクに割り当てられたリソースのカレンダーを考慮するかどうかを決定します。 |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | Microsoft Project でスケジュール競合の警告インジケーターを非表示にするかどうかを示します。 |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | タスクがアクティブかどうかを決定します。非アクティブなタスクは、他のタスクやプロジェクト スケジュール全体に影響しなくなります。 |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | タスクがクリティカル パス上にあるかどうかを判断します。 |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | タスクのスケジューリングが工数主導型スケジューリングかどうかを決定します。 |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | タスクを見積もるかどうかを決定します。 |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | ガントチャート ビューでサマリー タスクを展開するかどうかを決定します。 |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | タスクが外部かどうかを決定します。 |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | タスクが手動でスケジュールされているかどうかを決定します. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | タスクがさらなるアクションまたは何らかの種類の識別のためにマークされているかどうかを示します. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | タスクがマイルストーンかどうかを決定します。 |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | タスクが null タスクかどうかを判断します。 |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | タスクに割り当てられたリソースのいずれかが、通常の作業能力で実行できるよりも多くの作業に割り当てられているかどうかを示します. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | 現在のタスクを残りのプロジェクトと共に Project Server に発行するかどうかを決定します。 |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | タスクが一連の繰り返しタスクの一部であるかどうかを決定します。 |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | タスクを再開できるかどうかを決定します。 |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | サブタスク ガント バーに関する情報をサマリー タスク バーにロールアップするかどうかを決定します。 |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | タスクが挿入されたプロジェクトかどうかを判断します。 |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | サブプロジェクトが読み取り専用かどうかを決定します。 |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | タスクがサマリー タスクかどうかを決定します。 |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | プロジェクトの終了を遅らせることなくタスクを終了できる最も遅い日付。 |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | プロジェクトの終了を遅らせることなくタスクを開始できる最も遅い日付. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | 割り当て超過を解決するために、平準化機能が個々の割り当てを遅延および分割できるかどうかを決定します。 |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | リソース平準化機能により、このタスクの残りの作業を分割できるかどうかを決定します。 |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | リソースの平準化のためにタスクが早期開始日から遅れる時間。 |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat/) | 遅延時間の表現形式. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | 手動でスケジュールされたタスクの期間を定義します。 |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | 手動でスケジュールされたタスクの終了を定義します. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | 手動でスケジュールされたタスクの開始を定義します。 |
| static readonly [Name](../../aspose.tasks/tsk/name/) | タスクの名前。 |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | RTF 形式のテキスト ノート。 |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | RTF データから抽出されたメモのプレーン テキスト。 |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | タスクのアウトライン レベル。 |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | 階層的なアウトライン構造におけるタスクの位置を表す番号. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | タスク、割り当てられたすべてのタスクのリソース、またはリソース割り当ての合計残業コスト。 |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | タスクに割り当てられたすべてのリソースによって実行される予定の残業時間。 |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | 完了したタスクの期間のパーセンテージとして表される、タスクの現在のステータス。 |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | 完了した作業の割合として表されるタスクの現在のステータス。 |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | 実行された作業の予算コスト (BCWP) を計算するための代替として使用できる完了率の値。 |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | リソースの平準化が行われる前のタスクの終了日。 |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | リソースの平準化が行われる前のタスクの開始日。 |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | タスクに与えられた重要度のレベル。これは、リソースの平準化中にタスクまたは割り当てがどれだけ容易に延期または分割されるかを示します。 |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | リソースによって実行される予定の非残業時間の合計。 |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | 残りの予定された作業を完了するために発生する残りの予定された費用. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | タスクの未完了部分を完了するのに必要な時間. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | タスクの残りの予定残業代。 |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | 残業予定残業時間. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | タスクまたは一連のタスクを完了するためにまだ必要な時間. |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | 進行状況を入力した後、タスクの残りの部分が再開される予定の日付。 |
| static readonly [Start](../../aspose.tasks/tsk/start/) | タスクの開始予定日。 |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | 最早開始日と最遅開始日の間の期間. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | タスクの開始テキストを返します。 |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | タスクまたは割り当てのベースライン開始日と現在スケジュールされている開始日との差を表す時間. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | リソースから現在のタスクのステータス更新を受信するエンタープライズ リソースの名前。 |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | タスクの実際の部分の終了を表す日付。 |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | サブプロジェクトのソースの場所。 |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | プロジェクト状況報告日までのアーンド バリュー スケジュール差異。 スケジュール差異 (SV) は、BCWP と BCWS の差異です。 |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | プロジェクトの終了日を遅らせることなく、タスクの終了日を遅らせることができる時間。 |
| static readonly [Type](../../aspose.tasks/tsk/type/) | タスクのタイプ。 |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | タスクの一意の ID。 |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | タスクにスケジュールの不一致があることを示すフラグを表します。 |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | 作業分解構造 (WBS) コード. |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | タスクの右端の WBS レベル。 |
| static readonly [Work](../../aspose.tasks/tsk/work/) | 割り当てられたすべてのリソースのタスクにスケジュールされた合計時間. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | タスクの基準作業時間と現在スケジュールされている作業時間の差。 |

### 関連項目

* 名前空間 [Aspose.Tasks](../../aspose.tasks/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
