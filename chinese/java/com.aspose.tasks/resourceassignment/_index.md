---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目中的资源分配。"
type: docs
weight: 249
url: /zh/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

表示项目中的资源分配。
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 返回此容器中属性映射的值。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 将指定属性映射到此容器中的指定值。 |
| [delete()](#delete--) | 从项目分配集合中删除资源分配。 |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | 返回一个值，指示此实例是否等于指定的 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getACWP()](#getACWP--) | 获取 ACWP 的值。 |
| [getActualCost()](#getActualCost--) | 获取 ActualCost 的值。 |
| [getActualFinish()](#getActualFinish--) | 获取 ActualFinish 的值。 |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | 获取 ActualOvertimeCost 的值。 |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | 获取 ActualOvertimeWork 的值。 |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | 获取 ActualOvertimeWorkProtected 的值。 |
| [getActualStart()](#getActualStart--) | 获取 ActualStart 的值。 |
| [getActualWork()](#getActualWork--) | 获取 ActualWork 的值。 |
| [getActualWorkProtected()](#getActualWorkProtected--) | 获取 ActualWorkProtected 的值。 |
| [getAssignmentOwner()](#getAssignmentOwner--) | 获取 AssignmentOwner 的值。 |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | 获取 AssignmentOwnerGuid 的值。 |
| [getBCWP()](#getBCWP--) | 获取 BCWP 的值。 |
| [getBCWS()](#getBCWS--) | 获取 BCWS 的值。 |
| [getBaselines()](#getBaselines--) | 获取 AssignmentBaselineCollection 对象。 |
| [getBookingType()](#getBookingType--) | 获取 BookingType 的值。 |
| [getBudgetCost()](#getBudgetCost--) | 获取 BudgetCost 的值。 |
| [getBudgetWork()](#getBudgetWork--) | 获取 BudgetWork 的值。 |
| [getCV()](#getCV--) | 获取 CV 的值。 |
| [getConfirmed()](#getConfirmed--) | 获取一个值，指示 Confirmed 是否已设置。 |
| [getCost()](#getCost--) | 获取 Cost 的值。 |
| [getCostRateTableType()](#getCostRateTableType--) | 获取 CostRateTableType 的值。 |
| [getCostVariance()](#getCostVariance--) | 获取 CostVariance 的值。 |
| [getCreated()](#getCreated--) | 获取 Created 的值。 |
| [getDelay()](#getDelay--) | 获取 Delay 的值。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | 获取此对象的 ExtendedAttributeCollection 类实例。 |
| [getFinish()](#getFinish--) | 获取 Finish 的值。 |
| [getFinishVariance()](#getFinishVariance--) | 获取 FinishVariance 的值。 |
| [getFixedMaterial()](#getFixedMaterial--) | 获取一个值，指示 FixedMaterial 是否已设置。 |
| [getGuid()](#getGuid--) | 获取此分配的唯一标识符。 |
| [getHyperlink()](#getHyperlink--) | 获取 Hyperlink 的值。 |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | 获取 HyperlinkAddress 的值。 |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | 获取 HyperlinkSubAddress 的值。 |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | 获取 LevelingDelay 的值。 |
| [getLinkedFields()](#getLinkedFields--) | 获取一个值，指示 LinkedFields 是否已设置。 |
| [getMilestone()](#getMilestone--) | 获取一个值，指示 Milestone 是否已设置。 |
| [getNotesRTF()](#getNotesRTF--) | 获取 RTF 格式的文本备注。 |
| [getNotesText()](#getNotesText--) | 获取从RTF数据中提取的笔记纯文本。 |
| [getOverallocated()](#getOverallocated--) | 获取指示是否已设置 Overallocated 的值。 |
| [getOvertimeCost()](#getOvertimeCost--) | 获取 OvertimeCost 的值。 |
| [getOvertimeWork()](#getOvertimeWork--) | 获取 OvertimeWork 的值。 |
| [getParentProject()](#getParentProject--) | 获取此分配的父项目。 |
| [getPeakUnits()](#getPeakUnits--) | 获取 PeakUnits 的值。 |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | 获取 PercentWorkComplete 的值。 |
| [getRateScale()](#getRateScale--) | 获取 RateScale 的值。 |
| [getRegularWork()](#getRegularWork--) | 获取 RegularWork 的值。 |
| [getRemainingCost()](#getRemainingCost--) | 获取 RemainingCost 的值。 |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | 获取 RemainingOvertimeCost 的值。 |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | 获取 RemainingOvertimeWork 的值。 |
| [getRemainingWork()](#getRemainingWork--) | 获取 RemainingWork 的值。 |
| [getResource()](#getResource--) | 分配给任务的资源。 |
| [getResponsePending()](#getResponsePending--) | 获取指示是否已设置 ResponsePending 的值。 |
| [getResume()](#getResume--) | 获取 Resume 的值。 |
| [getSV()](#getSV--) | 获取 SV 的值。 |
| [getStart()](#getStart--) | 获取 Start 的值。 |
| [getStartVariance()](#getStartVariance--) | 获取 StartVariance 的值。 |
| [getStop()](#getStop--) | 获取 Stop 的值。 |
| [getSummary()](#getSummary--) | 获取指示是否已设置 Summary 的值。 |
| [getTask()](#getTask--) | 资源被分配到的任务。 |
| [getTimephasedData()](#getTimephasedData--) | 获取 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例，包含 `TimephasedData`（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 类的元素。 |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | 返回在给定的开始和结束日期（对应 [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork)）内，包含 `TimephasedData`（[getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 实例的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象。 |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | 返回在给定的开始和结束日期内（针对指定的 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)），包含 `TimephasedData`（[getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 实例的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。 |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | 获取指定日期时间间隔的时间分段工作量。 |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | 获取指定日期时间间隔的时间分段工作量。 |
| [getUid()](#getUid--) | 获取 Uid 的值。 |
| [getUnits()](#getUnits--) | 获取 Units 的值。 |
| [getUpdateNeeded()](#getUpdateNeeded--) | 获取指示是否已设置 UpdateNeeded 的值。 |
| [getVAC()](#getVAC--) | 获取 VAC 的值。 |
| [getWork()](#getWork--) | 获取 Work 的值。 |
| [getWorkContour()](#getWorkContour--) | 获取 WorkContour 的值。 |
| [getWorkVariance()](#getWorkVariance--) | 获取 WorkVariance 的值。 |
| [hasChildren()](#hasChildren--) | 获取指示此资源分配是否有子项的值。 |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | 获取指示是否已设置 HasFixedRateUnits 的值。 |
| [hashCode()](#hashCode--) | 返回 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例的哈希码值。 |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | 生成时间分段数据的列表。 |
| [setACWP(double value)](#setACWP-double-) | 设置 ACWP 的值。 |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | 设置 ActualCost 的值。 |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | 设置 ActualFinish 的值。 |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | 设置 ActualOvertimeCost 的值。 |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | 设置 ActualOvertimeWork 的值。 |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | 设置 ActualOvertimeWorkProtected 的值。 |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | 设置 ActualStart 的值。 |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | 设置 ActualWork 的值。 |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | 设置 ActualWorkProtected 的值。 |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | 设置 AssignmentOwner 的值。 |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | 设置 AssignmentOwnerGuid 的值。 |
| [setBCWP(double value)](#setBCWP-double-) | 设置 BCWP 的值。 |
| [setBCWS(double value)](#setBCWS-double-) | 设置 BCWS 的值。 |
| [setBookingType(int value)](#setBookingType-int-) | 设置 BookingType 的值。 |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | 设置 BudgetCost 的值。 |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | 设置 BudgetWork 的值。 |
| [setCV(double value)](#setCV-double-) | 设置 CV 的值。 |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | 设置指示是否已设置 Confirmed 的值。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | 设置 Cost 的值。 |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | 设置 CostRateTableType 的值。 |
| [setCostVariance(double value)](#setCostVariance-double-) | 设置 CostVariance 的值。 |
| [setCreated(Date value)](#setCreated-java.util.Date-) | 设置 Created 的值。 |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | 设置 Delay 的值。 |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | 为此对象设置 ExtendedAttributeCollection 类的实例。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 设置 Finish 的值。 |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | 设置 FinishVariance 的值。 |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | 设置一个值，指示 FixedMaterial 是否已设置。 |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | 设置一个值，指示 HasFixedRateUnits 是否已设置。 |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | 为此分配设置唯一标识符。 |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | 设置 Hyperlink 的值。 |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | 设置 HyperlinkAddress 的值。 |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | 设置 HyperlinkSubAddress 的值。 |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | 设置 LevelingDelay 的值。 |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | 设置一个值，指示 LinkedFields 是否已设置。 |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | 为具有可变材料消耗的材料资源分配设置单位。 |
| [setMilestone(boolean value)](#setMilestone-boolean-) | 设置一个值，指示 Milestone 是否已设置。 |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | 以 RTF 格式设置文本备注。 |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | 设置从 RTF 数据中提取的备注纯文本。 |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | 设置一个值，指示 Overallocated 是否已设置。 |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | 设置 OvertimeCost 的值。 |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | 设置 OvertimeWork 的值。 |
| [setPeakUnits(double value)](#setPeakUnits-double-) | 设置 PeakUnits 的值。 |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | 设置 PercentWorkComplete 的值。 |
| [setRateScale(int value)](#setRateScale-int-) | 设置 RateScale 的值。 |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | 设置 RegularWork 的值。 |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | 设置 RemainingCost 的值。 |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | 设置 RemainingOvertimeCost 的值。 |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | 设置 RemainingOvertimeWork 的值。 |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | 设置 RemainingWork 的值。 |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | 分配给任务的资源。 |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | 设置一个值，指示 ResponsePending 是否已设置。 |
| [setResume(Date value)](#setResume-java.util.Date-) | 设置 Resume 的值。 |
| [setSV(double value)](#setSV-double-) | 设置 SV 的值。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 设置 Start 的值。 |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | 设置 StartVariance 的值。 |
| [setStop(Date value)](#setStop-java.util.Date-) | 设置 Stop 的值。 |
| [setSummary(boolean value)](#setSummary-boolean-) | 设置一个值，指示 Summary 是否已设置。 |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | 资源被分配到的任务。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 设置包含 `TimephasedData` 元素的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 类。 |
| [setUid(int value)](#setUid-int-) | 设置 Uid 的值。 |
| [setUnits(double value)](#setUnits-double-) | 设置 Units 的值。 |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | 设置一个值，指示 UpdateNeeded 是否已设置。 |
| [setVAC(double value)](#setVAC-double-) | 设置 VAC 的值。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | 设置 Work 的值。 |
| [setWorkContour(int value)](#setWorkContour-int-) | 设置 WorkContour 的值。 |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | 设置 WorkVariance 的值。 |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | 将任务拆分为两个部分。 |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | 根据任务持续时间和计划开始日期生成时间分段数据列表。 |
| [toString()](#toString--) | 返回 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例的简短字符串表示。 |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


返回此容器中属性映射的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。[Asn](../../com.aspose.tasks/asn) 用于获取属性键。 |

**Returns:**
T - 在此容器中映射到的属性值。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


将指定属性映射到此容器中的指定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。[Asn](../../com.aspose.tasks/asn) 用于获取属性键。 |
| val | T | 该值。 |

### delete() {#delete--}
```
public final void delete()
```


从项目分配集合中删除资源分配。

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


返回一个值，指示此实例是否等于指定的 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 指定的 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例，用于与此实例比较。 |

**Returns:**
布尔值 - 如果指定的 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例具有与此实例相同的 UID 值，则为 **True**；否则为 **false**。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
布尔值 - 如果 o 是一个将相同资源和任务分配给此实例的 ResourceAssignment，则为 **True**；否则为 **false**。
### getACWP() {#getACWP--}
```
public final double getACWP()
```


获取 ACWP 的值。

**Returns:**
double - ACWP 的值。
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


获取 ActualCost 的值。

**Returns:**
java.math.BigDecimal - ActualCost 的值。
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


获取 ActualFinish 的值。

**Returns:**
java.util.Date - ActualFinish 的值。
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


获取 ActualOvertimeCost 的值。

**Returns:**
java.math.BigDecimal - ActualOvertimeCost 的值。
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


获取 ActualOvertimeWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


获取 ActualOvertimeWorkProtected 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


获取 ActualStart 的值。

**Returns:**
java.util.Date - ActualStart 的值。
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


获取 ActualWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


获取 ActualWorkProtected 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


获取 AssignmentOwner 的值。

**Returns:**
java.lang.String - AssignmentOwner 的值。
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


获取 AssignmentOwnerGuid 的值。

**Returns:**
java.lang.String - AssignmentOwnerGuid 的值。
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


获取 BCWP 的值。

**Returns:**
double - BCWP 的值。
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


获取 BCWS 的值。

**Returns:**
double - BCWS 的值。
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


获取 AssignmentBaselineCollection 对象。与分配关联的基线值集合。

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


获取 BookingType 的值。

**Returns:**
int - BookingType 的值。
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


获取 BudgetCost 的值。

**Returns:**
java.math.BigDecimal - BudgetCost 的值。
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


获取 BudgetWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


获取 CV 的值。

**Returns:**
double - CV 的值。
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


获取一个值，指示 Confirmed 是否已设置。

**Returns:**
布尔值 - 表示 Confirmed 是否已设置的值。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


获取 Cost 的值。

**Returns:**
java.math.BigDecimal - Cost 的值。
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


获取 CostRateTableType 的值。

**Returns:**
int - CostRateTableType 的值。
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


获取 CostVariance 的值。

**Returns:**
double - CostVariance 的值。
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


获取 Created 的值。

**Returns:**
java.util.Date - Created 的值。
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


获取 Delay 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


获取此对象的 ExtendedAttributeCollection 类实例。

--------------------

仅支持读取 XML 格式。

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


获取 Finish 的值。

**Returns:**
java.util.Date - Finish 的值。
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


获取 FinishVariance 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


获取一个值，指示 FixedMaterial 是否已设置。

**Returns:**
布尔值 - 表示 FixedMaterial 是否已设置的值。
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


获取此分配的唯一标识符。

**Returns:**
java.util.UUID - 此分配的唯一标识符。
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


获取 Hyperlink 的值。

**Returns:**
java.lang.String - Hyperlink 的值。
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


获取 HyperlinkAddress 的值。

**Returns:**
java.lang.String - HyperlinkAddress 的值。
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


获取 HyperlinkSubAddress 的值。

**Returns:**
java.lang.String - HyperlinkSubAddress 的值。
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


保留供内部使用。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


获取 LevelingDelay 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


获取一个值，指示 LinkedFields 是否已设置。

**Returns:**
布尔值 - 表示 LinkedFields 是否已设置的值。
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


获取一个值，指示 Milestone 是否已设置。

**Returns:**
布尔值 - 表示 Milestone 是否已设置的值。
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


获取 RTF 格式的文本备注。

--------------------

仅支持 MPP 格式。

**Returns:**
java.lang.String - RTF 格式的文本备注。
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


获取从RTF数据中提取的笔记纯文本。

**Returns:**
java.lang.String - 从 RTF 数据中提取的备注纯文本。
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


获取指示是否已设置 Overallocated 的值。

**Returns:**
布尔值 - 表示 Overallocated 是否已设置的值。
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


获取 OvertimeCost 的值。

**Returns:**
java.math.BigDecimal - OvertimeCost 的一个值。
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


获取 OvertimeWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取此分配的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


获取 PeakUnits 的值。

**Returns:**
double - PeakUnits 的一个值。
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


获取 PercentWorkComplete 的值。

**Returns:**
int - PercentWorkComplete 的一个值。
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


获取 RateScale 的值。

**Returns:**
int - RateScale 的值。
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


获取 RegularWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


获取 RemainingCost 的值。

**Returns:**
java.math.BigDecimal - RemainingCost 的一个值。
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


获取 RemainingOvertimeCost 的值。

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost 的一个值。
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


获取 RemainingOvertimeWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


获取 RemainingWork 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


分配给任务的资源。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


获取指示是否已设置 ResponsePending 的值。

**Returns:**
布尔值 - 表示 ResponsePending 是否已设置的值。
### getResume() {#getResume--}
```
public final Date getResume()
```


获取 Resume 的值。

**Returns:**
java.util.Date - Resume 的值。
### getSV() {#getSV--}
```
public final double getSV()
```


获取 SV 的值。

**Returns:**
double - SV 的一个值。
### getStart() {#getStart--}
```
public final Date getStart()
```


获取 Start 的值。

**Returns:**
java.util.Date - Start 的一个值。
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


获取 StartVariance 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


获取 Stop 的值。

**Returns:**
java.util.Date - Stop 的值。
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


获取指示是否已设置 Summary 的值。

**Returns:**
boolean - 表示是否已设置 Summary 的值。
### getTask() {#getTask--}
```
public final Task getTask()
```


资源被分配到的任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


获取 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例，包含 `TimephasedData`（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 类的元素。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


返回在给定的开始和结束日期（对应 [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork)）内，包含 `TimephasedData`（[getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 实例的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 时间分段数据的开始日期。 |
| 结束 | java.util.Date | 时间分段数据的结束日期。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


返回在给定的开始和结束日期内（针对指定的 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)），包含 `TimephasedData`（[getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 实例的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 时间分段数据的开始日期。 |
| 结束 | java.util.Date | 时间分段数据的结束日期。 |
| timephasedType | byte | 时间分段数据的类型 ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype))。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


获取指定日期时间间隔的时间分段工作量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 日期时间间隔的开始。 |
| 结束 | java.util.Date | 日期时间间隔的结束。 |

**Returns:**
double - 指定日期时间间隔的时间分段工作量。
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


获取指定日期时间间隔的时间分段工作量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 日期时间间隔的开始。 |
| 结束 | java.util.Date | 日期时间间隔的结束。 |
| timephasedDataType | 字节 | 要使用的时间分段数据类型。 |

**Returns:**
double - 指定日期时间间隔的时间分段工作量。
### getUid() {#getUid--}
```
public final int getUid()
```


获取 Uid 的值。

**Returns:**
int - Uid 的值。
### getUnits() {#getUnits--}
```
public final double getUnits()
```


获取 Units 的值。

**Returns:**
double - Units 的值。
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


获取指示是否已设置 UpdateNeeded 的值。

**Returns:**
boolean - 表示是否已设置 UpdateNeeded 的值。
### getVAC() {#getVAC--}
```
public final double getVAC()
```


获取 VAC 的值。

**Returns:**
double - VAC 的值。
### getWork() {#getWork--}
```
public final Duration getWork()
```


获取 Work 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


获取 WorkContour 的值。

**Returns:**
int - WorkContour 的值。
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


获取 WorkVariance 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


获取指示此资源分配是否有子项的值。

**Returns:**
boolean - 始终为 false。
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


获取指示是否已设置 HasFixedRateUnits 的值。

**Returns:**
boolean - 表示是否已设置 HasFixedRateUnits 的值。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


生成时间分段数据的列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 指定的开始日期。 |
| time | double | 指定的工作时间。 |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 指定的工作日历。 |
| list | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | 时间分段数据的列表。 |
| isWorking | boolean | 指定的标志，用于指示时间分段数据是否工作。 |
| type | int | 指定的时间分段数据类型。 |

**Returns:**
java.util.Date - 列表中的最大日期，若列表为空则为开始日期。
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


设置 ACWP 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | ACWP 的值。 |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


设置 ActualCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | ActualCost 的值。 |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


设置 ActualFinish 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | ActualFinish 的值。 |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


设置 ActualOvertimeCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | ActualOvertimeCost 的值。 |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


设置 ActualOvertimeWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork 的值。 |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


设置 ActualOvertimeWorkProtected 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected 的值。 |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


设置 ActualStart 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | ActualStart 的值。 |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


设置 ActualWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork 的值。 |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


设置 ActualWorkProtected 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected 的值。 |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


设置 AssignmentOwner 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | AssignmentOwner 的值。 |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


设置 AssignmentOwnerGuid 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | AssignmentOwnerGuid 的值。 |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


设置 BCWP 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | BCWP 的一个值。 |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


设置 BCWS 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | BCWS 的一个值。 |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


设置 BookingType 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | BookingType 的一个值。 |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


设置 BudgetCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | BudgetCost 的一个值。 |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


设置 BudgetWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork 的一个值。 |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


设置 CV 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | CV 的一个值。 |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


设置指示是否已设置 Confirmed 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 Confirmed 是否已设置的值。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


设置 Cost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | Cost 的一个值。 |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


设置 CostRateTableType 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | CostRateTableType 的值。 |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


设置 CostVariance 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | CostVariance 的一个值。 |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


设置 Created 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Created 的一个值。 |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


设置 Delay 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Delay 的值。 |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


为此对象设置 ExtendedAttributeCollection 类的实例。

--------------------

仅支持读取 XML 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | 此对象的 ExtendedAttributeCollection 类的实例。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


设置 Finish 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Finish 的一个值。 |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


设置 FinishVariance 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | FinishVariance 的值。 |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


设置一个值，指示 FixedMaterial 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 FixedMaterial 是否已设置的值。 |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


设置一个值，指示 HasFixedRateUnits 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 HasFixedRateUnits 是否已设置的值。 |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


为此分配设置唯一标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID | 此分配的唯一标识符。 |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


设置 Hyperlink 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Hyperlink 的值。 |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


设置 HyperlinkAddress 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | HyperlinkAddress 的值。 |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


设置 HyperlinkSubAddress 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | HyperlinkSubAddress 的值。 |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


设置 LevelingDelay 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | LevelingDelay 的值。 |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


设置一个值，指示 LinkedFields 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 LinkedFields 是否已设置的值。 |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


为具有可变材料消耗的材料资源分配设置单位。可变材料消耗意味着随着分配持续时间的变化，使用的材料数量按比例变化。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 单位 | double | 在该时间段累计的单位数量。 |
|  | rateScaleType | int | 累计单位值的时间段。 |

--------------------

例如，要设置 '123/月'，应调用 SetUnitsScaled(123D, RateScaleType.Month)。 |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


设置一个值，指示 Milestone 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 Milestone 是否已设置的值。 |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


以 RTF 格式设置文本备注。

--------------------

仅支持 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | RTF 格式的文本备注。 |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


设置从 RTF 数据中提取的备注纯文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 从 RTF 数据中提取的 notes 的纯文本。 |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


设置一个值，指示 Overallocated 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否设置了 Overallocated 的值。 |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


设置 OvertimeCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | OvertimeCost 的值。 |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


设置 OvertimeWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork 的值。 |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


设置 PeakUnits 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | PeakUnits 的值。 |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


设置 PercentWorkComplete 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | PercentWorkComplete 的值。 |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


设置 RateScale 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | RateScale 的值。 |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


设置 RegularWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork 的值。 |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


设置 RemainingCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | RemainingCost 的值。 |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


设置 RemainingOvertimeCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | RemainingOvertimeCost 的值。 |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


设置 RemainingOvertimeWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork 的值。 |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


设置 RemainingWork 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork 的值。 |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


分配给任务的资源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | 分配给任务的资源。 |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


设置一个值，指示 ResponsePending 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否已设置 ResponsePending 的值。 |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


设置 Resume 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Resume 的值。 |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


设置 SV 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | SV 的值。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


设置 Start 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Start 的值。 |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


设置 StartVariance 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | StartVariance 的值。 |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


设置 Stop 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Stop 的值。 |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


设置一个值，指示 Summary 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否已设置 Summary 的值。 |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


资源被分配到的任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 资源被分配的任务。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


设置包含 `TimephasedData` 元素的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 类。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 包含 `TimephasedData` 元素的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例（[getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) 方法）。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


设置 Uid 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Uid 的值。 |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


设置 Units 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | Units 的值。 |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


设置一个值，指示 UpdateNeeded 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否已设置 UpdateNeeded 的值。 |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


设置 VAC 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | VAC 的值。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


设置 Work 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work 的值。 |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


设置 WorkContour 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | WorkContour 的值。 |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


设置 WorkVariance 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | WorkVariance 的值。 |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


将任务拆分为两个部分。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 用于拆分的工作中断的开始。 |
| 完成 | java.util.Date | 用于拆分的工作中断的结束。 |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 用于拆分的日历。 |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


根据任务持续时间和计划开始日期生成时间分段数据列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 用于生成时间分段数据的日历。 |

### toString() {#toString--}
```
public String toString()
```


返回 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 类实例的简短字符串表示。该表示的具体细节未指定，且可能会更改。

**Returns:**
java.lang.String - 表示分配对象的简短字符串。
