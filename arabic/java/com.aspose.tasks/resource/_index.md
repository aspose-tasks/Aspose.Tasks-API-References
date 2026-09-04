---
title: "Resource"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل موردًا في مشروع."
type: docs
weight: 248
url: /ar/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

يمثل موردًا في مشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [canLevel()](#canLevel--) | يحصل على قيمة تشير إلى ما إذا كان CanLevel مضبوطًا أم لا. |
| [delete()](#delete--) | يحذف موردًا وتعييناته من المشروع. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | يعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لمثيلة محددة من فئة [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [getACWP()](#getACWP--) | يحصل على قيمة ACWP. |
| [getAccrueAt()](#getAccrueAt--) | يحصل على قيمة AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | يحصل على قيمة ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | يحصل على قيمة ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | يحصل على قيمة ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | يحصل على قيمة ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | يحصل على قيمة ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | يحصل على قيمة ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | يحصل على قيمة ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | يحصل على قيمة AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | يحصل على قيمة AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | يحصل على مجموعة من تعيينات الموارد لهذا الكائن. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | يحصل على المثيل من فئة [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | يحصل على قيمة AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | يحصل على قيمة AvailableTo. |
| [getBCWP()](#getBCWP--) | يحصل على قيمة BCWP. |
| [getBCWS()](#getBCWS--) | يحصل على قيمة BCWS. |
| [getBaselines()](#getBaselines--) | يحصل على مثيل BaselineCollection لهذا الكائن. |
| [getBookingType()](#getBookingType--) | يحصل على قيمة BookingType. |
| [getBudgetCost()](#getBudgetCost--) | يحصل على قيمة BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | يحصل على قيمة BudgetWork. |
| [getCV()](#getCV--) | يحصل على قيمة CV. |
| [getCalendar()](#getCalendar--) | يحصل على قيمة Calendar. |
| [getCode()](#getCode--) | يحصل على قيمة Code. |
| [getCost()](#getCost--) | يحصل على قيمة Cost. |
| [getCostCenter()](#getCostCenter--) | يحصل على قيمة CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | يحصل على قيمة CostPerUse. |
| [getCostVariance()](#getCostVariance--) | يحصل على قيمة CostVariance. |
| [getCreated()](#getCreated--) | يحصل على قيمة Created. |
| [getEMailAddress()](#getEMailAddress--) | يحصل على قيمة EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | يحصل على قيم سمة موسعة. |
| [getFinish()](#getFinish--) | يحصل على قيمة Finish. |
| [getGroup()](#getGroup--) | يحصل على قيمة Group. |
| [getGuid()](#getGuid--) | يحصل على قيمة Guid. |
| [getHyperlink()](#getHyperlink--) | يحصل على العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | يحصل على العنوان لرابط تشعبي مرتبط بمورد. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | يحصل على الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمورد. |
| [getId()](#getId--) | يحصل على قيمة Id. |
| [getInactive()](#getInactive--) | يحصل على قيمة تشير إلى ما إذا كان Inactive مضبوطًا أم لا. |
| [getInitials()](#getInitials--) | يحصل على قيمة Initials. |
| [getItems()](#getItems--) | يحصل على الموارد الفرعية. |
| [getMaterialLabel()](#getMaterialLabel--) | يحصل على قيمة MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | يحصل على قيمة MaxUnits. |
| [getName()](#getName--) | يحصل على قيمة Name. |
| [getNotesRTF()](#getNotesRTF--) | يحصل على قيمة NotesRTF. |
| [getNotesText()](#getNotesText--) | يحصل على قيمة NotesText. |
| [getOutlineCode()](#getOutlineCode--) | يحصل على كائن OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | يحصل على قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا. |
| [getOvertimeCost()](#getOvertimeCost--) | يحصل على قيمة OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | يحصل على قيمة OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | يحصل على قيمة OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | يحصل على قيمة OvertimeWork. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأصل لهذه الحاوية. |
| [getPeakUnits()](#getPeakUnits--) | يحصل على قيمة PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | يحصل على قيمة PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | يحصل على قيمة Phonetics. |
| [getRates()](#getRates--) | يحصل على نسخة من الفئة [RateCollection](../../com.aspose.tasks/ratecollection) لهذا الكائن. |
| [getRegularWork()](#getRegularWork--) | يحصل على قيمة RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | يحصل على قيمة RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | يحصل على قيمة RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | يحصل على قيمة RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | يحصل على قيمة RemainingWork. |
| [getSV()](#getSV--) | يحصل على قيمة SV. |
| [getStandardRate()](#getStandardRate--) | يحصل على قيمة StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | يحصل على قيمة StandardRateFormat. |
| [getStart()](#getStart--) | يحصل على قيمة Start. |
| [getTimephasedData()](#getTimephasedData--) | يحصل على نسخة من الفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | يعيد [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن مع `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) القيم ضمن تواريخ البداية والنهاية المعطاة. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | يعيد نسخة من الفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن مع `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) القيم ضمن تواريخ البداية والنهاية المعطاة لنوع [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | يحصل على قيمة Type. |
| [getUid()](#getUid--) | يحصل على قيمة Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | يحصل على قيمة WindowsUserAccount. |
| [getWork()](#getWork--) | يحصل على قيمة Work. |
| [getWorkVariance()](#getWorkVariance--) | يحصل على قيمة WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | يحصل على قيمة Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | يرجع قيمة رمز تجزئة للنسخة من الفئة [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | يحصل على قيمة تشير إلى ما إذا كان IsBudget مضبوطًا أم لا. |
| [isCostResource()](#isCostResource--) | يحصل على قيمة تشير إلى ما إذا كان IsCostResource مضبوطًا أم لا. |
| [isEnterprise()](#isEnterprise--) | يحصل على قيمة تشير إلى ما إذا كان IsEnterprise مضبوطًا أم لا. |
| [isGeneric()](#isGeneric--) | يحصل على قيمة تشير إلى ما إذا كان IsGeneric مضبوطًا أم لا. |
| [isNull()](#isNull--) | يحصل على قيمة تشير إلى ما إذا كان IsNull مضبوطًا أم لا. |
| [isRoot()](#isRoot--) | يحصل على العلامة التي تشير إلى ما إذا كان المورد موردًا جذريًا. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | يحصل على قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مضبوطًا أم لا. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [setACWP(double value)](#setACWP-double-) | يضبط قيمة ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | يضبط قيمة AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | يضبط قيمة ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | يضبط قيمة ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | يضبط قيمة ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | يضبط قيمة ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | يضبط قيمة ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | يضبط قيمة ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | يضبط قيمة AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | يضبط قيمة AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | يضبط قيمة AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | يضبط قيمة AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | يضبط قيمة BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | يضبط قيمة BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | يضبط قيمة للـ BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان IsBudget مضبوطًا أم لا. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | يضبط قيمة للـ BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | يضبط قيمة للـ BudgetWork. |
| [setCV(double value)](#setCV-double-) | يضبط قيمة للـ CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | يضبط قيمة للـ Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان CanLevel مضبوطًا أم لا. |
| [setCode(String value)](#setCode-java.lang.String-) | يضبط قيمة للـ Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | يضبط قيمة للـ Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | يضبط قيمة للـ CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | يضبط قيمة للـ CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان IsCostResource مضبوطًا أم لا. |
| [setCostVariance(double value)](#setCostVariance-double-) | يضبط قيمة للـ CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | يضبط قيمة للـ Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | يضبط قيمة للـ EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان IsEnterprise مضبوطًا أم لا. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | يضبط قيمة للـ Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان IsGeneric مضبوطًا أم لا. |
| [setGroup(String value)](#setGroup-java.lang.String-) | يضبط قيمة للـ Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | يضبط قيمة للـ Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | يضبط العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | يضبط العنوان لرابط تشعبي مرتبط بمورد. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | يضبط الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمورد. |
| [setId(int value)](#setId-int-) | يضبط قيمة للـ Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان Inactive مضبوطًا أم لا. |
| [setInitials(String value)](#setInitials-java.lang.String-) | يضبط قيمة Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | يضبط قيمة MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | يضبط قيمة MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | يضبط قيمة Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | يضبط قيمة NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | يضبط قيمة NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان IsNull مُعَيَّنًا أم لا. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | يضبط قيمة تشير إلى ما إذا كان Overallocated مُعَيَّنًا أم لا. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | يضبط قيمة OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | يضبط قيمة OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | يضبط قيمة OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | يضبط قيمة PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | يضبط قيمة PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | يضبط قيمة Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | يضبط قيمة RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | يضبط قيمة RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | يضبط قيمة RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | يضبط قيمة RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | يضبط قيمة RemainingWork. |
| [setSV(double value)](#setSV-double-) | يضبط قيمة SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | يضبط قيمة StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | يضبط قيمة StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | يضبط قيمة Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | يضبط قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مُعَيَّنًا أم لا. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | يحدد مثيلاً لفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |
| [setType(int value)](#setType-int-) | يحدد قيمة للنوع. |
| [setUid(int value)](#setUid-int-) | يحدد قيمة للـ Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | يحدد قيمة لـ WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | يحدد قيمة للـ Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | يحدد قيمة للـ WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | يحدد قيمة للـ Workgroup. |
| [toString()](#toString--) | يرجع تمثيلًا نصيًا قصيرًا لمثيل فئة [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Rsc](../../com.aspose.tasks/rsc) للحصول على مفتاح الخاصية. |

**Returns:**
T - القيمة التي تُعيَّن لها الخاصية في هذه الحاوية.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Rsc](../../com.aspose.tasks/rsc) للحصول على مفتاح الخاصية. |
| القيمة | T | القيمة. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


يحصل على قيمة تشير إلى ما إذا كان CanLevel مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


يحذف موردًا وتعييناته من المشروع.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


يعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لمثيلة محددة من فئة [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | المثيل المحدد لفئة [Resource](../../com.aspose.tasks/resource) للمقارنة مع هذا المثيل. |

**Returns:**
منطقي - **True** إذا كان المثيل المحدد لفئة [Resource](../../com.aspose.tasks/resource) يحتوي على نفس قيمة Uid لهذا المثيل؛ وإلا، **false**.
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
منطقي - **True** إذا كان الكائن المحدد هو Resource يحتوي على نفس قيمة Uid لهذا المثيل؛ وإلا، **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


يحصل على قيمة ACWP.

**Returns:**
مزدوج - قيمة لـ ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


يحصل على قيمة AccrueAt.

**Returns:**
عدد صحيح - قيمة لـ AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


يحصل على قيمة ActiveDirectoryGuid.

**Returns:**
java.lang.String - قيمة لـ ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


يحصل على قيمة ActualCost.

**Returns:**
java.math.BigDecimal - قيمة لـ ActualCost.
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


يحصل على مجموعة من تعيينات الموارد لهذا الكائن.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


يحصل على مثيل فئة [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). مجموعة الفترات التي يكون فيها المورد متاحًا.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


يحصل على قيمة AvailableFrom.

**Returns:**
java.util.Date - قيمة لـ AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


يحصل على قيمة AvailableTo.

**Returns:**
java.util.Date - قيمة لـ AvailableTo.
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
public final BaselineCollection getBaselines()
```


يحصل على مثيل BaselineCollection لهذا الكائن. قيم الخط الأساسي للموارد.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


يحصل على قيمة Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


يحصل على قيمة Code.

**Returns:**
java.lang.String - قيمة لـ Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


يحصل على قيمة Cost.

**Returns:**
java.math.BigDecimal - قيمة لـ Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


يحصل على قيمة CostCenter.

**Returns:**
java.lang.String - قيمة لـ CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


يحصل على قيمة CostPerUse.

**Returns:**
java.math.BigDecimal - قيمة لـ CostPerUse.
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


يحصل على قيمة EMailAddress.

**Returns:**
java.lang.String - قيمة لـ EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


يحصل على قيم سمة موسعة.

--------------------

هناك قطعتان من البيانات ضروريان - مؤشر يعود إلى جدول السمة الموسعة الذي يُحدَّد إما بالمعرف الفريد أو معرف الحقل، والقيمة التي تُحدَّد إما بالقيمة نفسها أو بمؤشر يعود إلى قائمة القيم.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


يحصل على قيمة Finish.

**Returns:**
java.util.Date - قيمة لـ Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


يحصل على قيمة Group.

**Returns:**
java.lang.String - قيمة لـ Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


يحصل على قيمة Guid.

**Returns:**
java.lang.String - قيمة لـ Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


يحصل على العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد.

**Returns:**
java.lang.String - العنوان أو النص التوضيحي للارتباط التشعبي المرتبط بموارد.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


يحصل على العنوان لرابط تشعبي مرتبط بمورد.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

**Returns:**
java.lang.String - العنوان للارتباط التشعبي المرتبط بموارد.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


يحصل على الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمورد.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

**Returns:**
java.lang.String - الموقع المحدد في مستند داخل ارتباط تشعبي مرتبط بموارد.
### getId() {#getId--}
```
public final int getId()
```


يحصل على قيمة Id.

**Returns:**
int - قيمة لـ Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


يحصل على قيمة تشير إلى ما إذا كان Inactive مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


يحصل على قيمة Initials.

**Returns:**
java.lang.String - قيمة لـ Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


يحصل على الموارد الفرعية.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - موارد فرعية.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


يحصل على قيمة MaterialLabel.

**Returns:**
java.lang.String - قيمة لـ MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


يحصل على قيمة MaxUnits.

**Returns:**
double - قيمة لـ MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


يحصل على قيمة Name.

**Returns:**
java.lang.String - قيمة لـ Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


يحصل على قيمة NotesRTF.

**Returns:**
java.lang.String - قيمة لـ NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


يحصل على قيمة NotesText.

**Returns:**
java.lang.String - قيمة لـ NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


يحصل على كائن OutlineCodeCollection. قيمة رمز المخطط.

--------------------

هناك قطعتان من البيانات ضرورية - مؤشر إلى جدول رمز المخطط المحدد بواسطة FieldID، والقيمة المحددة إما بواسطة ValueID أو مؤشر ValueGUID إلى قائمة القيم.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


يحصل على قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


يحصل على قيمة OvertimeCost.

**Returns:**
java.math.BigDecimal - قيمة لـ OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


يحصل على قيمة OvertimeRate.

**Returns:**
java.math.BigDecimal - قيمة لـ OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


يحصل على قيمة OvertimeRateFormat.

**Returns:**
int - قيمة لـ OvertimeRateFormat.
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


يحصل على المشروع الأصل لهذه الحاوية.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


يحصل على قيمة Phonetics.

**Returns:**
java.lang.String - قيمة لـ Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


يحصل على نسخة من فئة [RateCollection](../../com.aspose.tasks/ratecollection) لهذا الكائن. مجموعة الفترات والأسعار المرتبطة بكل منها.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


يحصل على قيمة SV.

**Returns:**
double - قيمة لـ SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


يحصل على قيمة StandardRate.

**Returns:**
java.math.BigDecimal - قيمة لـ StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


يحصل على قيمة StandardRateFormat.

**Returns:**
int - قيمة لـ StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


يحصل على قيمة Start.

**Returns:**
java.util.Date - قيمة لـ Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


يحصل على نسخة من الفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن.

--------------------

القراءة مدعومة لتنسيق XML فقط.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


يعيد [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن مع `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) القيم ضمن تواريخ البداية والنهاية المعطاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للبيانات المتدرجة زمنياً. |
| نهاية | java.util.Date | تاريخ الانتهاء للبيانات الزمنية المرحلية. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


يعيد نسخة من الفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن مع `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) القيم ضمن تواريخ البداية والنهاية المعطاة لنوع [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| بدء | java.util.Date | تاريخ البدء للبيانات الزمنية المرحلية. |
| نهاية | java.util.Date | تاريخ الانتهاء للبيانات الزمنية المرحلية. |
| timephasedType | byte | نوع البيانات الزمنية المرحلية ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


يحصل على قيمة Type.

**Returns:**
int - قيمة من Type.
### getUid() {#getUid--}
```
public final int getUid()
```


يحصل على قيمة Uid.

**Returns:**
int - قيمة من Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


يحصل على قيمة WindowsUserAccount.

**Returns:**
java.lang.String - قيمة من WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


يحصل على قيمة Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


يحصل على قيمة WorkVariance.

**Returns:**
double - قيمة من WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


يحصل على قيمة Workgroup.

**Returns:**
int - قيمة من Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


محجوز للاستخدام الداخلي.

**Returns:**
منطقي - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


يرجع قيمة رمز تجزئة للنسخة من الفئة [Resource](../../com.aspose.tasks/resource).

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


يحصل على قيمة تشير إلى ما إذا كان IsBudget مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


يحصل على قيمة تشير إلى ما إذا كان IsCostResource مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


يحصل على قيمة تشير إلى ما إذا كان IsEnterprise مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


يحصل على قيمة تشير إلى ما إذا كان IsGeneric مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


يحصل على قيمة تشير إلى ما إذا كان IsNull مضبوطًا أم لا.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


يحصل على العلامة التي تشير إلى ما إذا كان المورد موردًا جذريًا. المورد الجذري هو مورد خاص يُقصد به دعم البنى الداخلية لتنسيقات MS Project ولا يُقصد استخدامه مباشرةً من شفرة المستخدم.

**Returns:**
boolean - العلامة التي تشير إلى ما إذا كان المورد موردًا جذريًا.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


يحصل على قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مضبوطًا أم لا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مُحددًا أم لا.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | مفتاح الخاصية المحدد. [Rsc](../../com.aspose.tasks/rsc) للحصول على مفتاح الخاصية. |
| القيمة | java.util.Date | القيمة. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


يضبط قيمة ACWP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة من ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


يضبط قيمة AccrueAt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة من AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


يضبط قيمة ActiveDirectoryGuid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


يضبط قيمة ActualCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من ActualCost. |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


يضبط قيمة AvailableFrom.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


يضبط قيمة AvailableTo.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من AvailableTo. |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان IsBudget مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان IsBudget مضبوطًا أم لا. |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


يضبط قيمة للـ Calendar.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | قيمة من Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان CanLevel مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان CanLevel مضبوطًا أم لا. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


يضبط قيمة للـ Code.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


يضبط قيمة للـ Cost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


يضبط قيمة للـ CostCenter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


يضبط قيمة للـ CostPerUse.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة من CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان IsCostResource مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان IsCostResource مضبوطًا أم لا. |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


يضبط قيمة للـ EMailAddress.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان IsEnterprise مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان IsEnterprise مضبوطًا أم لا. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


يضبط قيمة للـ Finish.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة من Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان IsGeneric مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان IsGeneric مضبوطًا أم لا. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


يضبط قيمة للـ Group.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


يضبط قيمة للـ Guid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة من Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


يضبط العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


يضبط العنوان لرابط تشعبي مرتبط بمورد.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | العنوان الخاص برابط تشعبي مرتبط بمورد. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


يضبط الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمورد.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | الموقع المحدد في مستند داخل رابط تشعبي مرتبط بمورد. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


يضبط قيمة للـ Id.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان Inactive مضبوطًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان Inactive مضبوطًا أم لا. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


يضبط قيمة Initials.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


يضبط قيمة MaterialLabel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


يضبط قيمة MaxUnits.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


يضبط قيمة Name.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


يضبط قيمة NotesRTF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


يضبط قيمة NotesText.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان IsNull مُعَيَّنًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان IsNull مضبوطًا أم لا. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


يضبط قيمة تشير إلى ما إذا كان Overallocated مُعَيَّنًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | قيمة تشير إلى ما إذا كان Overallocated مضبوطًا أم لا. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


يضبط قيمة OvertimeCost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


يضبط قيمة OvertimeRate.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


يضبط قيمة OvertimeRateFormat.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة OvertimeRateFormat. |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


يضبط قيمة Phonetics.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة Phonetics. |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


يضبط قيمة SV.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


يضبط قيمة StandardRate.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة لـ StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


يضبط قيمة StandardRateFormat.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة لـ StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


يضبط قيمة Start.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة لـ Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مُعَيَّنًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان IsTeamAssignmentPool مُعينًا أم لا. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


يحدد مثيلاً لفئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن.

--------------------

القراءة مدعومة لتنسيق XML فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | مثال من فئة [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) لهذا الكائن. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


يحدد قيمة للنوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة لـ Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


يحدد قيمة للـ Uid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة لـ Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


يحدد قيمة لـ WindowsUserAccount.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة لـ WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


يحدد قيمة للـ Work.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة لـ Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


يحدد قيمة للـ WorkVariance.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | قيمة لـ WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


يحدد قيمة للـ Workgroup.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة لـ Workgroup. |

### toString() {#toString--}
```
public String toString()
```


يعيد تمثيل نص قصير لنسخة فئة [Resource](../../com.aspose.tasks/resource). التفاصيل الدقيقة للتمثيل غير محددة وقابلة للتغيير.

**Returns:**
java.lang.String - نص قصير يمثل كائن المورد.
