---
title: "Asn"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのプロパティを表します。"
type: docs
weight: 15
url: /ja/java/com.aspose.tasks/asn/
---

**Inheritance:**
java.lang.Object
```
public class Asn
```

[ResourceAssignment](../../com.aspose.tasks/resourceassignment) オブジェクトのプロパティを表します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [ACTUAL_COST](#ACTUAL-COST) | 割り当てで発生した実際のコストです。 |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | 割り当ての実際の完了日です。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 割り当てで発生した実際の残業コストです。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 割り当てで発生した実際の残業作業量です。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 実際の作業が保護される期間です。 |
| [ACTUAL_START](#ACTUAL-START) | 割り当ての実際の開始日です。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | 割り当てで発生した実際の作業量です。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 実際の残業作業が保護される期間です。 |
| [ACWP](#ACWP) | 割り当てでこれまでに実行された作業の実際のコストです。 |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | 割り当て所有者の名前。 |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | 割り当て所有者のグローバルに一意な識別子です。 |
| [BCWP](#BCWP) | 割り当てでこれまでに実行された作業の予算コストです。 |
| [BCWS](#BCWS) | 割り当て上の作業の予算コストです。 |
| [BOOKING_TYPE](#BOOKING-TYPE) | 割り当ての予約タイプです。 |
| [BUDGET_COST](#BUDGET-COST) | 割り当て上のリソースの予算コストです。 |
| [BUDGET_WORK](#BUDGET-WORK) | 割り当て上の作業または材料リソースの予算作業量です。 |
| [CONFIRMED](#CONFIRMED) | リソースがすべての割り当てを受け入れたかどうかを判断します。 |
| [COST](#COST) | 割り当ての予測または予定コストです。 |
| [COST_RATE_TABLE_TYPE](#COST-RATE-TABLE-TYPE) | この割り当てに使用されるコストレートテーブルです。 |
| [COST_VARIANCE](#COST-VARIANCE) | 割り当てのベースラインコストと総コストの差です。 |
| [CREATED](#CREATED) | 割り当てが作成された日付です。 |
| [CV](#CV) | 獲得価値コスト差異。 |
| [DELAY](#DELAY) | 割り当ての遅延。 |
| [FINISH](#FINISH) | 割り当ての予定完了日。 |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | 割り当て完了日がベースライン完了日からの差異。 |
| [FIXED_MATERIAL](#FIXED-MATERIAL) | 割り当てられた材料リソースの消費が単一の固定量で行われるかどうかを決定します。 |
| [HAS_FIXED_RATE_UNITS](#HAS-FIXED-RATE-UNITS) | 単位が固定レートかどうかを決定します。 |
| [HYPERLINK](#HYPERLINK) | 割り当てに関連付けられたハイパーリンクのタイトルまたは説明テキスト。 |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 割り当てに関連付けられたハイパーリンクのアドレス。 |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 割り当てに関連付けられたハイパーリンク内のドキュメントの特定位置。 |
| [LEVELING_DELAY](#LEVELING-DELAY) | レベリングによって生じる遅延。 |
| [LINKED_FIELDS](#LINKED-FIELDS) | プロジェクトが別の OLE オブジェクトにリンクされているかどうかを決定します。 |
| [MILESTONE](#MILESTONE) | 割り当てがマイルストーンかどうかを決定します。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 形式のテキストノートです。 |
| [NOTES_TEXT](#NOTES-TEXT) | RTF データから抽出されたノートのプレーンテキストです。 |
| [OVERALLOCATED](#OVERALLOCATED) | 割り当てが過剰割り当てかどうかを決定します。 |
| [OVERTIME_COST](#OVERTIME-COST) | 割り当ての実際の残業コストと残りの残業コストの合計。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | 割り当ての予定残業作業。 |
| [PEAK_UNITS](#PEAK-UNITS) | タスクに対してリソースが割り当てられる最大単位数。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 割り当てで完了した作業量。 |
| [RATE_SCALE](#RATE-SCALE) | 材料リソース割り当ての使用率の時間単位。 |
| [REGULAR_WORK](#REGULAR-WORK) | 割り当ての予定非残業作業量。 |
| [REMAINING_COST](#REMAINING-COST) | 割り当て完了のための残りの予測コスト。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 割り当て完了のための残りの予測残業コスト。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 割り当て完了のために予定された残りの残業作業。 |
| [REMAINING_WORK](#REMAINING-WORK) | 割り当て完了のために予定された残りの作業。 |
| [RESOURCE](#RESOURCE) | タスクに割り当てられたリソース。 |
| [RESPONSE_PENDING](#RESPONSE-PENDING) | TeamAssign メッセージの応答が受信されたかどうかを決定します。 |
| [RESUME](#RESUME) | 割り当てが再開される日付。 |
| [START](#START) | 割り当ての予定開始日。 |
| [START_VARIANCE](#START-VARIANCE) | 割り当て開始日と基準開始日との差異。 |
| [STOP](#STOP) | 割り当てが停止される日付。 |
| [SUMMARY](#SUMMARY) | タスクがサマリータスクかどうかを決定します。 |
| [SV](#SV) | プロジェクトステータス日までの実績価値スケジュール差異です。 |
| [TASK](#TASK) | リソースが割り当てられるタスク。 |
| [UID](#UID) | 割り当ての一意の識別子。 |
| [UNITS](#UNITS) | 割り当ての単位数。 |
| [UPDATE_NEEDED](#UPDATE-NEEDED) | タスクに割り当てられたリソースのタスクステータスに関する更新が必要かどうかを決定します。 |
| [VAC](#VAC) | ベースラインコストと総コストの差。 |
| [WORK](#WORK) | 割り当ての予定作業量。 |
| [WORK_CONTOUR](#WORK-CONTOUR) | 割り当ての作業コンター。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | タスクのベースライン作業と現在予定されている作業との差。 |
### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


割り当てで発生した実際のコストです。

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


割り当ての実際の完了日です。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


割り当てで発生した実際の残業コストです。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


割り当てで発生した実際の残業作業量です。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


実際の作業が保護される期間です。

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


割り当ての実際の開始日です。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


割り当てで発生した実際の作業量です。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


実際の残業作業が保護される期間です。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


割り当てでこれまでに実行された作業の実際のコストです。

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


割り当て所有者の名前。

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


割り当て所有者のグローバルに一意な識別子です。

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


割り当てでこれまでに実行された作業の予算コストです。

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


割り当て上の作業の予算コストです。

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


割り当ての予約タイプです。

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


割り当て上のリソースの予算コストです。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


割り当て上の作業または材料リソースの予算作業量です。

### CONFIRMED {#CONFIRMED}
```
public static final Key<Boolean,Byte> CONFIRMED
```


リソースがすべての割り当てを受け入れたかどうかを判断します。

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


割り当ての予測または予定コストです。

### COST_RATE_TABLE_TYPE {#COST-RATE-TABLE-TYPE}
```
public static final Key<Integer,Byte> COST_RATE_TABLE_TYPE
```


この割り当てに使用されるコストレートテーブルです。

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


割り当てのベースラインコストと総コストの差です。

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


割り当てが作成された日付です。

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


実績価値コスト差異。CV は割り当ての BCWP（実施作業の予算コスト）と ACWP（実施作業の実際コスト）の差です。

### DELAY {#DELAY}
```
public static final Key<Duration,Byte> DELAY
```


割り当ての遅延。

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


割り当ての予定完了日。

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


割り当て完了日がベースライン完了日からの差異。

### FIXED_MATERIAL {#FIXED-MATERIAL}
```
public static final Key<Boolean,Byte> FIXED_MATERIAL
```


割り当てられた材料リソースの消費が単一の固定量で行われるかどうかを決定します。

### HAS_FIXED_RATE_UNITS {#HAS-FIXED-RATE-UNITS}
```
public static final Key<Boolean,Byte> HAS_FIXED_RATE_UNITS
```


単位が固定レートかどうかを決定します。

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


割り当てに関連付けられたハイパーリンクのタイトルまたは説明テキスト。

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


割り当てに関連付けられたハイパーリンクのアドレス。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


割り当てに関連付けられたハイパーリンク内のドキュメントの特定位置。

--------------------

ハイパーリンクの完全なアドレス（Microsoft Project の Hyperlink Href）は、HyperlinkAddress と HyperlinkSubAddress を連結したものです。

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


レベリングによって生じる遅延。

### LINKED_FIELDS {#LINKED-FIELDS}
```
public static final Key<Boolean,Byte> LINKED_FIELDS
```


プロジェクトが別の OLE オブジェクトにリンクされているかどうかを決定します。

### MILESTONE {#MILESTONE}
```
public static final Key<Boolean,Byte> MILESTONE
```


割り当てがマイルストーンかどうかを決定します。

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
public static final Key<Boolean,Byte> OVERALLOCATED
```


割り当てが過剰割り当てかどうかを決定します。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


割り当ての実際の残業コストと残りの残業コストの合計。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


割り当ての予定残業作業。

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


タスクに対してリソースが割り当てられる最大単位数。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


割り当てで完了した作業量。

### RATE_SCALE {#RATE-SCALE}
```
public static final Key<Integer,Byte> RATE_SCALE
```


素材リソース割り当ての使用率の時間単位。未定義の場合は 0 を返します。

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


割り当ての予定非残業作業量。

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


割り当て完了のための残りの予測コスト。

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


割り当て完了のための残りの予測残業コスト。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


割り当て完了のために予定された残りの残業作業。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


割り当て完了のために予定された残りの作業。

### RESOURCE {#RESOURCE}
```
public static final Key<Resource,Byte> RESOURCE
```


タスクに割り当てられたリソース。

### RESPONSE_PENDING {#RESPONSE-PENDING}
```
public static final Key<Boolean,Byte> RESPONSE_PENDING
```


TeamAssign メッセージの応答が受信されたかどうかを決定します。

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


割り当てが再開される日付。

### START {#START}
```
public static final Key<Date,Byte> START
```


割り当ての予定開始日。

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


割り当て開始日と基準開始日との差異。

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


割り当てが停止される日付。

### SUMMARY {#SUMMARY}
```
public static final Key<Boolean,Byte> SUMMARY
```


タスクがサマリータスクかどうかを決定します。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


プロジェクトステータス日までの獲得価値スケジュール差異。スケジュール差異（SV）はBCWPとBCWSの差です。

### TASK {#TASK}
```
public static final Key<Task,Byte> TASK
```


リソースが割り当てられるタスク。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


割り当ての一意の識別子。

### UNITS {#UNITS}
```
public static final Key<Double,Byte> UNITS
```


割り当ての単位数。

### UPDATE_NEEDED {#UPDATE-NEEDED}
```
public static final Key<Boolean,Byte> UPDATE_NEEDED
```


タスクに割り当てられたリソースのタスクステータスに関する更新が必要かどうかを決定します。

### VAC {#VAC}
```
public static final Key<Double,Byte> VAC
```


ベースラインコストと総コストの差。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


割り当ての予定作業量。

### WORK_CONTOUR {#WORK-CONTOUR}
```
public static final Key<Integer,Byte> WORK_CONTOUR
```


割り当ての作業コンター。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


タスクのベースライン作業と現在予定されている作業との差。

