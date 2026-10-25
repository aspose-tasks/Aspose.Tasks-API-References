---
title: "Prj"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのサポートされているプロパティを表します。"
type: docs
weight: 216
url: /ja/java/com.aspose.tasks/prj/
---

**Inheritance:**
java.lang.Object
```
public class Prj
```

[Project](../../com.aspose.tasks/project) オブジェクトのサポートされているプロパティを表します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [ACTUALS_IN_SYNC](#ACTUALS-IN-SYNC) | すべての実績作業がプロジェクトと同期されているかどうかを決定します。 |
| [ADMIN_PROJECT](#ADMIN-PROJECT) | プロジェクトが管理プロジェクトかどうかを決定します。 |
| [ARE_EDITABLE_ACTUAL_COSTS](#ARE-EDITABLE-ACTUAL-COSTS) | 実績コストが編集可能かどうかを決定します。 |
| [AUTHOR](#AUTHOR) | プロジェクトの作成者。 |
| [AUTOLINK](#AUTOLINK) | 挿入または移動されたタスクが自動的にリンクされるかどうかを決定します。 |
| [AUTO_ADD_NEW_RESOURCES_AND_TASKS](#AUTO-ADD-NEW-RESOURCES-AND-TASKS) | 新しいリソースまたはタスクがリソースまたはタスクプールに自動的に追加されるかどうかを決定します。 |
| [AUTO_CALCULATE_ASSIGNMENT_COSTS](#AUTO-CALCULATE-ASSIGNMENT-COSTS) | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算すべきかどうかを決定します。 |
| [BASELINE_FOR_EARNED_VALUE](#BASELINE-FOR-EARNED-VALUE) | 分散値を計算するために使用される特定のベースライン。 |
| [CALENDAR](#CALENDAR) | プロジェクトのカレンダー。 |
| [CATEGORY](#CATEGORY) | プロジェクトのカテゴリ。 |
| [COMMENTS](#COMMENTS) | プロジェクトのコメント。 |
| [COMPANY](#COMPANY) | プロジェクトが作成された会社。 |
| [CREATION_DATE](#CREATION-DATE) | プロジェクトが作成された日時。 |
| [CRITICAL_SLACK_LIMIT](#CRITICAL-SLACK-LIMIT) | MS Project では、総余裕時間がこの日数以下の場合、タスクはクリティカルと見なされます。 |
| [CURRENCY_CODE](#CURRENCY-CODE) | ISO 4217で定義された3文字の通貨コード。 |
| [CURRENCY_DIGITS](#CURRENCY-DIGITS) | 小数点記号の後の桁数。 |
| [CURRENCY_SYMBOL](#CURRENCY-SYMBOL) | プロジェクトで使用される通貨記号。 |
| [CURRENCY_SYMBOL_POSITION](#CURRENCY-SYMBOL-POSITION) | 通貨記号の配置。 |
| [CURRENT_DATE](#CURRENT-DATE) | システム日付。 |
| [CUSTOM_DATE_FORMAT](#CUSTOM-DATE-FORMAT) | プロジェクトビューのカスタム日付形式。 |
| [DATE_FORMAT](#DATE-FORMAT) | プロジェクトビューの日付形式。 |
| [DAYS_PER_MONTH](#DAYS-PER-MONTH) | 月ごとの日数。 |
| [DEFAULT_FINISH_TIME](#DEFAULT-FINISH-TIME) | 新しいタスクのデフォルト完了時刻。 |
| [DEFAULT_FIXED_COST_ACCRUAL](#DEFAULT-FIXED-COST-ACCRUAL) | 固定費が発生する際のデフォルトタイプ。 |
| [DEFAULT_OVERTIME_RATE](#DEFAULT-OVERTIME-RATE) | 新しいリソースのデフォルト残業率。 |
| [DEFAULT_STANDARD_RATE](#DEFAULT-STANDARD-RATE) | 新しいリソースのデフォルト標準率。 |
| [DEFAULT_START_TIME](#DEFAULT-START-TIME) | 新しいタスクのデフォルト開始時刻。 |
| [DEFAULT_TASK_EV_METHOD](#DEFAULT-TASK-EV-METHOD) | タスクのデフォルト実績価値計算方法。 |
| [DEFAULT_TASK_TYPE](#DEFAULT-TASK-TYPE) | 新しいタスクのデフォルトタイプ。 |
| [DURATION_FORMAT](#DURATION-FORMAT) | 総期間を表す形式。 |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | 実績価値を計算するデフォルト方法。 |
| [EXTENDED_CREATION_DATE](#EXTENDED-CREATION-DATE) | 計算およびレポートに使用される日付。 |
| [FINISH_DATE](#FINISH-DATE) | プロジェクトの完了日。 |
| [FISCAL_YEAR_START](#FISCAL-YEAR-START) | 会計年度番号が使用されるかどうかを決定します。 |
| [FY_START_DATE](#FY-START-DATE) | 会計年度が開始する月。 |
| [GUID](#GUID) | プロジェクトのGUID。 |
| [HONOR_CONSTRAINTS](#HONOR-CONSTRAINTS) | タスクが制約日を遵守するかどうかを決定します。 |
| [HYPERLINK_BASE](#HYPERLINK-BASE) | プロジェクトのハイパーリンクベース。 |
| [INSERTED_PROJECTS_LIKE_SUMMARY](#INSERTED-PROJECTS-LIKE-SUMMARY) | サブタスクがサマリタスクとして計算されるかどうかを決定します。 |
| [KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED](#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED) | 手動タスクが自動スケジュールに変更されたとき、最も近い作業時間に保持されるかどうかを決定します。 |
| [KEYWORDS](#KEYWORDS) | プロジェクトのキーワード。 |
| [LAST_AUTHOR](#LAST-AUTHOR) | プロジェクトの最終作成者。 |
| [LAST_PRINTED](#LAST-PRINTED) | プロジェクトの最終印刷時刻。 |
| [LAST_SAVED](#LAST-SAVED) | プロジェクトが最後に保存された日時。 |
| [MANAGER](#MANAGER) | プロジェクトのマネージャー。 |
| [MICROSOFT_PROJECT_SERVER_URL](#MICROSOFT-PROJECT-SERVER-URL) | プロジェクトが NT ユーザーではなく Project Server ユーザーによって作成されたかどうかを決定します。 |
| [MINUTES_PER_DAY](#MINUTES-PER-DAY) | 1日あたりの分数。 |
| [MINUTES_PER_WEEK](#MINUTES-PER-WEEK) | 1週間あたりの分数。 |
| [MOVE_COMPLETED_ENDS_BACK](#MOVE-COMPLETED-ENDS-BACK) | ステータス日以降に開始予定だったが実際には早く開始されたタスクの完了部分の終了時点をステータス日に戻すかどうかを決定します。 |
| [MOVE_COMPLETED_ENDS_FORWARD](#MOVE-COMPLETED-ENDS-FORWARD) | ステータス日以前に完了予定だったが実際には後で開始されたタスクの完了部分の終了時点をステータス日に繰り上げるかどうかを決定します。 |
| [MOVE_REMAINING_STARTS_BACK](#MOVE-REMAINING-STARTS-BACK) | ステータス日以降に開始予定だったが実際には早く開始されたタスクの残り部分の開始時点をステータス日に戻すかどうかを決定します。 |
| [MOVE_REMAINING_STARTS_FORWARD](#MOVE-REMAINING-STARTS-FORWARD) | 後で開始される予定だったタスクの残り部分の開始時点をステータス日に繰り上げるかどうかを決定します。 |
| [MULTIPLE_CRITICAL_PATHS](#MULTIPLE-CRITICAL-PATHS) | 複数のクリティカルパスが計算されるかどうかを決定します。 |
| [NAME](#NAME) | プロジェクトの名前。 |
| [NEW_TASKS_ARE_MANUAL](#NEW-TASKS-ARE-MANUAL) | 新規タスクが手動として作成されるかどうかを決定します。 |
| [NEW_TASKS_EFFORT_DRIVEN](#NEW-TASKS-EFFORT-DRIVEN) | 新規タスクが労力駆動かどうかを決定します。 |
| [NEW_TASKS_ESTIMATED](#NEW-TASKS-ESTIMATED) | 既定で推定期間が表示されるかどうかを決定します。 |
| [NEW_TASK_START_DATE](#NEW-TASK-START-DATE) | 新規タスクの既定開始日タイプ。 |
| [PROJECT_EXTERNALLY_EDITED](#PROJECT-EXTERNALLY-EDITED) | プロジェクトが外部で編集されたかどうかを決定します。 |
| [REMOVE_FILE_PROPERTIES](#REMOVE-FILE-PROPERTIES) | 保存時にすべてのファイルプロパティが削除されるかどうかを決定します。 |
| [REVISION](#REVISION) | プロジェクトが保存された回数。 |
| [SAVE_VERSION](#SAVE-VERSION) | プロジェクト ファイルが保存された Microsoft Office Project のバージョン。 |
| [SCHEDULE_FROM_START](#SCHEDULE-FROM-START) | 開始日からプロジェクト スケジュールを前方に計算するかどうかを決定します。 |
| [SHOW_PROJECT_SUMMARY_TASK](#SHOW-PROJECT-SUMMARY-TASK) | ガントチャート ビューの上部にある独自のサマリ タスク バーとともに、単一の行でプロジェクト全体のサマリ情報を表示するかどうかを決定します。 |
| [SPLITS_IN_PROGRESS_TASKS](#SPLITS-IN-PROGRESS-TASKS) | 進行中のタスクを分割できるかどうかを決定します。 |
| [SPREAD_ACTUAL_COST](#SPREAD-ACTUAL-COST) | 実際のコストをステータス日まで分配するかどうかを決定します。 |
| [SPREAD_PERCENT_COMPLETE](#SPREAD-PERCENT-COMPLETE) | 完了率をステータス日まで分配するかどうかを決定します。 |
| [START_DATE](#START-DATE) | プロジェクトの開始日。 |
| [STATUS_DATE](#STATUS-DATE) | 進捗を表示したり、獲得価値合計を計算したりするためのステータス日。 |
| [SUBJECT](#SUBJECT) | プロジェクトの件名。 |
| [TASK_UPDATES_RESOURCE](#TASK-UPDATES-RESOURCE) | タスクの更新がリソースを更新するかどうかを決定します。 |
| [TEMPLATE](#TEMPLATE) | プロジェクトのテンプレート。 |
| [TIMESCALE_FINISH](#TIMESCALE-FINISH) | ビューのタイムスケールが終了する日付。 |
| [TIMESCALE_START](#TIMESCALE-START) | ビューのタイムスケールが開始する日付。 |
| [TITLE](#TITLE) | プロジェクトのタイトル。 |
| [UID](#UID) | プロジェクトの一意の ID。 |
| [UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS](#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS) | リンクが編集されたときに手動タスクを更新する必要があるかどうかを決定します。 |
| [WEEK_START_DAY](#WEEK-START-DAY) | 週の最初の日。 |
| [WORK_FORMAT](#WORK-FORMAT) | タスクの期間を表示するために使用される形式。 |
### ACTUALS_IN_SYNC {#ACTUALS-IN-SYNC}
```
public static final Key<NullableBool,Byte> ACTUALS_IN_SYNC
```


すべての実績作業がプロジェクトと同期されているかどうかを決定します。

### ADMIN_PROJECT {#ADMIN-PROJECT}
```
public static final Key<NullableBool,Byte> ADMIN_PROJECT
```


プロジェクトが管理プロジェクトかどうかを決定します。

### ARE_EDITABLE_ACTUAL_COSTS {#ARE-EDITABLE-ACTUAL-COSTS}
```
public static final Key<NullableBool,Byte> ARE_EDITABLE_ACTUAL_COSTS
```


実績コストが編集可能かどうかを決定します。

### AUTHOR {#AUTHOR}
```
public static final Key<String,Byte> AUTHOR
```


プロジェクトの作成者。

### AUTOLINK {#AUTOLINK}
```
public static final Key<NullableBool,Byte> AUTOLINK
```


挿入または移動されたタスクが自動的にリンクされるかどうかを決定します。

### AUTO_ADD_NEW_RESOURCES_AND_TASKS {#AUTO-ADD-NEW-RESOURCES-AND-TASKS}
```
public static final Key<NullableBool,Byte> AUTO_ADD_NEW_RESOURCES_AND_TASKS
```


新しいリソースまたはタスクがリソースまたはタスクプールに自動的に追加されるかどうかを決定します。

### AUTO_CALCULATE_ASSIGNMENT_COSTS {#AUTO-CALCULATE-ASSIGNMENT-COSTS}
```
public static final Key<Boolean,Byte> AUTO_CALCULATE_ASSIGNMENT_COSTS
```


割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算すべきかどうかを決定します。

### BASELINE_FOR_EARNED_VALUE {#BASELINE-FOR-EARNED-VALUE}
```
public static final Key<Integer,Byte> BASELINE_FOR_EARNED_VALUE
```


分散値を計算するために使用される特定のベースライン。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


プロジェクトのカレンダー。

### CATEGORY {#CATEGORY}
```
public static final Key<String,Byte> CATEGORY
```


プロジェクトのカテゴリ。

### COMMENTS {#COMMENTS}
```
public static final Key<String,Byte> COMMENTS
```


プロジェクトのコメント。

### COMPANY {#COMPANY}
```
public static final Key<String,Byte> COMPANY
```


プロジェクトが作成された会社。

### CREATION_DATE {#CREATION-DATE}
```
public static final Key<Date,Byte> CREATION_DATE
```


プロジェクトが作成された日時。

--------------------

mpp ファイルで UTC 形式で保存されます。java.util.Date 型。

### CRITICAL_SLACK_LIMIT {#CRITICAL-SLACK-LIMIT}
```
public static final Key<Integer,Byte> CRITICAL_SLACK_LIMIT
```


MS Project では、総余裕時間がこの日数以下の場合、タスクはクリティカルと見なされます。

### CURRENCY_CODE {#CURRENCY-CODE}
```
public static final Key<String,Byte> CURRENCY_CODE
```


ISO 4217 で定義された 3 文字の通貨コードです。有効な値の例は "USD" です。

### CURRENCY_DIGITS {#CURRENCY-DIGITS}
```
public static final Key<Integer,Byte> CURRENCY_DIGITS
```


小数点記号の後の桁数。

### CURRENCY_SYMBOL {#CURRENCY-SYMBOL}
```
public static final Key<String,Byte> CURRENCY_SYMBOL
```


プロジェクトで使用される通貨記号。

### CURRENCY_SYMBOL_POSITION {#CURRENCY-SYMBOL-POSITION}
```
public static final Key<Integer,Byte> CURRENCY_SYMBOL_POSITION
```


通貨記号の配置。

### CURRENT_DATE {#CURRENT-DATE}
```
public static final Key<Date,Byte> CURRENT_DATE
```


システム日付。

### CUSTOM_DATE_FORMAT {#CUSTOM-DATE-FORMAT}
```
public static final Key<String,Byte> CUSTOM_DATE_FORMAT
```


プロジェクト ビューのカスタム日付形式。[DATE\\_FORMAT](../../com.aspose.tasks/prj\\#DATE-FORMAT) プロパティが [DateFormat.Custom](../../com.aspose.tasks/dateformat\\#Custom) に設定されている場合に日付をフォーマットするために使用されます。

### DATE_FORMAT {#DATE-FORMAT}
```
public static final Key<Integer,Byte> DATE_FORMAT
```


プロジェクトビューの日付形式。

### DAYS_PER_MONTH {#DAYS-PER-MONTH}
```
public static final Key<Integer,Byte> DAYS_PER_MONTH
```


月ごとの日数。

### DEFAULT_FINISH_TIME {#DEFAULT-FINISH-TIME}
```
public static final Key<Date,Byte> DEFAULT_FINISH_TIME
```


新しいタスクのデフォルト完了時刻。

### DEFAULT_FIXED_COST_ACCRUAL {#DEFAULT-FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> DEFAULT_FIXED_COST_ACCRUAL
```


固定費が発生する際のデフォルトタイプ。

### DEFAULT_OVERTIME_RATE {#DEFAULT-OVERTIME-RATE}
```
public static final Key<Double,Byte> DEFAULT_OVERTIME_RATE
```


新しいリソースのデフォルト残業率。

### DEFAULT_STANDARD_RATE {#DEFAULT-STANDARD-RATE}
```
public static final Key<Double,Byte> DEFAULT_STANDARD_RATE
```


新しいリソースのデフォルト標準率。

### DEFAULT_START_TIME {#DEFAULT-START-TIME}
```
public static final Key<Date,Byte> DEFAULT_START_TIME
```


新しいタスクのデフォルト開始時刻。

### DEFAULT_TASK_EV_METHOD {#DEFAULT-TASK-EV-METHOD}
```
public static final Key<Integer,Byte> DEFAULT_TASK_EV_METHOD
```


タスクのデフォルト実績価値計算方法。

### DEFAULT_TASK_TYPE {#DEFAULT-TASK-TYPE}
```
public static final Key<Integer,Byte> DEFAULT_TASK_TYPE
```


新しいタスクのデフォルトタイプ。

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Byte,Byte> DURATION_FORMAT
```


バルク期間を表す形式。`TimeUnitType` 型。

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


実績価値を計算するデフォルト方法。

### EXTENDED_CREATION_DATE {#EXTENDED-CREATION-DATE}
```
public static final Key<Date,Byte> EXTENDED_CREATION_DATE
```


計算およびレポートに使用される日付。

### FINISH_DATE {#FINISH-DATE}
```
public static final Key<Date,Byte> FINISH_DATE
```


プロジェクトの完了日。

### FISCAL_YEAR_START {#FISCAL-YEAR-START}
```
public static final Key<NullableBool,Byte> FISCAL_YEAR_START
```


会計年度番号が使用されるかどうかを決定します。

### FY_START_DATE {#FY-START-DATE}
```
public static final Key<Integer,Byte> FY_START_DATE
```


会計年度が開始する月。

### GUID {#GUID}
```
public static final Key<UUID,Byte> GUID
```


プロジェクトのGUID。

### HONOR_CONSTRAINTS {#HONOR-CONSTRAINTS}
```
public static final Key<NullableBool,Byte> HONOR_CONSTRAINTS
```


タスクが制約日を遵守するかどうかを決定します。

### HYPERLINK_BASE {#HYPERLINK-BASE}
```
public static final Key<String,Byte> HYPERLINK_BASE
```


プロジェクトのハイパーリンクベース。

### INSERTED_PROJECTS_LIKE_SUMMARY {#INSERTED-PROJECTS-LIKE-SUMMARY}
```
public static final Key<NullableBool,Byte> INSERTED_PROJECTS_LIKE_SUMMARY
```


サブタスクがサマリタスクとして計算されるかどうかを決定します。

### KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED {#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED}
```
public static final Key<NullableBool,Byte> KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED
```


手動タスクが自動スケジュールに変更されたとき、最も近い作業時間に保持されるかどうかを決定します。

### KEYWORDS {#KEYWORDS}
```
public static final Key<String,Byte> KEYWORDS
```


プロジェクトのキーワード。

### LAST_AUTHOR {#LAST-AUTHOR}
```
public static final Key<String,Byte> LAST_AUTHOR
```


プロジェクトの最終作成者。

### LAST_PRINTED {#LAST-PRINTED}
```
public static final Key<Date,Byte> LAST_PRINTED
```


プロジェクトの最終印刷時刻。

--------------------

mpp ファイルで UTC 形式で保存されます。java.util.Date 型。

### LAST_SAVED {#LAST-SAVED}
```
public static final Key<Date,Byte> LAST_SAVED
```


プロジェクトが最後に保存された日時。

--------------------

mpp ファイルで UTC 形式で保存されます。java.util.Date 型。

### MANAGER {#MANAGER}
```
public static final Key<String,Byte> MANAGER
```


プロジェクトのマネージャー。

### MICROSOFT_PROJECT_SERVER_URL {#MICROSOFT-PROJECT-SERVER-URL}
```
public static final Key<NullableBool,Byte> MICROSOFT_PROJECT_SERVER_URL
```


プロジェクトが NT ユーザーではなく Project Server ユーザーによって作成されたかどうかを決定します。

### MINUTES_PER_DAY {#MINUTES-PER-DAY}
```
public static final Key<Integer,Byte> MINUTES_PER_DAY
```


1日あたりの分数。

### MINUTES_PER_WEEK {#MINUTES-PER-WEEK}
```
public static final Key<Integer,Byte> MINUTES_PER_WEEK
```


1週間あたりの分数。

### MOVE_COMPLETED_ENDS_BACK {#MOVE-COMPLETED-ENDS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_BACK
```


ステータス日以降に開始予定だったが実際には早く開始されたタスクの完了部分の終了時点をステータス日に戻すかどうかを決定します。

### MOVE_COMPLETED_ENDS_FORWARD {#MOVE-COMPLETED-ENDS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_FORWARD
```


ステータス日以前に完了予定だったが実際には後で開始されたタスクの完了部分の終了時点をステータス日に繰り上げるかどうかを決定します。

### MOVE_REMAINING_STARTS_BACK {#MOVE-REMAINING-STARTS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_BACK
```


ステータス日以降に開始予定だったが実際には早く開始されたタスクの残り部分の開始時点をステータス日に戻すかどうかを決定します。

### MOVE_REMAINING_STARTS_FORWARD {#MOVE-REMAINING-STARTS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_FORWARD
```


後で開始される予定だったタスクの残り部分の開始時点をステータス日に繰り上げるかどうかを決定します。

### MULTIPLE_CRITICAL_PATHS {#MULTIPLE-CRITICAL-PATHS}
```
public static final Key<NullableBool,Byte> MULTIPLE_CRITICAL_PATHS
```


複数のクリティカルパスが計算されるかどうかを決定します。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


プロジェクトの名前。

### NEW_TASKS_ARE_MANUAL {#NEW-TASKS-ARE-MANUAL}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ARE_MANUAL
```


新規タスクが手動として作成されるかどうかを決定します。

### NEW_TASKS_EFFORT_DRIVEN {#NEW-TASKS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> NEW_TASKS_EFFORT_DRIVEN
```


新規タスクが労力駆動かどうかを決定します。

### NEW_TASKS_ESTIMATED {#NEW-TASKS-ESTIMATED}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ESTIMATED
```


既定で推定期間が表示されるかどうかを決定します。

### NEW_TASK_START_DATE {#NEW-TASK-START-DATE}
```
public static final Key<Integer,Byte> NEW_TASK_START_DATE
```


新規タスクの既定開始日タイプ。

### PROJECT_EXTERNALLY_EDITED {#PROJECT-EXTERNALLY-EDITED}
```
public static final Key<NullableBool,Byte> PROJECT_EXTERNALLY_EDITED
```


プロジェクトが外部で編集されたかどうかを決定します。

### REMOVE_FILE_PROPERTIES {#REMOVE-FILE-PROPERTIES}
```
public static final Key<NullableBool,Byte> REMOVE_FILE_PROPERTIES
```


保存時にすべてのファイルプロパティが削除されるかどうかを決定します。

### REVISION {#REVISION}
```
public static final Key<Integer,Byte> REVISION
```


プロジェクトが保存された回数。

### SAVE_VERSION {#SAVE-VERSION}
```
public static final Key<Integer,Byte> SAVE_VERSION
```


プロジェクト ファイルが保存された Microsoft Office Project のバージョン。

### SCHEDULE_FROM_START {#SCHEDULE-FROM-START}
```
public static final Key<NullableBool,Byte> SCHEDULE_FROM_START
```


開始日からプロジェクト スケジュールを前方に計算するかどうかを決定します。

### SHOW_PROJECT_SUMMARY_TASK {#SHOW-PROJECT-SUMMARY-TASK}
```
public static final Key<Boolean,Byte> SHOW_PROJECT_SUMMARY_TASK
```


ガントチャート ビューの上部にある独自のサマリ タスク バーとともに、単一の行でプロジェクト全体のサマリ情報を表示するかどうかを決定します。

### SPLITS_IN_PROGRESS_TASKS {#SPLITS-IN-PROGRESS-TASKS}
```
public static final Key<NullableBool,Byte> SPLITS_IN_PROGRESS_TASKS
```


進行中のタスクを分割できるかどうかを決定します。

### SPREAD_ACTUAL_COST {#SPREAD-ACTUAL-COST}
```
public static final Key<NullableBool,Byte> SPREAD_ACTUAL_COST
```


実際のコストをステータス日まで分配するかどうかを決定します。

### SPREAD_PERCENT_COMPLETE {#SPREAD-PERCENT-COMPLETE}
```
public static final Key<NullableBool,Byte> SPREAD_PERCENT_COMPLETE
```


完了率をステータス日まで分配するかどうかを決定します。

### START_DATE {#START-DATE}
```
public static final Key<Date,Byte> START_DATE
```


プロジェクトの開始日。

### STATUS_DATE {#STATUS-DATE}
```
public static final Key<Date,Byte> STATUS_DATE
```


進捗を表示したり、獲得価値合計を計算したりするためのステータス日。別のステータス日が指定されていない限り、ステータス日は現在の日付（本日の日付）と同じです。

### SUBJECT {#SUBJECT}
```
public static final Key<String,Byte> SUBJECT
```


プロジェクトの件名。

### TASK_UPDATES_RESOURCE {#TASK-UPDATES-RESOURCE}
```
public static final Key<NullableBool,Byte> TASK_UPDATES_RESOURCE
```


タスクの更新がリソースを更新するかどうかを決定します。

### TEMPLATE {#TEMPLATE}
```
public static final Key<String,Byte> TEMPLATE
```


プロジェクトのテンプレート。

### TIMESCALE_FINISH {#TIMESCALE-FINISH}
```
public static final Key<Date,Byte> TIMESCALE_FINISH
```


ビューのタイムスケールが終了する日付。

### TIMESCALE_START {#TIMESCALE-START}
```
public static final Key<Date,Byte> TIMESCALE_START
```


ビューのタイムスケールが開始する日付。

### TITLE {#TITLE}
```
public static final Key<String,Byte> TITLE
```


プロジェクトのタイトル。

### UID {#UID}
```
public static final Key<String,Byte> UID
```


プロジェクトの一意の ID。

### UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS {#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS}
```
public static final Key<NullableBool,Byte> UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS
```


リンクが編集されたときに手動タスクを更新する必要があるかどうかを決定します。

### WEEK_START_DAY {#WEEK-START-DAY}
```
public static final Key<Integer,Byte> WEEK_START_DAY
```


週の最初の日。

### WORK_FORMAT {#WORK-FORMAT}
```
public static final Key<Byte,Byte> WORK_FORMAT
```


タスクの期間を表示するために使用される形式。

