---
title: "Tsk"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのプロパティを表します。"
type: docs
weight: 328
url: /ja/java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

[Task](../../com.aspose.tasks/task) オブジェクトのプロパティを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## フィールド

| フィールド | 説明 |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | アクティビティ ID フィールドを表します。これは Primavera が使用するタスクの一意の識別子です。 |
| [ACTUAL_COST](#ACTUAL-COST) | リソースがタスクで既に実施した作業に対して発生したコストと、タスクに関連するその他の記録されたコストを含みます。 |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | タスクの実際の作業時間の期間で、予定期間と現在の残作業または完了率に基づきます。 |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | タスクが完了した日付です。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 割り当てられたリソースがタスクで既に実施した残業作業に対して発生したコスト。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | タスクに割り当てられたリソースが既に実施した残業作業の実際の量です。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 実際の残業作業が保護される期間です。 |
| [ACTUAL_START](#ACTUAL-START) | タスクが実際に開始した日時です。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | タスクに割り当てられたリソースが既に行った作業量です。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 実際の作業が保護される期間です。 |
| [ACWP](#ACWP) | タスクで既に行われた作業に対して発生したコストで、プロジェクトのステータス日または本日の日付までです。 |
| [BCWP](#BCWP) | タスクの完了率に時間フェーズベースラインコストを掛けた累積値です。 |
| [BCWS](#BCWS) | ステータス日または本日の日付までの累積時間フェーズベースラインコストです。 |
| [BUDGET_COST](#BUDGET-COST) | 予算コストリソースの予算コスト。 |
| [BUDGET_WORK](#BUDGET-WORK) | 予算作業と材料リソースのための予算作業。 |
| [CALENDAR](#CALENDAR) | タスクのカレンダーです。 |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | 配達の完了日です。 |
| [COMMITMENT_START](#COMMITMENT-START) | 配達の開始日です。 |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | タスクに関連する配信があるか、または関連する配信への依存関係があるかを判定します。 |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | 制約タイプに関連付けられた特定の日付です。 |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | タスクのスケジューリングに適用できる制約タイプの選択肢を提供します。 |
| [CONTACT](#CONTACT) | タスクの責任者の名前です。 |
| [COST](#COST) | タスクに割り当てられたリソースが実施した作業で既に発生したコストと、残りの作業に計画されたコストを合計した、タスクの総予定コストまたは予測コストです。 |
| [COST_VARIANCE](#COST-VARIANCE) | タスク、リソース、または割り当てのベースラインコストと総コストとの差です。 |
| [CREATED](#CREATED) | タスクが作成された日付です。 |
| [CV](#CV) | タスクのベースラインコストと総コストとの差です。 |
| [DEADLINE](#DEADLINE) | タスクの完了予定日を示す目標日です。 |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | タスクをサマリータスクとして表示すべきかどうかを判定します。 |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | タスクをタイムラインビューに表示すべきかどうかを指定します。 |
| [DURATION](#DURATION) | 開始日、終了日、カレンダー、その他のスケジューリング要因に基づき、Microsoft Project が入力または計算したタスクのアクティブ作業時間の合計期間です。 |
| [DURATION_TEXT](#DURATION-TEXT) | タスクの期間テキストを返します。 |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | タスクのベースライン期間と総期間（現在の見積もり）の差です。 |
| [EARLY_FINISH](#EARLY-FINISH) | 前任タスクと後続タスクの早期終了日、その他の制約、レベリング遅延を考慮した、タスクが最も早く完了できる日付です。 |
| [EARLY_START](#EARLY-START) | 前任タスクと後続タスクの早期開始日、その他の制約に基づく、タスクが最も早く開始できる日付です。 |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | 実績コスト（BCWP）を計算する際に、% 完了または物理的 % 完了フィールドのどちらを使用すべきかを判定します。 |
| [EXTERNAL_ID](#EXTERNAL-ID) | タスクが外部タスクの場合、そのタスクの外部 ID が含まれます。 |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | 外部タスクのソース位置とタスク識別子です。 |
| [EXTERNAL_UID](#EXTERNAL-UID) | タスクが外部の場合、外部タスクの一意識別子が含まれます。 |
| [FINISH](#FINISH) | タスクの予定終了日です。 |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | 早期終了日と遅延終了日の間の期間（秒）です。 |
| [FINISH_TEXT](#FINISH-TEXT) | タスクの終了テキストを返します。 |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | タスクまたは割り当てのベースライン終了日と現在の終了日の差を表す時間です。 |
| [FIXED_COST](#FIXED-COST) | リソース以外のタスク費用を表示します。 |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | タスクのコストに対して、固定費をいつ、どのように請求または発生させるかの選択肢を決定します。 |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | 後続タスクを遅延させずにタスクを遅延できる時間（秒）です。 |
| [GUID](#GUID) | タスクに生成される一意の識別コードです。 |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | タスクに割り当てられたリソースが、通常の作業容量内で完了できる以上の作業を持っているかどうかを示します。 |
| [HIDE_BAR](#HIDE-BAR) | Microsoft Projectで表示される際に、タスクのガントバーが非表示になるかどうかを決定します。 |
| [HYPERLINK](#HYPERLINK) | タスクに関連付けられたハイパーリンクのタイトルまたは説明テキストです。 |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | タスクに関連付けられたハイパーリンクのアドレスです。 |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | タスクに関連付けられたハイパーリンク内のドキュメントの特定位置。 |
| [ID](#ID) | タスク一覧内でのタスクの位置識別子です。 |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | タスクのスケジューリングが、割り当てられたリソースのカレンダーを考慮するかどうかを決定します。 |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | Microsoft Projectでスケジュール競合警告インジケーターを非表示にするかどうかを示します。 |
| [IS_ACTIVE](#IS-ACTIVE) | タスクがアクティブかどうかを決定します。 |
| [IS_CRITICAL](#IS-CRITICAL) | タスクがクリティカルパス上にあるかどうかを決定します。 |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | タスクのスケジューリングが作業量主導かどうかを決定します。 |
| [IS_ESTIMATED](#IS-ESTIMATED) | タスクが見積もりかどうかを決定します。 |
| [IS_EXPANDED](#IS-EXPANDED) | ガントチャートビューでサマリータスクが展開されているかどうかを決定します。 |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | タスクが外部タスクかどうかを決定します。 |
| [IS_MANUAL](#IS-MANUAL) | タスクが手動でスケジュールされているかどうかを決定します。 |
| [IS_MARKED](#IS-MARKED) | タスクが何らかの追加アクションや識別のためにマークされているかどうかを示します。 |
| [IS_MILESTONE](#IS-MILESTONE) | タスクがマイルストーンかどうかを決定します。 |
| [IS_NULL](#IS-NULL) | タスクがヌルタスクかどうかを決定します。 |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | タスクに割り当てられたリソースのいずれかが、通常の作業容量内で完了できる以上の作業を割り当てられているかどうかを示します。 |
| [IS_PUBLISHED](#IS-PUBLISHED) | 現在のタスクをプロジェクト全体とともに Project Server に公開すべきかどうかを決定します。 |
| [IS_RECURRING](#IS-RECURRING) | タスクが繰り返しタスクのシリーズの一部かどうかを決定します。 |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | タスクを再開できるかどうかを決定します。 |
| [IS_ROLLUP](#IS-ROLLUP) | サブタスクのガントバーに関する情報がサマリータスクバーに集約されるかどうかを決定します。 |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | タスクが挿入されたプロジェクトかどうかを判断します。 |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | サブプロジェクトが読み取り専用かどうかを判断します。 |
| [IS_SUMMARY](#IS-SUMMARY) | タスクがサマリータスクかどうかを判断します。 |
| [LATE_FINISH](#LATE-FINISH) | プロジェクトの完了を遅らせずにタスクが完了できる最も遅い日付です。 |
| [LATE_START](#LATE-START) | プロジェクトの完了を遅らせずにタスクが開始できる最も遅い日付です。 |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | リソースレベリング機能がこのタスクの残り作業を分割させるかどうかを判断します。 |
| [LEVELING_DELAY](#LEVELING-DELAY) | リソースレベリングのためにタスクが早期開始日から遅延する時間です。 |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | レベリング機能が過剰割り当てを解消するために個々の割り当てを遅延および分割できるかどうかを判断します。 |
| [MANUAL_DURATION](#MANUAL-DURATION) | タスクの手動スケジュール期間を定義します。 |
| [MANUAL_FINISH](#MANUAL-FINISH) | タスクの手動スケジュール完了日時を定義します。 |
| [MANUAL_START](#MANUAL-START) | タスクの手動スケジュール開始日時を定義します。 |
| [NAME](#NAME) | タスクの名前です。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 形式のテキストノートです。 |
| [NOTES_TEXT](#NOTES-TEXT) | RTF データから抽出されたノートのプレーンテキストです。 |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | タスクのアウトラインレベルです。 |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | 階層アウトライン構造におけるタスクの位置を表す番号です。 |
| [OVERTIME_COST](#OVERTIME-COST) | タスクの総残業コスト、割り当てられたすべてのタスクに対するリソースの残業コスト、またはリソース割り当ての残業コストです。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | タスクに割り当てられたすべてのリソースが実施する予定の残業量です。 |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | タスクの現在のステータスで、タスク期間の完了した割合として表されます。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | タスクの現在のステータスで、完了した作業の割合として表されます。 |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | 実績コスト（BCWP）を計算する代替として使用できる完了率の値です。 |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | リソースレベリング実施前のタスクの完了日です。 |
| [PRELEVELED_START](#PRELEVELED-START) | リソースレベリング実施前のタスクの開始日です。 |
| [PRIORITY](#PRIORITY) | タスクに付与された重要度レベルで、リソースレベリング中にタスクや割り当てがどれだけ容易に遅延または分割できるかを示します。 |
| [REGULAR_WORK](#REGULAR-WORK) | リソースが実施する予定の総非残業作業量です。 |
| [REMAINING_COST](#REMAINING-COST) | 残りの予定作業を完了する際に発生する残りの予定費用です。 |
| [REMAINING_DURATION](#REMAINING-DURATION) | タスクの未完了部分を完了するために必要な時間です。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | タスクの残りの予定残業費用です。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 残りの予定残業時間の量。 |
| [REMAINING_WORK](#REMAINING-WORK) | タスクまたはタスク群を完了するためにまだ必要な時間です。 |
| [RESUME](#RESUME) | タスクの残り部分が進捗に入った後に再開する予定の日付。 |
| [START](#START) | タスクの予定開始日。 |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | 早期開始日と遅延開始日間の期間（秒）。 |
| [START_TEXT](#START-TEXT) | タスクの開始テキストを返します。 |
| [START_VARIANCE](#START-VARIANCE) | タスクまたは割り当てのベースライン開始日と現在の予定開始日の差を表す時間。 |
| [STATUS_MANAGER](#STATUS-MANAGER) | 現在のタスクに関するステータス更新をリソースから受け取る企業リソースの名前。 |
| [STOP](#STOP) | タスクの実際の部分の終了を示す日付。 |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | サブプロジェクトのソース場所。 |
| [SV](#SV) | プロジェクトステータス日までの実績価値スケジュール差異です。 |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | タスクの完了日がプロジェクトの完了日を遅らせることなく遅延できる時間。 |
| [TYPE](#TYPE) | タスクのタイプ。 |
| [UID](#UID) | タスクの一意のID。 |
| [WARNING](#WARNING) | スケジュールの不一致があることを示すフラグを表します。 |
| [WBS](#WBS) | 作業分解構成 (WBS) コード。 |
| [WBS_LEVEL](#WBS-LEVEL) | タスクの最右側のWBSレベル。 |
| [WORK](#WORK) | 割り当てられたすべてのリソースに対してタスクに予定されている合計時間。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | タスクのベースライン作業と現在予定されている作業との差。 |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Byte> ACTIVITY_ID
```


アクティビティIDフィールドを表します - Primaveraで使用されるタスクの一意の識別子です。（Primaveraプロジェクトにのみ適用）

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


リソースがタスクで既に実施した作業に対して発生したコストと、タスクに関連するその他の記録されたコストを含みます。

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Byte> ACTUAL_DURATION
```


タスクの実際の作業時間の期間で、予定期間と現在の残作業または完了率に基づきます。

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


タスクが完了した日付です。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


割り当てられたリソースがタスクで既に実施した残業作業に対して発生したコスト。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


タスクに割り当てられたリソースが既に実施した残業作業の実際の量です。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


実際の残業作業が保護される期間です。

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


タスクが実際に開始した日時です。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


タスクに割り当てられたリソースが既に行った作業量です。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


実際の作業が保護される期間です。

--------------------

XML フォーマットのみで読み取りがサポートされています。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


タスクで既に行われた作業に対して発生したコストで、プロジェクトのステータス日または本日の日付までです。

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


タスクの完了率に時間フェーズベースラインコストを掛けた累積値です。

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


ステータス日または本日の日付までの累積時間フェーズベースラインコストです。

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


予算コストリソースの予算コストです。予算リソースはプロジェクトサマリタスクにのみ割り当てられます。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


予算作業は予算作業および資材リソースに対して行われます。予算リソースはプロジェクトのサマリタスクにのみ割り当てられます。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


タスクのカレンダーです。

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Byte> COMMITMENT_FINISH
```


配達の完了日です。

--------------------

XML フォーマットのみで読み取りがサポートされています。

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Byte> COMMITMENT_START
```


配達の開始日です。

--------------------

XML フォーマットのみで読み取りがサポートされています。

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Byte> COMMITMENT_TYPE
```


タスクに関連する配信があるか、または関連する配信への依存関係があるかを判定します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Byte> CONSTRAINT_DATE
```


制約タイプに関連付けられた特定の日付です。

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Byte> CONSTRAINT_TYPE
```


タスクのスケジューリングに適用できる制約タイプの選択肢を提供します。

### CONTACT {#CONTACT}
```
public static final Key<String,Byte> CONTACT
```


タスクの責任者の名前です。

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


タスクに割り当てられたリソースが実施した作業で既に発生したコストと、残りの作業に計画されたコストを合計した、タスクの総予定コストまたは予測コストです。

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


タスク、リソース、または割り当てのベースラインコストと総コストとの差です。

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


タスクが作成された日付です。

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


タスクのベースラインコストと総コストの差。コスト差異 = コスト - ベースラインコスト

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Byte> DEADLINE
```


タスクの完了予定日を示す目標日です。

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Byte> DISPLAY_AS_SUMMARY
```


タスクをサマリータスクとして表示すべきかどうかを判定します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Byte> DISPLAY_ON_TIMELINE
```


タスクをタイムラインビューに表示すべきかどうかを指定します。

### DURATION {#DURATION}
```
public static final Key<Duration,Byte> DURATION
```


開始日、終了日、カレンダー、その他のスケジューリング要因に基づき、Microsoft Project が入力または計算したタスクのアクティブ作業時間の合計期間です。

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Byte> DURATION_TEXT
```


タスクの期間テキストを返します。

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Byte> DURATION_VARIANCE
```


タスクのベースライン期間と総期間（現在の見積もり）の差です。

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Byte> EARLY_FINISH
```


前任タスクと後続タスクの早期終了日、その他の制約、レベリング遅延を考慮した、タスクが最も早く完了できる日付です。

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Byte> EARLY_START
```


前任タスクと後続タスクの早期開始日、その他の制約に基づく、タスクが最も早く開始できる日付です。

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


実績コスト（BCWP）を計算する際に、% 完了または物理的 % 完了フィールドのどちらを使用すべきかを判定します。

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Byte> EXTERNAL_ID
```


タスクが外部タスクの場合、そのタスクの外部 ID が含まれます。

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Byte> EXTERNAL_TASK_PROJECT
```


外部タスクのソース位置とタスク識別子です。

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Byte> EXTERNAL_UID
```


タスクが外部の場合、外部タスクの一意識別子が含まれます。

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


タスクの予定終了日です。

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FINISH_SLACK_TIME_SPAN
```


早期終了日と遅延終了日の間の期間（秒）です。

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Byte> FINISH_TEXT
```


タスクの終了テキストを返します。

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


タスクまたは割り当てのベースライン終了日と現在の終了日の差を表す時間です。

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Byte> FIXED_COST
```


リソース以外のタスク費用を表示します。

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> FIXED_COST_ACCRUAL
```


タスクのコストに対して、固定費をいつ、どのように請求または発生させるかの選択肢を決定します。

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FREE_SLACK_TIME_SPAN
```


後続タスクを遅延させずにタスクを遅延できる時間（秒）です。

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


タスクに生成される一意の識別コードです。

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Byte> HAS_OVERALLOCATED_RESOURCE
```


タスクに割り当てられたリソースが、通常の作業容量内で完了できる以上の作業を持っているかどうかを示します。

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Byte> HIDE_BAR
```


Microsoft Projectで表示される際に、タスクのガントバーが非表示になるかどうかを決定します。

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


タスクに関連付けられたハイパーリンクのタイトルまたは説明テキストです。

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


タスクに関連付けられたハイパーリンクのアドレスです。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


タスクに関連付けられたハイパーリンク内のドキュメントの特定位置。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


タスク一覧内でのタスクの位置識別子です。

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Byte> IGNORE_RESOURCE_CALENDAR
```


タスクのスケジューリングが、割り当てられたリソースのカレンダーを考慮するかどうかを決定します。

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Byte> IGNORE_WARNINGS
```


Microsoft Projectでスケジュール競合警告インジケーターを非表示にするかどうかを示します。

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Byte> IS_ACTIVE
```


タスクがアクティブかどうかを判断します。非アクティブなタスクは他のタスクやプロジェクト全体のスケジュールに影響しなくなります。

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Byte> IS_CRITICAL
```


タスクがクリティカルパス上にあるかどうかを決定します。

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> IS_EFFORT_DRIVEN
```


タスクのスケジューリングが作業量主導かどうかを決定します。

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Byte> IS_ESTIMATED
```


タスクが見積もりかどうかを決定します。

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Byte> IS_EXPANDED
```


ガントチャートビューでサマリータスクが展開されているかどうかを決定します。

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Byte> IS_EXTERNAL_TASK
```


タスクが外部タスクかどうかを決定します。

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Byte> IS_MANUAL
```


タスクが手動でスケジュールされているかどうかを決定します。

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Byte> IS_MARKED
```


タスクが何らかの追加アクションや識別のためにマークされているかどうかを示します。

--------------------

mppファイル形式にのみ適用されます。

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Byte> IS_MILESTONE
```


タスクがマイルストーンかどうかを決定します。

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


タスクがヌルタスクかどうかを決定します。

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Byte> IS_OVERALLOCATED
```


タスクに割り当てられたリソースのいずれかが、通常の作業容量内で完了できる以上の作業を割り当てられているかどうかを示します。

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Byte> IS_PUBLISHED
```


現在のタスクをプロジェクト全体とともに Project Server に公開すべきかどうかを決定します。

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Byte> IS_RECURRING
```


タスクが繰り返しタスクのシリーズの一部かどうかを決定します。

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Byte> IS_RESUME_VALID
```


タスクを再開できるかどうかを決定します。

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Byte> IS_ROLLUP
```


サブタスクのガントバーに関する情報がサマリータスクバーに集約されるかどうかを決定します。

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Byte> IS_SUBPROJECT
```


タスクが挿入されたプロジェクトかどうかを判断します。

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Byte> IS_SUBPROJECT_READ_ONLY
```


サブプロジェクトが読み取り専用かどうかを判断します。

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Byte> IS_SUMMARY
```


タスクがサマリータスクかどうかを判断します。

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Byte> LATE_FINISH
```


プロジェクトの完了を遅らせずにタスクが完了できる最も遅い日付です。

### LATE_START {#LATE-START}
```
public static final Key<Date,Byte> LATE_START
```


プロジェクトの完了を遅らせずにタスクが開始できる最も遅い日付です。

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Byte> LEVELING_CAN_SPLIT
```


リソースレベリング機能がこのタスクの残り作業を分割させるかどうかを判断します。

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


リソースレベリングのためにタスクが早期開始日から遅延する時間です。

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Byte> LEVEL_ASSIGNMENTS
```


レベリング機能が過剰割り当てを解消するために個々の割り当てを遅延および分割できるかどうかを判断します。

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Byte> MANUAL_DURATION
```


タスクの手動スケジュール期間を定義します。

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Byte> MANUAL_FINISH
```


タスクの手動スケジュール完了日時を定義します。

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Byte> MANUAL_START
```


タスクの手動スケジュール開始日時を定義します。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


タスクの名前です。

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


RTF 形式のテキストノートです。

--------------------

MPP 形式のみサポートされています。

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


RTF データから抽出されたノートのプレーンテキストです。

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Byte> OUTLINE_LEVEL
```


タスクのアウトラインレベルです。

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Byte> OUTLINE_NUMBER
```


階層アウトライン構造におけるタスクの位置を表す番号です。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


タスクの総残業コスト、割り当てられたすべてのタスクに対するリソースの残業コスト、またはリソース割り当ての残業コストです。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


タスクに割り当てられたすべてのリソースが実施する予定の残業量です。

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_COMPLETE
```


タスクの現在のステータスで、タスク期間の完了した割合として表されます。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


タスクの現在のステータスで、完了した作業の割合として表されます。

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PHYSICAL_PERCENT_COMPLETE
```


実績コスト（BCWP）を計算する代替として使用できる完了率の値です。

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Byte> PRELEVELED_FINISH
```


リソースレベリング実施前のタスクの完了日です。

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Byte> PRELEVELED_START
```


リソースレベリング実施前のタスクの開始日です。

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Byte> PRIORITY
```


タスクに付与された重要度レベルで、リソースレベリング中にタスクや割り当てがどれだけ容易に遅延または分割できるかを示します。

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


リソースが実施する予定の総非残業作業量です。

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


残りの予定作業を完了する際に発生する残りの予定費用です。

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Byte> REMAINING_DURATION
```


タスクの未完了部分を完了するために必要な時間です。

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


タスクの残りの予定残業費用です。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


残りの予定残業時間の量。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


タスクまたはタスク群を完了するためにまだ必要な時間です。

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


タスクの残り部分が進捗に入った後に再開する予定の日付。

### START {#START}
```
public static final Key<Date,Byte> START
```


タスクの予定開始日。

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> START_SLACK_TIME_SPAN
```


早期開始日と遅延開始日間の期間（秒）。

### START_TEXT {#START-TEXT}
```
public static final Key<String,Byte> START_TEXT
```


タスクの開始テキストを返します。

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


タスクまたは割り当てのベースライン開始日と現在の予定開始日の差を表す時間。

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Byte> STATUS_MANAGER
```


現在のタスクに関するステータス更新をリソースから受け取る企業リソースの名前。

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


タスクの実際の部分の終了を示す日付。

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Byte> SUBPROJECT_NAME
```


サブプロジェクトのソース場所。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


プロジェクトステータス日までの獲得価値スケジュール差異。スケジュール差異（SV）はBCWPとBCWSの差です。

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> TOTAL_SLACK_TIME_SPAN
```


タスクの完了日がプロジェクトの完了日を遅らせることなく遅延できる時間。

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


タスクのタイプ。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


タスクの一意のID。

### WARNING {#WARNING}
```
public static final Key<Boolean,Byte> WARNING
```


スケジュールの不一致があることを示すフラグを表します。

### WBS {#WBS}
```
public static final Key<String,Byte> WBS
```


作業分解構成 (WBS) コード。

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Byte> WBS_LEVEL
```


タスクの最右側のWBSレベル。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


割り当てられたすべてのリソースに対してタスクに予定されている合計時間。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


タスクのベースライン作業と現在予定されている作業との差。

