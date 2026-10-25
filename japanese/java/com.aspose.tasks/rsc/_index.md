---
title: "Rsc"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Resource オブジェクトのサポートされているプロパティを表します。"
type: docs
weight: 271
url: /ja/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

`Resource` オブジェクトのサポートされているプロパティを表します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | リソースの標準コストと残業コストをタスクのコストに対していつ、どのように課金または発生させるかを決定します。 |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | リソースの Active Directory Guid。 |
| [ACTUAL_COST](#ACTUAL-COST) | リソースがタスクで既に実施した作業に対して発生したコストと、タスクに関連するその他の記録されたコスト。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 割り当てられたリソースがタスクで既に実施した残業作業に対して発生したコスト。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | タスクに割り当てられたリソースが既に実施した実際の残業作業量。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 実際の残業作業が保護される作業量。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | タスクに割り当てられたリソースが既に実施した作業量。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 実際の作業が保護される作業量。 |
| [ACWP](#ACWP) | プロジェクトにおいてリソースが実施した作業の現在までの実際のコスト。 |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | 割り当て所有者の名前。 |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | 割り当て所有者の GUID。 |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | リソースが現在の期間で指定された単位で作業可能になる開始日。 |
| [AVAILABLE_TO](#AVAILABLE-TO) | リソースが現在の期間で指定された単位で作業可能な終了日。 |
| [BCWP](#BCWP) | リソースがプロジェクトでこれまでに実施した作業の予算コスト。 |
| [BCWS](#BCWS) | リソースに予定された作業の予算コスト。 |
| [BOOKING_TYPE](#BOOKING-TYPE) | リソースの予約タイプ。 |
| [BUDGET_COST](#BUDGET-COST) | 予算コストリソースの予算コスト。 |
| [BUDGET_WORK](#BUDGET-WORK) | 予算作業および資材リソースの予算作業。 |
| [CALENDAR](#CALENDAR) | リソースのカレンダー。 |
| [CAN_LEVEL](#CAN-LEVEL) | リソースのレベル調整が可能かどうかを決定する。 |
| [CODE](#CODE) | リソースに関するコードまたはその他の情報。 |
| [COST](#COST) | タスクに割り当てられたリソースが実施した作業で既に発生したコストと、残りの作業に計画されたコストに基づく、リソースの総予定または予測コスト。 |
| [COST_CENTER](#COST-CENTER) | リソースが発生したコストを請求すべきコストセンターを示す。 |
| [COST_PER_USE](#COST-PER-USE) | リソースが使用されるたびに発生するコスト。 |
| [COST_VARIANCE](#COST-VARIANCE) | リソースのベースラインコストと総コストの差異。 |
| [CREATED](#CREATED) | リソースがプロジェクトに追加された日時。 |
| [CV](#CV) | プロジェクトステータス日までの獲得価値コスト差異。 |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | リソースのメールアドレス。 |
| [FINISH](#FINISH) | リソースが割り当てられたすべてのタスクの作業を完了する予定日。 |
| [GROUP](#GROUP) | リソースが所属するグループ。 |
| [GUID](#GUID) | リソースの生成された一意の識別コードを含む。 |
| [HYPERLINK](#HYPERLINK) | リソースに関連付けられたハイパーリンクのタイトルまたは説明テキスト。 |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | リソースに関連付けられたハイパーリンクのアドレス。 |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | タスクに関連付けられたハイパーリンク内のドキュメントの特定位置。 |
| [ID](#ID) | リソース一覧内のリソース位置識別子。 |
| [INACTIVE](#INACTIVE) | 管理者権限を持つユーザーによってリソースが非アクティブ化されたかどうかを決定する。 |
| [INITIALS](#INITIALS) | リソースのイニシャル。 |
| [IS_BUDGET](#IS-BUDGET) | 作業、資材、またはコストリソースが予算リソースかどうかを判断します。 |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | リソースがコストリソースかどうかを判断します。 |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | リソースがエンタープライズリソースプールからのものか（true）、ローカルリソースプールからのものか（false）を示します。 |
| [IS_GENERIC](#IS-GENERIC) | リソースが汎用かどうかを判断します。 |
| [IS_NULL](#IS-NULL) | リソースが null かどうかを判断します。 |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | 現在のリソースがチームリソースかどうかを示します。 |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | 資材リソースの測定単位です。 |
| [MAX_UNITS](#MAX-UNITS) | リソースが現在の期間中にタスクを実行できる最大容量を表す単位数の上限です。 |
| [NAME](#NAME) | リソースの名前です。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 形式のテキストノートです。 |
| [NOTES_TEXT](#NOTES-TEXT) | RTF データから抽出されたノートのプレーンテキストです。 |
| [OVERALLOCATED](#OVERALLOCATED) | リソースが特定のタスクまたはすべてのタスクで、通常の作業容量内で完了できる以上の作業に割り当てられているかどうかを示します。 |
| [OVERTIME_COST](#OVERTIME-COST) | リソースが割り当てられたすべてのタスクに対する総残業コストです。 |
| [OVERTIME_RATE](#OVERTIME-RATE) | リソースが行う残業作業の給与率です。 |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Microsoft Project が残業率を表示するために使用する単位です。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | リソースがタスクで実施する予定の残業量で、関係するリソースの残業率で請求されます。 |
| [PEAK_UNITS](#PEAK-UNITS) | リソースが割り当てられたすべてのタスクに対し、任意の時点での最大割り当て単位です。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | すべてのタスクで完了した作業の割合です。 |
| [PHONETICS](#PHONETICS) | リソース名の音声表記です。 |
| [REGULAR_WORK](#REGULAR-WORK) | リソースが実施する予定の残業以外の作業の総量です。 |
| [REMAINING_COST](#REMAINING-COST) | 残りの予定作業を完了する際に発生する残りの予定費用です。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | リソースの残りの予定残業費用です。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 残りの予定残業量です。 |
| [REMAINING_WORK](#REMAINING-WORK) | タスクまたはタスク群を完了するためにまだ必要な時間です。 |
| [STANDARD_RATE](#STANDARD-RATE) | リソースが行う通常の残業なし作業の給与率です。 |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Microsoft Project が標準料金を表示するために使用する単位です。 |
| [START](#START) | 割り当てられたリソースがタスクで作業を開始するようにスケジュールされた日付です。 |
| [SV](#SV) | プロジェクトステータス日までの実績価値スケジュール差異です。 |
| [TYPE](#TYPE) | リソースのタイプです。 |
| [UID](#UID) | リソースの一意識別子です。 |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | リソースに関連付けられた NT アカウントです。 |
| [WORK](#WORK) | タスク上でリソースにスケジュールされた合計時間です。 |
| [WORKGROUP](#WORKGROUP) | リソースが所属するワークグループのタイプです。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | リソースのベースライン作業と現在スケジュールされた作業との差です。 |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


リソースの標準コストと残業コストをタスクのコストに対していつ、どのように課金または発生させるかを決定します。

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


リソースの Active Directory Guid。

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


リソースがタスクで既に実施した作業に対して発生したコストと、タスクに関連するその他の記録されたコスト。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


割り当てられたリソースがタスクで既に実施した残業作業に対して発生したコスト。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


タスクに割り当てられたリソースが既に実施した実際の残業作業量。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


実際の残業作業が保護される作業量。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


タスクに割り当てられたリソースが既に実施した作業量。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


実際の作業が保護される作業量。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


プロジェクトにおいてリソースが実施した作業の現在までの実際のコスト。

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


割り当て所有者の名前。

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


割り当て所有者の GUID。

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


リソースが現在の期間で指定された単位で作業可能になる開始日。

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


リソースが現在の期間で指定された単位で作業可能な終了日。

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


リソースがプロジェクトでこれまでに実施した作業の予算コスト。

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


リソースに予定された作業の予算コスト。

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


リソースの予約タイプ。

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


予算コストリソースの予算コストです。予算リソースはプロジェクトサマリタスクにのみ割り当てられます。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


予算作業は予算作業および資材リソース用です。予算リソースはプロジェクトサマリタスクにのみ割り当てられます。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


リソースのカレンダー。

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


リソースのレベル調整が可能かどうかを決定する。

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


リソースに関するコードまたはその他の情報。

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


タスクに割り当てられたリソースが実施した作業で既に発生したコストと、残りの作業に計画されたコストに基づく、リソースの総予定または予測コスト。

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


リソースが発生したコストを請求すべきコストセンターを示す。

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


リソースが使用されるたびに発生するコスト。

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


リソースのベースラインコストと総コストの差異。

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


リソースがプロジェクトに追加された日時。

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


プロジェクトステータス日までの実績価値コスト差異です。CV はタスクの BCWP（実績作業の予算コスト）と ACWP（実績作業の実コスト）の差です。

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


リソースのメールアドレス。

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


リソースが割り当てられたすべてのタスクの作業を完了する予定日。

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


リソースが所属するグループ。

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


リソースの生成された一意の識別コードを含む。

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


リソースに関連付けられたハイパーリンクのタイトルまたは説明テキスト。

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


リソースに関連付けられたハイパーリンクのアドレス。

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


リソース一覧内のリソース位置識別子。

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


管理者権限を持つユーザーによってリソースが非アクティブ化されたかどうかを決定する。

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


リソースのイニシャル。

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


作業、資材、またはコストリソースが予算リソースかどうかを判断します。

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


リソースがコストリソースかどうかを判断します。

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


リソースがエンタープライズリソースプールからのものか（true）、ローカルリソースプールからのものか（false）を示します。

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


リソースが汎用かどうかを判断します。

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


リソースが null かどうかを判断します。

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


現在のリソースがチームリソースかどうかを示します。

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


資材リソースの測定単位です。

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


リソースが現在の期間中にタスクを実行できる最大容量を表す単位数の上限です。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


リソースの名前です。

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

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


リソースが特定のタスクまたはすべてのタスクで、通常の作業容量内で完了できる以上の作業に割り当てられているかどうかを示します。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


リソースが割り当てられたすべてのタスクに対する総残業コストです。

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


リソースが行う残業作業の給与率です。

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Microsoft Project が残業率を表示するために使用する単位です。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


リソースがタスクで実施する予定の残業量で、関係するリソースの残業率で請求されます。

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


リソースが割り当てられたすべてのタスクに対し、任意の時点での最大割り当て単位です。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


すべてのタスクで完了した作業の割合です。

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


リソース名のふりがな表記です。日本語でのみ使用します。

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


リソースが実施する予定の残業以外の作業の総量です。

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


残りの予定作業を完了する際に発生する残りの予定費用です。

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


リソースの残りの予定残業費用です。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


残りの予定残業量です。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


タスクまたはタスク群を完了するためにまだ必要な時間です。

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


リソースが行う通常の残業なし作業の給与率です。

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Microsoft Project が標準料金を表示するために使用する単位です。

### START {#START}
```
public static final Key<Date,Byte> START
```


割り当てられたリソースがタスクで作業を開始するようにスケジュールされた日付です。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


プロジェクトステータス日までの実績価値スケジュール差異です。SV は実績作業の予算コスト（BCWP）と予定作業の予算コスト（BCWS）の差です。

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


リソースのタイプです。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


リソースの一意識別子です。

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


リソースに関連付けられた NT アカウントです。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


タスク上でリソースにスケジュールされた合計時間です。

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


リソースが所属するワークグループのタイプです。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


リソースのベースライン作業と現在スケジュールされた作業との差です。

