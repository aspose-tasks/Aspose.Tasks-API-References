---
title: "ResourceAssignment"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل تعيين مورد في مشروع."
type: docs
weight: 249
url: /ar/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

يمثل تعيين مورد في مشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [delete()](#delete--) | يحذف تعيين المورد من مجموعة تعيينات المشروع. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | يرجع قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لحالة محددة من فئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getACWP()](#getACWP--) | يحصل على قيمة ACWP. |
| [getActualCost()](#getActualCost--) | يحصل على قيمة ActualCost. |
| [getActualFinish()](#getActualFinish--) | يحصل على قيمة ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | يحصل على قيمة ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | يحصل على قيمة ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | يحصل على قيمة ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | يحصل على قيمة ActualStart. |
| [getActualWork()](#getActualWork--) | يحصل على قيمة ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | يحصل على قيمة ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | يحصل على قيمة AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | يحصل على قيمة AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | يحصل على قيمة BCWP. |
| [getBCWS()](#getBCWS--) | يحصل على قيمة BCWS. |
| [getBaselines()](#getBaselines--) | يحصل على كائن AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | يحصل على قيمة BookingType. |
| [getBudgetCost()](#getBudgetCost--) | يحصل على قيمة BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | يحصل على قيمة BudgetWork. |
| [getCV()](#getCV--) | يحصل على قيمة CV. |
| [getConfirmed()](#getConfirmed--) | يحصل على قيمة تشير إلى ما إذا كان Confirmed مضبوطًا أم لا. |
| [getCost()](#getCost--) | يحصل على قيمة Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | يحصل على قيمة CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | يحصل على قيمة CostVariance. |
| [getCreated()](#getCreated--) | يحصل على قيمة Created. |
| [getDelay()](#getDelay--) | يحصل على قيمة Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | يحصل على نسخة من فئة ExtendedAttributeCollection لهذا الكائن. |
| [getFinish()](#getFinish--) | يحصل على قيمة Finish. |
| [getFinishVariance()](#getFinishVariance--) | يحصل على قيمة FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | يحصل على قيمة تشير إلى ما إذا كان FixedMaterial مضبوطًا أم لا. |
| [getGuid()](#getGuid--) | يحصل على المعرف الفريد لهذا التعيين. |
| [getHyperlink()](#getHyperlink--) | يحصل على قيمة Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | يحصل على قيمة HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | يحصل على قيمة HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | يحصل على قيمة LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | يحصل على قيمة تشير إلى ما إذا كان LinkedFields مضبوطًا أم لا. |
| [getMilestone()](#getMilestone--) | يحصل على قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا. |
| [getNotesRTF()](#getNotesRTF--) | يحصل على ملاحظات النص بتنسيق RTF. |
| [getNotesText()](#getNotesText--) | يحصل على النص العادي للملاحظات المستخرج من بيانات RTF. |
| [getOverallocated()](#getOverallocated--) | يحصل على قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا. |
| [getOvertimeCost()](#getOvertimeCost--) | يحصل على قيمة OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | يحصل على قيمة OvertimeWork. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأصلي لهذا التعيين. |
| [getPeakUnits()](#getPeakUnits--) | يحصل على قيمة PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | يحصل على قيمة PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | يحصل على قيمة RateScale. |
| [getRegularWork()](#getRegularWork--) | يحصل على قيمة RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | يحصل على قيمة RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | يحصل على قيمة RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | يحصل على قيمة RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | يحصل على قيمة RemainingWork. |
| [getResource()](#getResource--) | المورد المعين لمهمة. |
| [getResponsePending()](#getResponsePending--) | يحصل على قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا. |
| [getResume()](#getResume--) | يحصل على قيمة Resume. |
| [getSV()](#getSV--) | يحصل على قيمة SV. |
| [getStart()](#getStart--) | يحصل على قيمة Start. |
| [getStartVariance()](#getStartVariance--) | يحصل على قيمة StartVariance. |
| [getStop()](#getStop--) | يحصل على قيمة Stop. |
| [getSummary()](#getSummary--) | يحصل على قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا. |
| [getTask()](#getTask--) | المهمة التي يُعين لها مورد. |
| [getTimephasedData()](#getTimephasedData--) | يحصل على نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على عناصر `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)). |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | يرجع كائن [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) مع نسخ `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) فئة ضمن تواريخ البداية والنهاية المحددة لـ [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | يرجع نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على نسخ `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) فئة ضمن تواريخ البداية والنهاية المحددة لـ [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | يحصل على مقدار العمل المتدرج الزمني للفترة الزمنية المحددة. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | يحصل على مقدار العمل المتدرج الزمني للفترة الزمنية المحددة. |
| [getUid()](#getUid--) | يحصل على قيمة Uid. |
| [getUnits()](#getUnits--) | يحصل على قيمة Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | يحصل على قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا. |
| [getVAC()](#getVAC--) | يحصل على قيمة VAC. |
| [getWork()](#getWork--) | يحصل على قيمة Work. |
| [getWorkContour()](#getWorkContour--) | يحصل على قيمة WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | يحصل على قيمة WorkVariance. |
| [hasChildren()](#hasChildren--) | يحصل على قيمة تشير إلى أن تعيين المورد هذا يحتوي على عناصر فرعية. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | يحصل على قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطًا أم لا. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز تجزئة (hash code) للنسخة من الفئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | ينشئ قائمة من البيانات المجدولة زمنياً. |
| [setACWP(double value)](#setACWP-double-) | يضبط قيمة ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | يضبط قيمة ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | يضبط قيمة ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | يضبط قيمة ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | يضبط قيمة ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | يضبط قيمة ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | يضبط قيمة ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | يضبط قيمة ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | يضبط قيمة AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | يضبط قيمة AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | يضبط قيمة BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | يضبط قيمة BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | يضبط قيمة للـ BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | يضبط قيمة للـ BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | يضبط قيمة للـ BudgetWork. |
| [setCV(double value)](#setCV-double-) | يضبط قيمة للـ CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | يضبط قيمة تشير إلى ما إذا كان Confirmed مضبوطًا أم لا. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | يضبط قيمة للـ Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | يضبط قيمة CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | يضبط قيمة للـ CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | يضبط قيمة للـ Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | يضبط قيمة Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | يضبط نسخة من الفئة ExtendedAttributeCollection لهذا الكائن. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | يضبط قيمة للـ Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | يضبط قيمة FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | يضبط قيمة تشير إلى ما إذا كان FixedMaterial مضبوطًا أم لا. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | يضبط قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطًا أم لا. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | يضبط المعرف الفريد لهذا التعيين. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | يضبط قيمة Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | يضبط قيمة HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | يضبط قيمة HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | يضبط قيمة LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | يضبط قيمة تشير إلى ما إذا كان LinkedFields مضبوطًا أم لا. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | يضبط الوحدات لتعيين مورد مادي مع استهلاك مادي متغير. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | يضبط قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | يضبط ملاحظات النص بتنسيق RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | يضبط النص العادي للملاحظات المستخرج من بيانات RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | يضبط قيمة تشير إلى ما إذا كان Overallocated مُعَيَّنًا أم لا. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | يضبط قيمة OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | يضبط قيمة PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | يضبط قيمة PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | يضبط قيمة RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | يضبط قيمة RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | يضبط قيمة RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | يضبط قيمة RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | يضبط قيمة RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | المورد المعين لمهمة. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | يضبط قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا. |
| [setResume(Date value)](#setResume-java.util.Date-) | يضبط قيمة Resume. |
| [setSV(double value)](#setSV-double-) | يضبط قيمة SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | يضبط قيمة Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | يضبط قيمة StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | يضبط قيمة Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | يضبط قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | المهمة التي يُعين لها مورد. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | يضبط نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على عناصر `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)). |
| [setUid(int value)](#setUid-int-) | يحدد قيمة للـ Uid. |
| [setUnits(double value)](#setUnits-double-) | يضبط قيمة Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | يضبط قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا. |
| [setVAC(double value)](#setVAC-double-) | يضبط قيمة VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | يحدد قيمة للـ Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | يضبط قيمة WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | يحدد قيمة للـ WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | يقسم المهمة إلى جزأين. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | ينشئ قائمة من البيانات الزمنية المرحلية بناءً على مدة المهمة وتاريخ البدء المجدول. |
| [toString()](#toString--) | يعيد تمثيل نصي قصير لنسخة من فئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Asn](../../com.aspose.tasks/asn) للحصول على مفتاح الخاصية. |

**Returns:**
T - القيمة التي تُعيَّن لها الخاصية في هذه الحاوية.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Asn](../../com.aspose.tasks/asn) للحصول على مفتاح الخاصية. |
| القيمة | T | القيمة. |

### delete() {#delete--}
```
public final void delete()
```


يحذف تعيين المورد من مجموعة تعيينات المشروع.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


يرجع قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لحالة محددة من فئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | النسخة المحددة من فئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment) للمقارنة مع هذه النسخة. |

**Returns:**
منطقي - **True** إذا كانت النسخة المحددة من فئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment) لديها نفس قيمة UID مثل هذه النسخة؛ وإلا، **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن للمقارنة مع هذا المثيل. |

**Returns:**
منطقي - **True** إذا كان o هو ResourceAssignment يعيّن نفس المورد والمهمة مثل هذه النسخة؛ وإلا، **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


يحصل على قيمة ACWP.

**Returns:**
مزدوج - قيمة لـ ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


يحصل على قيمة ActualCost.

**Returns:**
java.math.BigDecimal - قيمة لـ ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


يحصل على قيمة ActualFinish.

**Returns:**
java.util.Date - قيمة ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


يحصل على قيمة ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - قيمة لـ ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


يحصل على قيمة ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


يحصل على قيمة ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


يحصل على قيمة ActualStart.

**Returns:**
java.util.Date - قيمة ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


يحصل على قيمة ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


يحصل على قيمة ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


يحصل على قيمة AssignmentOwner.

**Returns:**
java.lang.String - قيمة لـ AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


يحصل على قيمة AssignmentOwnerGuid.

**Returns:**
java.lang.String - قيمة لـ AssignmentOwnerGuid.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


يحصل على قيمة BCWP.

**Returns:**
double - قيمة لـ BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


يحصل على قيمة BCWS.

**Returns:**
double - قيمة لـ BCWS.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


يحصل على كائن AssignmentBaselineCollection. مجموعة قيم الخط الأساسي المرتبطة بتعيين.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


يحصل على قيمة BookingType.

**Returns:**
int - قيمة لـ BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


يحصل على قيمة BudgetCost.

**Returns:**
java.math.BigDecimal - قيمة لـ BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


يحصل على قيمة BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


يحصل على قيمة CV.

**Returns:**
double - قيمة لـ CV.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


يحصل على قيمة تشير إلى ما إذا كان Confirmed مضبوطًا أم لا.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان Confirmed مضبوطًا أم لا.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


يحصل على قيمة Cost.

**Returns:**
java.math.BigDecimal - قيمة لـ Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


يحصل على قيمة CostRateTableType.

**Returns:**
int - قيمة CostRateTableType.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


يحصل على قيمة CostVariance.

**Returns:**
double - قيمة لـ CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


يحصل على قيمة Created.

**Returns:**
java.util.Date - قيمة لـ Created.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


يحصل على قيمة Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


يحصل على نسخة من فئة ExtendedAttributeCollection لهذا الكائن.

--------------------

القراءة مدعومة لتنسيق XML فقط.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


يحصل على قيمة Finish.

**Returns:**
java.util.Date - قيمة لـ Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


يحصل على قيمة FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


يحصل على قيمة تشير إلى ما إذا كان FixedMaterial مضبوطًا أم لا.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان FixedMaterial مضبوطًا أم لا.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


يحصل على المعرف الفريد لهذا التعيين.

**Returns:**
java.util.UUID - معرف فريد لهذا التعيين.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


يحصل على قيمة Hyperlink.

**Returns:**
java.lang.String - قيمة Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


يحصل على قيمة HyperlinkAddress.

**Returns:**
java.lang.String - قيمة HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


يحصل على قيمة HyperlinkSubAddress.

**Returns:**
java.lang.String - قيمة لـ HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


محجوز للاستخدام الداخلي.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


يحصل على قيمة LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


يحصل على قيمة تشير إلى ما إذا كان LinkedFields مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان LinkedFields مضبوطًا أم لا.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


يحصل على قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


يحصل على ملاحظات النص بتنسيق RTF.

--------------------

مدعوم لتنسيقات MPP فقط.

**Returns:**
java.lang.String - ملاحظات النص بتنسيق RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


يحصل على النص العادي للملاحظات المستخرج من بيانات RTF.

**Returns:**
java.lang.String - النص العادي للملاحظات المستخرج من بيانات RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


يحصل على قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


يحصل على قيمة OvertimeCost.

**Returns:**
java.math.BigDecimal - قيمة لـ OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


يحصل على قيمة OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


يحصل على المشروع الأصلي لهذا التعيين.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


يحصل على قيمة PeakUnits.

**Returns:**
double - قيمة لـ PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


يحصل على قيمة PercentWorkComplete.

**Returns:**
int - قيمة لـ PercentWorkComplete.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


يحصل على قيمة RateScale.

**Returns:**
int - قيمة لـ RateScale.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


يحصل على قيمة RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


يحصل على قيمة RemainingCost.

**Returns:**
java.math.BigDecimal - قيمة لـ RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


يحصل على قيمة RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - قيمة لـ RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


يحصل على قيمة RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


يحصل على قيمة RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


المورد المعين لمهمة.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


يحصل على قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا.
### getResume() {#getResume--}
```
public final Date getResume()
```


يحصل على قيمة Resume.

**Returns:**
java.util.Date - قيمة لـ Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


يحصل على قيمة SV.

**Returns:**
double - قيمة لـ SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


يحصل على قيمة Start.

**Returns:**
java.util.Date - قيمة لـ Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


يحصل على قيمة StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


يحصل على قيمة Stop.

**Returns:**
java.util.Date - قيمة لـ Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


يحصل على قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا.
### getTask() {#getTask--}
```
public final Task getTask()
```


المهمة التي يُعين لها مورد.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


يحصل على نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على عناصر `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)).

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


يرجع كائن [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) مع نسخ `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) فئة ضمن تواريخ البداية والنهاية المحددة لـ [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للبيانات الزمنية المرحلية. |
| نهاية | java.util.Date | تاريخ الانتهاء للبيانات الزمنية المرحلية. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


يرجع نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على نسخ `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) فئة ضمن تواريخ البداية والنهاية المحددة لـ [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للبيانات الزمنية المرحلية. |
| نهاية | java.util.Date | تاريخ الانتهاء للبيانات الزمنية المرحلية. |
| timephasedType | byte | نوع البيانات الزمنية المرحلية ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


يحصل على مقدار العمل المتدرج الزمني للفترة الزمنية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | بداية الفاصل الزمني للتاريخ والوقت. |
| نهاية | java.util.Date | نهاية الفاصل الزمني للتاريخ والوقت. |

**Returns:**
double - مقدار العمل المتدرج زمنياً للفاصل الزمني المحدد.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


يحصل على مقدار العمل المتدرج الزمني للفترة الزمنية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | بداية الفاصل الزمني للتاريخ والوقت. |
| نهاية | java.util.Date | نهاية الفاصل الزمني للتاريخ والوقت. |
| timephasedDataType | byte | نوع البيانات المتدرجة زمنياً للاستخدام. |

**Returns:**
double - مقدار العمل المتدرج زمنياً للفاصل الزمني المحدد.
### getUid() {#getUid--}
```
public final int getUid()
```


يحصل على قيمة Uid.

**Returns:**
int - قيمة من Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


يحصل على قيمة Units.

**Returns:**
double - قيمة لـ Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


يحصل على قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


يحصل على قيمة VAC.

**Returns:**
double - قيمة لـ VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


يحصل على قيمة Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


يحصل على قيمة WorkContour.

**Returns:**
int - قيمة لـ WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


يحصل على قيمة WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


يحصل على قيمة تشير إلى أن تعيين المورد هذا يحتوي على عناصر فرعية.

**Returns:**
boolean - دائمًا خاطئ.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


يحصل على قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطًا أم لا.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز تجزئة (hash code) للنسخة من الفئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


ينشئ قائمة من البيانات المجدولة زمنياً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء المحدد. |
| time | double | وقت العمل المحدد. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | تقويم العمل المحدد. |
| قائمة | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | قائمة البيانات المتدرجة زمنياً. |
| isWorking | منطقي | العلم المحدد الذي يحدد ما إذا كانت البيانات المتدرجة زمنياً تعمل أم لا. |
| type | int | نوع البيانات المتدرجة زمنياً المحدد. |

**Returns:**
java.util.Date - تاريخ أقصى من القائمة أو تاريخ البدء إذا كانت القائمة فارغة.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


يضبط قيمة ACWP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


يضبط قيمة ActualCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


يضبط قيمة ActualFinish.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


يضبط قيمة ActualOvertimeCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


يضبط قيمة ActualOvertimeWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


يضبط قيمة ActualOvertimeWorkProtected.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


يضبط قيمة ActualStart.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


يضبط قيمة ActualWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


يضبط قيمة ActualWorkProtected.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


يضبط قيمة AssignmentOwner.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


يضبط قيمة AssignmentOwnerGuid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من AssignmentOwnerGuid. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


يضبط قيمة BCWP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


يضبط قيمة BCWS.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


يضبط قيمة للـ BookingType.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة من BookingType. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


يضبط قيمة للـ BudgetCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


يضبط قيمة للـ BudgetWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


يضبط قيمة للـ CV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من CV. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان Confirmed مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان Confirmed مضبوطاً أم لا. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


يضبط قيمة للـ Cost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


يضبط قيمة CostRateTableType.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة CostRateTableType. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


يضبط قيمة للـ CostVariance.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


يضبط قيمة للـ Created.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من Created. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


يضبط قيمة Delay.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


يضبط نسخة من الفئة ExtendedAttributeCollection لهذا الكائن.

--------------------

القراءة مدعومة لتنسيق XML فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | مثال من الفئة ExtendedAttributeCollection لهذا الكائن. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


يضبط قيمة للـ Finish.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


يضبط قيمة FinishVariance.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان FixedMaterial مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان FixedMaterial مضبوطاً أم لا. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان HasFixedRateUnits مضبوطاً أم لا. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


يضبط المعرف الفريد لهذا التعيين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID | معرّف فريد لهذا التكليف. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


يضبط قيمة Hyperlink.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


يضبط قيمة HyperlinkAddress.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


يضبط قيمة HyperlinkSubAddress.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


يضبط قيمة LevelingDelay.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان LinkedFields مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان LinkedFields مضبوطاً أم لا. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


يضبط الوحدات لتكليف مورد مادي باستهلاك مادي متغيّر. يعني الاستهلاك المادي المتغيّر أنه كلما تغيرت مدة التكليف، تتغير كمية المواد المستخدمة بصورة متناسبة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوحدات | double | عدد الوحدات المتراكمة خلال الفترة الزمنية. |
|  | rateScaleType | int | الفترة الزمنية التي يتم فيها تراكم قيمة الوحدة. |

--------------------

على سبيل المثال، لتعيين '123/شهر'، يجب استدعاء SetUnitsScaled(123D, RateScaleType.Month). |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان Milestone مضبوطًا أم لا. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


يضبط ملاحظات النص بتنسيق RTF.

--------------------

مدعوم لتنسيقات MPP فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | ملاحظات النص بتنسيق RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


يضبط النص العادي للملاحظات المستخرج من بيانات RTF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | النص العادي للملاحظات المستخرج من بيانات RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان Overallocated مُعَيَّنًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


يضبط قيمة OvertimeCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


يضبط قيمة OvertimeWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


يضبط قيمة PeakUnits.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


يضبط قيمة PercentWorkComplete.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة PercentWorkComplete. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


يضبط قيمة RateScale.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة من RateScale. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


يضبط قيمة RegularWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


يضبط قيمة RemainingCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


يضبط قيمة RemainingOvertimeCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


يضبط قيمة RemainingOvertimeWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


يضبط قيمة RemainingWork.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة RemainingWork. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


المورد المعين لمهمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | المورد المعين لمهمة. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان ResponsePending مضبوطًا أم لا. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


يضبط قيمة Resume.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


يضبط قيمة SV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


يضبط قيمة Start.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة لـ Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


يضبط قيمة StartVariance.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة من StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


يضبط قيمة Stop.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان Summary مضبوطًا أم لا. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


المهمة التي يُعين لها مورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | المهمة التي يُعيّن لها المورد. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


يضبط نسخة من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على عناصر `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | مثال على نسخة من الفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) التي تحتوي على عناصر `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


يحدد قيمة للـ Uid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة لـ Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


يضبط قيمة Units.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان UpdateNeeded مضبوطًا أم لا. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


يضبط قيمة VAC.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


يحدد قيمة للـ Work.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة لـ Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


يضبط قيمة WorkContour.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة من WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


يحدد قيمة للـ WorkVariance.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة لـ WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


يقسم المهمة إلى جزأين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | بداية انقطاع العمل الذي يُقسم بناءً عليه. |
| الانتهاء | java.util.Date | نهاية انقطاع العمل الذي يُقسم بناءً عليه. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | التقويم الذي يُقسم بناءً عليه. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


ينشئ قائمة من البيانات الزمنية المرحلية بناءً على مدة المهمة وتاريخ البدء المجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | التقويم الذي يُستخدم لإنشاء بيانات زمنية مجزأة منه. |

### toString() {#toString--}
```
public String toString()
```


يعيد تمثيلًا نصيًا قصيرًا لنسخة من الفئة [ResourceAssignment](../../com.aspose.tasks/resourceassignment). التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير.

**Returns:**
java.lang.String - نص قصير يمثل كائن التعيين.
