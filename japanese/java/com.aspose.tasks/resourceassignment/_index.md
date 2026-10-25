---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト内のリソース割り当てを表します。"
type: docs
weight: 249
url: /ja/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

プロジェクト内のリソース割り当てを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | このコンテナ内でプロパティがマッピングされている値を返します。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | このコンテナ内で指定されたプロパティを指定された値にマッピングします。 |
| [delete()](#delete--) | プロジェクト割り当てコレクションからリソース割り当てを削除します。 |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | このインスタンスが [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスの指定されたインスタンスと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getACWP()](#getACWP--) | ACWP の値を取得します。 |
| [getActualCost()](#getActualCost--) | ActualCost の値を取得します。 |
| [getActualFinish()](#getActualFinish--) | ActualFinish の値を取得します。 |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost の値を取得します。 |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork の値を取得します。 |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected の値を取得します。 |
| [getActualStart()](#getActualStart--) | ActualStart の値を取得します。 |
| [getActualWork()](#getActualWork--) | ActualWork の値を取得します。 |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected の値を取得します。 |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner の値を取得します。 |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid の値を取得します。 |
| [getBCWP()](#getBCWP--) | BCWP の値を取得します。 |
| [getBCWS()](#getBCWS--) | BCWS の値を取得します。 |
| [getBaselines()](#getBaselines--) | AssignmentBaselineCollection オブジェクトを取得します。 |
| [getBookingType()](#getBookingType--) | BookingType の値を取得します。 |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost の値を取得します。 |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork の値を取得します。 |
| [getCV()](#getCV--) | CV の値を取得します。 |
| [getConfirmed()](#getConfirmed--) | Confirmed が設定されているかどうかを示す値を取得します。 |
| [getCost()](#getCost--) | Cost の値を取得します。 |
| [getCostRateTableType()](#getCostRateTableType--) | CostRateTableType の値を取得します。 |
| [getCostVariance()](#getCostVariance--) | CostVariance の値を取得します。 |
| [getCreated()](#getCreated--) | Created の値を取得します。 |
| [getDelay()](#getDelay--) | Delay の値を取得します。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | このオブジェクトの ExtendedAttributeCollection クラスのインスタンスを取得します。 |
| [getFinish()](#getFinish--) | Finish の値を取得します。 |
| [getFinishVariance()](#getFinishVariance--) | FinishVariance の値を取得します。 |
| [getFixedMaterial()](#getFixedMaterial--) | FixedMaterial が設定されているかどうかを示す値を取得します。 |
| [getGuid()](#getGuid--) | この割り当ての一意の識別子を取得します。 |
| [getHyperlink()](#getHyperlink--) | Hyperlink の値を取得します。 |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | HyperlinkAddress の値を取得します。 |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | HyperlinkSubAddress の値を取得します。 |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | LevelingDelay の値を取得します。 |
| [getLinkedFields()](#getLinkedFields--) | LinkedFields が設定されているかどうかを示す値を取得します。 |
| [getMilestone()](#getMilestone--) | Milestone が設定されているかどうかを示す値を取得します。 |
| [getNotesRTF()](#getNotesRTF--) | RTF 形式のテキストノートを取得します。 |
| [getNotesText()](#getNotesText--) | RTF データから抽出されたノートのプレーンテキストを取得します。 |
| [getOverallocated()](#getOverallocated--) | Overallocated が設定されているかどうかを示す値を取得します。 |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost の値を取得します。 |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork の値を取得します。 |
| [getParentProject()](#getParentProject--) | この割り当ての親プロジェクトを取得します。 |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits の値を取得します。 |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete の値を取得します。 |
| [getRateScale()](#getRateScale--) | RateScale の値を取得します。 |
| [getRegularWork()](#getRegularWork--) | RegularWork の値を取得します。 |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost の値を取得します。 |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost の値を取得します。 |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork の値を取得します。 |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork の値を取得します。 |
| [getResource()](#getResource--) | タスクに割り当てられたリソース。 |
| [getResponsePending()](#getResponsePending--) | ResponsePending が設定されているかどうかを示す値を取得します。 |
| [getResume()](#getResume--) | Resume の値を取得します。 |
| [getSV()](#getSV--) | SV の値を取得します。 |
| [getStart()](#getStart--) | Start の値を取得します。 |
| [getStartVariance()](#getStartVariance--) | StartVariance の値を取得します。 |
| [getStop()](#getStop--) | Stop の値を取得します。 |
| [getSummary()](#getSummary--) | Summary が設定されているかどうかを示す値を取得します。 |
| [getTask()](#getTask--) | リソースが割り当てられるタスク。 |
| [getTimephasedData()](#getTimephasedData--) | `TimephasedData` の要素を含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを取得します（`TimephasedData` の [getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) メソッド）。 |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | 指定された開始日と終了日の [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) に対して、`TimephasedData` のインスタンスを含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトを返します（`TimephasedData` の [getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-) メソッド）。 |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | 指定された [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) の開始日と終了日の範囲内で、`TimephasedData` のインスタンスを含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを返します（`TimephasedData` の [getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-) メソッド）。 |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | 指定された日時間隔に対する時間別作業量を取得します。 |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | 指定された日時間隔に対する時間別作業量を取得します。 |
| [getUid()](#getUid--) | Uid の値を取得します。 |
| [getUnits()](#getUnits--) | Units の値を取得します。 |
| [getUpdateNeeded()](#getUpdateNeeded--) | UpdateNeeded が設定されているかどうかを示す値を取得します。 |
| [getVAC()](#getVAC--) | VAC の値を取得します。 |
| [getWork()](#getWork--) | Work の値を取得します。 |
| [getWorkContour()](#getWorkContour--) | WorkContour の値を取得します。 |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance の値を取得します。 |
| [hasChildren()](#hasChildren--) | このリソース割り当てに子があることを示す値を取得します。 |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | HasFixedRateUnits が設定されているかどうかを示す値を取得します。 |
| [hashCode()](#hashCode--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスに対するハッシュコード値を返します。 |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | 時間別データのリストを生成します。 |
| [setACWP(double value)](#setACWP-double-) | ACWP の値を設定します。 |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost の値を設定します。 |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | ActualFinish の値を設定します。 |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost の値を設定します。 |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork の値を設定します。 |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected の値を設定します。 |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | ActualStart の値を設定します。 |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork の値を設定します。 |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected の値を設定します。 |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner の値を設定します。 |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid の値を設定します。 |
| [setBCWP(double value)](#setBCWP-double-) | BCWP の値を設定します。 |
| [setBCWS(double value)](#setBCWS-double-) | BCWS の値を設定します。 |
| [setBookingType(int value)](#setBookingType-int-) | BookingType の値を設定します。 |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost の値を設定します。 |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork の値を設定します。 |
| [setCV(double value)](#setCV-double-) | CV の値を設定します。 |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Confirmed が設定されているかどうかを示す値を設定します。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost の値を設定します。 |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | CostRateTableType の値を設定します。 |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance の値を設定します。 |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created の値を設定します。 |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Delay の値を設定します。 |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | このオブジェクトの ExtendedAttributeCollection クラスのインスタンスを設定します。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish の値を設定します。 |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | FinishVariance の値を設定します。 |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | FixedMaterial が設定されているかどうかを示す値を設定します。 |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | HasFixedRateUnits が設定されているかどうかを示す値を設定します。 |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | この割り当ての一意の識別子を設定します。 |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Hyperlink の値を設定します。 |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | HyperlinkAddress の値を設定します。 |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | HyperlinkSubAddress の値を設定します。 |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | LevelingDelay の値を設定します。 |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | LinkedFields が設定されているかどうかを示す値を設定します。 |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | 可変材料消費を持つ材料リソースの割り当ての単位を設定します。 |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Milestone が設定されているかどうかを示す値を設定します。 |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | RTF 形式のテキストノートを設定します。 |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | RTF データから抽出されたノートのプレーンテキストを設定します。 |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Overallocated が設定されているかどうかを示す値を設定します。 |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost の値を設定します。 |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork の値を設定します。 |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits の値を設定します。 |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete の値を設定します。 |
| [setRateScale(int value)](#setRateScale-int-) | RateScale の値を設定します。 |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork の値を設定します。 |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost の値を設定します。 |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost の値を設定します。 |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork の値を設定します。 |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork の値を設定します。 |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | タスクに割り当てられたリソース。 |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | ResponsePending が設定されているかどうかを示す値を設定します。 |
| [setResume(Date value)](#setResume-java.util.Date-) | Resume の値を設定します。 |
| [setSV(double value)](#setSV-double-) | SV の値を設定します。 |
| [setStart(Date value)](#setStart-java.util.Date-) | Start の値を設定します。 |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | StartVariance の値を設定します。 |
| [setStop(Date value)](#setStop-java.util.Date-) | Stop の値を設定します。 |
| [setSummary(boolean value)](#setSummary-boolean-) | Summary が設定されているかどうかを示す値を設定します。 |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | リソースが割り当てられるタスク。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | このインスタンスを、要素 `TimephasedData` を含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスとして設定します（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)）。 |
| [setUid(int value)](#setUid-int-) | Uid の値を設定します。 |
| [setUnits(double value)](#setUnits-double-) | Units の値を設定します。 |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | UpdateNeeded が設定されているかどうかを示す値を設定します。 |
| [setVAC(double value)](#setVAC-double-) | VAC の値を設定します。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work の値を設定します。 |
| [setWorkContour(int value)](#setWorkContour-int-) | WorkContour の値を設定します。 |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | WorkVariance の値を設定します。 |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | タスクを2つの部分に分割します。 |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | タスクの期間と予定開始日に基づいて、時間フェーズデータのリストを生成します。 |
| [toString()](#toString--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスの短い文字列表現を返します。 |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


このコンテナ内でプロパティがマッピングされている値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティキーです。プロパティキーを取得するための [Asn](../../com.aspose.tasks/asn) 。 |

**Returns:**
T - このコンテナ内でプロパティがマッピングされる値です。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


このコンテナ内で指定されたプロパティを指定された値にマッピングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティキーです。プロパティキーを取得するための [Asn](../../com.aspose.tasks/asn) 。 |
| val | T | 値です。 |

### delete() {#delete--}
```
public final void delete()
```


プロジェクト割り当てコレクションからリソース割り当てを削除します。

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


このインスタンスが [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスの指定されたインスタンスと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | このインスタンスと比較するための、指定された [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスです。 |

**Returns:**
boolean - 指定された [ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスがこのインスタンスと同じ UID 値を持つ場合は **True**、それ以外の場合は **false**。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - o がこのインスタンスと同じリソースとタスクを割り当てる ResourceAssignment である場合は **True**、それ以外の場合は **false**。
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP の値を取得します。

**Returns:**
double - ACWP の値です。
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost の値を取得します。

**Returns:**
java.math.BigDecimal - ActualCost の値です。
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


ActualFinish の値を取得します。

**Returns:**
java.util.Date - ActualFinish の値です。
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - ActualOvertimeCost の値です。
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


ActualStart の値を取得します。

**Returns:**
java.util.Date - ActualStart の値です。
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner の値を取得します。

**Returns:**
java.lang.String - AssignmentOwner の値です。
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid の値を取得します。

**Returns:**
java.lang.String - AssignmentOwnerGuid の値です。
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP の値を取得します。

**Returns:**
double - BCWP の値。
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS の値を取得します。

**Returns:**
double - BCWS の値。
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


AssignmentBaselineCollection オブジェクトを取得します。割り当てに関連付けられたベースライン値のコレクションです。

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType の値を取得します。

**Returns:**
int - BookingType の値。
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost の値を取得します。

**Returns:**
java.math.BigDecimal - BudgetCost の値。
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV の値を取得します。

**Returns:**
double - CV の値。
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Confirmed が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - Confirmed が設定されているかどうかを示す値です。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost の値を取得します。

**Returns:**
java.math.BigDecimal - Cost の値。
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


CostRateTableType の値を取得します。

**Returns:**
int - CostRateTableType の値です。
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


CostVariance の値を取得します。

**Returns:**
double - CostVariance の値。
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Created の値を取得します。

**Returns:**
java.util.Date - Created の値。
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Delay の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


このオブジェクトの ExtendedAttributeCollection クラスのインスタンスを取得します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish の値を取得します。

**Returns:**
java.util.Date - Finish の値。
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


FinishVariance の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


FixedMaterial が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - FixedMaterial が設定されているかどうかを示す値です。
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


この割り当ての一意の識別子を取得します。

**Returns:**
java.util.UUID - この割り当ての一意の識別子です。
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hyperlink の値を取得します。

**Returns:**
java.lang.String - Hyperlink の値です。
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


HyperlinkAddress の値を取得します。

**Returns:**
java.lang.String - HyperlinkAddress の値です。
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


HyperlinkSubAddress の値を取得します。

**Returns:**
java.lang.String - HyperlinkSubAddress の値です。
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


内部使用のために予約されています。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


LevelingDelay の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


LinkedFields が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - LinkedFields が設定されているかどうかを示す値です。
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Milestone が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - Milestone が設定されているかどうかを示す値です。
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


RTF 形式のテキストノートを取得します。

--------------------

MPP 形式のみサポートされています。

**Returns:**
java.lang.String - RTF 形式のテキストノートです。
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


RTF データから抽出されたノートのプレーンテキストを取得します。

**Returns:**
java.lang.String - RTF データから抽出されたノートのプレーンテキストです。
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Overallocated が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - Overallocated が設定されているかどうかを示す値です。
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - OvertimeCost の値。
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


OvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


この割り当ての親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


PeakUnits の値を取得します。

**Returns:**
double - PeakUnits の値。
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


PercentWorkComplete の値を取得します。

**Returns:**
int - PercentWorkComplete の値。
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


RateScale の値を取得します。

**Returns:**
int - RateScale の値です。
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


RegularWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


RemainingCost の値を取得します。

**Returns:**
java.math.BigDecimal - RemainingCost の値。
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


RemainingOvertimeCost の値を取得します。

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost の値。
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


RemainingOvertimeWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


RemainingWork の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


タスクに割り当てられたリソース。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


ResponsePending が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - ResponsePending が設定されているかどうかを示す値です。
### getResume() {#getResume--}
```
public final Date getResume()
```


Resume の値を取得します。

**Returns:**
java.util.Date - Resume の値です。
### getSV() {#getSV--}
```
public final double getSV()
```


SV の値を取得します。

**Returns:**
double - SV の値。
### getStart() {#getStart--}
```
public final Date getStart()
```


Start の値を取得します。

**Returns:**
java.util.Date - Start の値。
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


StartVariance の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Stop の値を取得します。

**Returns:**
java.util.Date - Stop の値です。
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Summary が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - Summary が設定されているかどうかを示す値です。
### getTask() {#getTask--}
```
public final Task getTask()
```


リソースが割り当てられるタスク。

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


`TimephasedData` の要素を含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを取得します（`TimephasedData` の [getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) メソッド）。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


指定された開始日と終了日の [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) に対して、`TimephasedData` のインスタンスを含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトを返します（`TimephasedData` の [getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-) メソッド）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 時間分割データの開始日。 |
| 終了 | java.util.Date | 時間分割データの終了日。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


指定された [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) の開始日と終了日の範囲内で、`TimephasedData` のインスタンスを含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスを返します（`TimephasedData` の [getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-) メソッド）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 時間分割データの開始日。 |
| 終了 | java.util.Date | 時間分割データの終了日。 |
| timephasedType | byte | 時間分割データの種類（[TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)）。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


指定された日時間隔に対する時間別作業量を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 日時間隔の開始です。 |
| 終了 | java.util.Date | 日時間隔の終了です。 |

**Returns:**
double - 指定された日時間隔の時間別作業量です。
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


指定された日時間隔に対する時間別作業量を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 日時間隔の開始です。 |
| 終了 | java.util.Date | 日時間隔の終了です。 |
| timephasedDataType | バイト | 使用する時間別データのタイプです。 |

**Returns:**
double - 指定された日時間隔の時間別作業量です。
### getUid() {#getUid--}
```
public final int getUid()
```


Uid の値を取得します。

**Returns:**
int - Uid の値。
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Units の値を取得します。

**Returns:**
double - Units の値です。
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


UpdateNeeded が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - UpdateNeeded が設定されているかどうかを示す値です。
### getVAC() {#getVAC--}
```
public final double getVAC()
```


VAC の値を取得します。

**Returns:**
double - VAC の値です。
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


WorkContour の値を取得します。

**Returns:**
int - WorkContour の値です。
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


WorkVariance の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


このリソース割り当てに子があることを示す値を取得します。

**Returns:**
boolean - 常に false です。
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


HasFixedRateUnits が設定されているかどうかを示す値を取得します。

**Returns:**
boolean - HasFixedRateUnits が設定されているかどうかを示す値です。
### hashCode() {#hashCode--}
```
public int hashCode()
```


[ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスに対するハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


時間別データのリストを生成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 指定された開始日です。 |
| time | double | 指定された作業時間です。 |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 指定された作業カレンダーです。 |
| list | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | 時間別データのリストです。 |
| isWorking | boolean | 時間別データが作業中かどうかを示す指定されたフラグです。 |
| type | int | 指定された時間別データのタイプです。 |

**Returns:**
java.util.Date - リストが空の場合は、リストからの最大日付または開始日です。
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ACWP の値。 |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | ActualCost の値。 |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


ActualFinish の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ActualFinish の値。 |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | ActualOvertimeCost の値。 |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork の値。 |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected の値。 |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


ActualStart の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ActualStart の値。 |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork の値。 |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected の値。 |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | AssignmentOwner の値。 |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | AssignmentOwnerGuid の値。 |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | BCWP の値。 |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | BCWS の値。 |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | BookingType の値。 |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | BudgetCost の値。 |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork の値。 |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | CV の値。 |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Confirmed が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Confirmed が設定されているかどうかを示す値。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | Cost の値。 |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


CostRateTableType の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | CostRateTableType の値。 |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | CostVariance の値。 |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Created の値。 |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Delay の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Delay の値。 |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


このオブジェクトの ExtendedAttributeCollection クラスのインスタンスを設定します。

--------------------

XML フォーマットのみで読み取りがサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | このオブジェクトの ExtendedAttributeCollection クラスのインスタンス。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Finish の値。 |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


FinishVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | FinishVariance の値。 |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


FixedMaterial が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | FixedMaterial が設定されているかどうかを示す値。 |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


HasFixedRateUnits が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | HasFixedRateUnits が設定されているかどうかを示す値。 |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


この割り当ての一意の識別子を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.UUID | この割り当ての一意の識別子。 |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Hyperlink の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Hyperlink の値。 |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


HyperlinkAddress の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | HyperlinkAddress の値。 |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


HyperlinkSubAddress の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | HyperlinkSubAddress の値。 |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


LevelingDelay の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | LevelingDelay の値。 |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


LinkedFields が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | LinkedFields が設定されているかどうかを示す値。 |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


可変材料消費を伴う材料リソースの割り当ての単位を設定します。可変材料消費とは、割り当て期間が変わると、使用される材料の量が比例して変化することを意味します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 単位 | double | 期間中に蓄積された単位数。 |
|  | rateScaleType | int | 単位値が蓄積される期間。 |

--------------------

たとえば、'123/月' を設定するには、SetUnitsScaled(123D, RateScaleType.Month) を呼び出す必要があります。 |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Milestone が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Milestone が設定されているかどうかを示す値。 |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


RTF 形式のテキストノートを設定します。

--------------------

MPP 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | RTF 形式のテキストノート。 |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


RTF データから抽出されたノートのプレーンテキストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | RTF データから抽出されたノートのプレーンテキスト。 |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Overallocated が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Overallocated が設定されているかどうかを示す値。 |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | OvertimeCost の値。 |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork の値。 |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | PeakUnits の値。 |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | PercentWorkComplete の値。 |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


RateScale の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | RateScale の値。 |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork の値。 |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | RemainingCost の値。 |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | RemainingOvertimeCost の値。 |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork の値。 |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork の値。 |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


タスクに割り当てられたリソース。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | タスクに割り当てられたリソース。 |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


ResponsePending が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ResponsePending が設定されているかどうかを示す値。 |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Resume の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Resume の値。 |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | SV の値。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Start の値。 |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


StartVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | StartVariance の値。 |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Stop の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Stop の値。 |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Summary が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Summary が設定されているかどうかを示す値。 |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


リソースが割り当てられるタスク。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | リソースが割り当てられるタスク。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


このインスタンスを、要素 `TimephasedData` を含む [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスとして設定します（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスのインスタンスで、`TimephasedData` の要素を含む（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) クラス。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Uid の値。 |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Units の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | Units の値。 |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


UpdateNeeded が設定されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | UpdateNeeded が設定されているかどうかを示す値。 |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


VAC の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | VAC の値。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work の値。 |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


WorkContour の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | WorkContour の値。 |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


WorkVariance の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | WorkVariance の値。 |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


タスクを2つの部分に分割します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 分割の基準となる作業中断の開始時点。 |
| 終了 | java.util.Date | 分割の基準となる作業中断の終了時点。 |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 分割の基準となるカレンダー。 |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


タスクの期間と予定開始日に基づいて、時間フェーズデータのリストを生成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 時間フェーズデータを生成する元となるカレンダー。 |

### toString() {#toString--}
```
public String toString()
```


[ResourceAssignment](../../com.aspose.tasks/resourceassignment) クラスのインスタンスの短い文字列表現を返します。表現の正確な詳細は未定義で、変更される可能性があります。

**Returns:**
java.lang.String - 割り当てオブジェクトを表す短い文字列。
