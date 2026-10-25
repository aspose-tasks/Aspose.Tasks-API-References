---
title: "资源"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目中的资源。"
type: docs
weight: 248
url: /zh/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

表示项目中的资源。
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 返回此容器中属性映射的值。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 将指定属性映射到此容器中的指定值。 |
| [canLevel()](#canLevel--) | 获取一个值，指示 CanLevel 是否已设置。 |
| [delete()](#delete--) | 从项目中删除资源及其分配。 |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | 返回一个值，指示此实例是否等于指定的 [Resource](../../com.aspose.tasks/resource) 类的实例。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getACWP()](#getACWP--) | 获取 ACWP 的值。 |
| [getAccrueAt()](#getAccrueAt--) | 获取 AccrueAt 的值。 |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | 获取 ActiveDirectoryGuid 的值。 |
| [getActualCost()](#getActualCost--) | 获取 ActualCost 的值。 |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | 获取 ActualOvertimeCost 的值。 |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | 获取 ActualOvertimeWork 的值。 |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | 获取 ActualOvertimeWorkProtected 的值。 |
| [getActualWork()](#getActualWork--) | 获取 ActualWork 的值。 |
| [getActualWorkProtected()](#getActualWorkProtected--) | 获取 ActualWorkProtected 的值。 |
| [getAssignmentOwner()](#getAssignmentOwner--) | 获取 AssignmentOwner 的值。 |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | 获取 AssignmentOwnerGuid 的值。 |
| [getAssignments()](#getAssignments--) | 获取此对象的资源分配集合。 |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | 获取 [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) 类的实例。 |
| [getAvailableFrom()](#getAvailableFrom--) | 获取 AvailableFrom 的值。 |
| [getAvailableTo()](#getAvailableTo--) | 获取 AvailableTo 的值。 |
| [getBCWP()](#getBCWP--) | 获取 BCWP 的值。 |
| [getBCWS()](#getBCWS--) | 获取 BCWS 的值。 |
| [getBaselines()](#getBaselines--) | 获取此对象的 BaselineCollection 实例。 |
| [getBookingType()](#getBookingType--) | 获取 BookingType 的值。 |
| [getBudgetCost()](#getBudgetCost--) | 获取 BudgetCost 的值。 |
| [getBudgetWork()](#getBudgetWork--) | 获取 BudgetWork 的值。 |
| [getCV()](#getCV--) | 获取 CV 的值。 |
| [getCalendar()](#getCalendar--) | 获取 Calendar 的值。 |
| [getCode()](#getCode--) | 获取 Code 的值。 |
| [getCost()](#getCost--) | 获取 Cost 的值。 |
| [getCostCenter()](#getCostCenter--) | 获取 CostCenter 的值。 |
| [getCostPerUse()](#getCostPerUse--) | 获取 CostPerUse 的值。 |
| [getCostVariance()](#getCostVariance--) | 获取 CostVariance 的值。 |
| [getCreated()](#getCreated--) | 获取 Created 的值。 |
| [getEMailAddress()](#getEMailAddress--) | 获取 EMailAddress 的值。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | 获取扩展属性的值。 |
| [getFinish()](#getFinish--) | 获取 Finish 的值。 |
| [getGroup()](#getGroup--) | 获取 Group 的值。 |
| [getGuid()](#getGuid--) | 获取 Guid 的值。 |
| [getHyperlink()](#getHyperlink--) | 获取与资源关联的超链接的标题或说明文本。 |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | 获取与资源关联的超链接的地址。 |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | 获取与资源关联的超链接在文档中的具体位置。 |
| [getId()](#getId--) | 获取 Id 的值。 |
| [getInactive()](#getInactive--) | 获取指示是否已设置 Inactive 的值。 |
| [getInitials()](#getInitials--) | 获取 Initials 的值。 |
| [getItems()](#getItems--) | 获取子资源。 |
| [getMaterialLabel()](#getMaterialLabel--) | 获取 MaterialLabel 的值。 |
| [getMaxUnits()](#getMaxUnits--) | 获取 MaxUnits 的值。 |
| [getName()](#getName--) | 获取 Name 的值。 |
| [getNotesRTF()](#getNotesRTF--) | 获取 NotesRTF 的值。 |
| [getNotesText()](#getNotesText--) | 获取 NotesText 的值。 |
| [getOutlineCode()](#getOutlineCode--) | 获取 OutlineCodeCollection 对象。 |
| [getOverallocated()](#getOverallocated--) | 获取指示是否已设置 Overallocated 的值。 |
| [getOvertimeCost()](#getOvertimeCost--) | 获取 OvertimeCost 的值。 |
| [getOvertimeRate()](#getOvertimeRate--) | 获取 OvertimeRate 的值。 |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | 获取 OvertimeRateFormat 的值。 |
| [getOvertimeWork()](#getOvertimeWork--) | 获取 OvertimeWork 的值。 |
| [getParentProject()](#getParentProject--) | 获取此容器的父项目。 |
| [getPeakUnits()](#getPeakUnits--) | 获取 PeakUnits 的值。 |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | 获取 PercentWorkComplete 的值。 |
| [getPhonetics()](#getPhonetics--) | 获取 Phonetics 的值。 |
| [getRates()](#getRates--) | 获取此对象的 [RateCollection](../../com.aspose.tasks/ratecollection) 类的实例。 |
| [getRegularWork()](#getRegularWork--) | 获取 RegularWork 的值。 |
| [getRemainingCost()](#getRemainingCost--) | 获取 RemainingCost 的值。 |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | 获取 RemainingOvertimeCost 的值。 |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | 获取 RemainingOvertimeWork 的值。 |
| [getRemainingWork()](#getRemainingWork--) | 获取 RemainingWork 的值。 |
| [getSV()](#getSV--) | 获取 SV 的值。 |
| [getStandardRate()](#getStandardRate--) | 获取 StandardRate 的值。 |
| [getStandardRateFormat()](#getStandardRateFormat--) | 获取 StandardRateFormat 的值。 |
| [getStart()](#getStart--) | 获取 Start 的值。 |
| [getTimephasedData()](#getTimephasedData--) | 获取此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。 |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | 返回此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)，其中包含在给定开始和结束日期内的 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 值。 |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | 返回此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例，其中包含在给定开始和结束日期内、指定的 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) 的 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 值。 |
| [getType()](#getType--) | 获取 Type 的值。 |
| [getUid()](#getUid--) | 获取 Uid 的值。 |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | 获取 WindowsUserAccount 的值。 |
| [getWork()](#getWork--) | 获取 Work 的值。 |
| [getWorkVariance()](#getWorkVariance--) | 获取 WorkVariance 的值。 |
| [getWorkgroup()](#getWorkgroup--) | 获取 Workgroup 的值。 |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | 返回 [Resource](../../com.aspose.tasks/resource) 类实例的哈希码值。 |
| [isBudget()](#isBudget--) | 获取指示 IsBudget 是否已设置的值。 |
| [isCostResource()](#isCostResource--) | 获取指示 IsCostResource 是否已设置的值。 |
| [isEnterprise()](#isEnterprise--) | 获取指示 IsEnterprise 是否已设置的值。 |
| [isGeneric()](#isGeneric--) | 获取指示 IsGeneric 是否已设置的值。 |
| [isNull()](#isNull--) | 获取指示 IsNull 是否已设置的值。 |
| [isRoot()](#isRoot--) | 获取指示资源是否为根资源的标志。 |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | 获取指示 IsTeamAssignmentPool 是否已设置的值。 |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | 将指定属性映射到此容器中的指定值。 |
| [setACWP(double value)](#setACWP-double-) | 设置 ACWP 的值。 |
| [setAccrueAt(int value)](#setAccrueAt-int-) | 设置 AccrueAt 的值。 |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | 设置 ActiveDirectoryGuid 的值。 |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | 设置 ActualCost 的值。 |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | 设置 ActualOvertimeCost 的值。 |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | 设置 ActualOvertimeWork 的值。 |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | 设置 ActualOvertimeWorkProtected 的值。 |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | 设置 ActualWork 的值。 |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | 设置 ActualWorkProtected 的值。 |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | 设置 AssignmentOwner 的值。 |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | 设置 AssignmentOwnerGuid 的值。 |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | 设置 AvailableFrom 的值。 |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | 设置 AvailableTo 的值。 |
| [setBCWP(double value)](#setBCWP-double-) | 设置 BCWP 的值。 |
| [setBCWS(double value)](#setBCWS-double-) | 设置 BCWS 的值。 |
| [setBookingType(int value)](#setBookingType-int-) | 设置 BookingType 的值。 |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | 设置一个值，指示 IsBudget 是否已设置。 |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | 设置 BudgetCost 的值。 |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | 设置 BudgetWork 的值。 |
| [setCV(double value)](#setCV-double-) | 设置 CV 的值。 |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | 设置 Calendar 的值。 |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | 设置一个值，指示 CanLevel 是否已设置。 |
| [setCode(String value)](#setCode-java.lang.String-) | 设置 Code 的值。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | 设置 Cost 的值。 |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | 设置 CostCenter 的值。 |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | 设置 CostPerUse 的值。 |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | 设置一个值，指示 IsCostResource 是否已设置。 |
| [setCostVariance(double value)](#setCostVariance-double-) | 设置 CostVariance 的值。 |
| [setCreated(Date value)](#setCreated-java.util.Date-) | 设置 Created 的值。 |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | 设置 EMailAddress 的值。 |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | 设置一个值，指示 IsEnterprise 是否已设置。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 设置 Finish 的值。 |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | 设置一个值，指示 IsGeneric 是否已设置。 |
| [setGroup(String value)](#setGroup-java.lang.String-) | 设置 Group 的值。 |
| [setGuid(String value)](#setGuid-java.lang.String-) | 设置 Guid 的值。 |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | 设置与资源关联的超链接的标题或说明文本。 |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | 设置与资源关联的超链接的地址。 |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | 设置与资源关联的超链接在文档中的具体位置。 |
| [setId(int value)](#setId-int-) | 设置 Id 的值。 |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | 设置一个值，指示 Inactive 是否已设置。 |
| [setInitials(String value)](#setInitials-java.lang.String-) | 设置 Initials 的值。 |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | 设置 MaterialLabel 的值。 |
| [setMaxUnits(double value)](#setMaxUnits-double-) | 设置 MaxUnits 的值。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 Name 的值。 |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | 设置 NotesRTF 的值。 |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | 设置 NotesText 的值。 |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | 设置一个值，指示 IsNull 是否已设置。 |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | 设置一个值，指示 Overallocated 是否已设置。 |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | 设置 OvertimeCost 的值。 |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | 设置 OvertimeRate 的值。 |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | 设置 OvertimeRateFormat 的值。 |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | 设置 OvertimeWork 的值。 |
| [setPeakUnits(double value)](#setPeakUnits-double-) | 设置 PeakUnits 的值。 |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | 设置 PercentWorkComplete 的值。 |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | 设置 Phonetics 的值。 |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | 设置 RegularWork 的值。 |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | 设置 RemainingCost 的值。 |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | 设置 RemainingOvertimeCost 的值。 |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | 设置 RemainingOvertimeWork 的值。 |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | 设置 RemainingWork 的值。 |
| [setSV(double value)](#setSV-double-) | 设置 SV 的值。 |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | 设置 StandardRate 的值。 |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | 设置 StandardRateFormat 的值。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 设置 Start 的值。 |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | 设置一个值，指示 IsTeamAssignmentPool 是否已设置。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 为此对象设置 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。 |
| [setType(int value)](#setType-int-) | 设置 Type 的值。 |
| [setUid(int value)](#setUid-int-) | 设置 Uid 的值。 |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | 设置 WindowsUserAccount 的值。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | 设置 Work 的值。 |
| [setWorkVariance(double value)](#setWorkVariance-double-) | 设置 WorkVariance 的值。 |
| [setWorkgroup(int value)](#setWorkgroup-int-) | 设置 Workgroup 的值。 |
| [toString()](#toString--) | 返回 [Resource](../../com.aspose.tasks/resource) 类实例的简短字符串表示。 |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


返回此容器中属性映射的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。 [Rsc](../../com.aspose.tasks/rsc) 用于获取属性键。 |

**Returns:**
T - 在此容器中映射到的属性值。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


将指定属性映射到此容器中的指定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。 [Rsc](../../com.aspose.tasks/rsc) 用于获取属性键。 |
| val | T | 该值。 |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


获取一个值，指示 CanLevel 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


从项目中删除资源及其分配。

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


返回一个值，指示此实例是否等于指定的 [Resource](../../com.aspose.tasks/resource) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | 指定的 [Resource](../../com.aspose.tasks/resource) 类实例，用于与此实例比较。 |

**Returns:**
boolean - **True** 如果指定的 [Resource](../../com.aspose.tasks/resource) 类实例的 Uid 值与此实例相同；否则 **false**。
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
boolean - **True** 如果指定的对象是具有相同 Uid 值的 Resource；否则 **false**。
### getACWP() {#getACWP--}
```
public final double getACWP()
```


获取 ACWP 的值。

**Returns:**
double - ACWP 的值。
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


获取 AccrueAt 的值。

**Returns:**
int - AccrueAt 的值。
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


获取 ActiveDirectoryGuid 的值。

**Returns:**
java.lang.String - ActiveDirectoryGuid 的值。
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


获取 ActualCost 的值。

**Returns:**
java.math.BigDecimal - ActualCost 的值。
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


获取此对象的资源分配集合。

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


获取 [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) 类的实例。该集合包含资源可用的期间。

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


获取 AvailableFrom 的值。

**Returns:**
java.util.Date - AvailableFrom 的值。
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


获取 AvailableTo 的值。

**Returns:**
java.util.Date - AvailableTo 的值。
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
public final BaselineCollection getBaselines()
```


获取此对象的 BaselineCollection 实例。资源的基线值。

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


获取 Calendar 的值。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


获取 Code 的值。

**Returns:**
java.lang.String - Code 的值。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


获取 Cost 的值。

**Returns:**
java.math.BigDecimal - Cost 的值。
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


获取 CostCenter 的值。

**Returns:**
java.lang.String - CostCenter 的值。
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


获取 CostPerUse 的值。

**Returns:**
java.math.BigDecimal - CostPerUse 的值。
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


获取 EMailAddress 的值。

**Returns:**
java.lang.String - EMailAddress 的值。
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


获取扩展属性的值。

--------------------

需要两个数据项 - 一个指向扩展属性表的指针，可通过唯一 ID 或字段 ID 指定，以及一个值，可直接提供该值，或指向值列表的指针。

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


获取 Finish 的值。

**Returns:**
java.util.Date - Finish 的值。
### getGroup() {#getGroup--}
```
public final String getGroup()
```


获取 Group 的值。

**Returns:**
java.lang.String - Group 的值。
### getGuid() {#getGuid--}
```
public final String getGuid()
```


获取 Guid 的值。

**Returns:**
java.lang.String - Guid 的值。
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


获取与资源关联的超链接的标题或说明文本。

**Returns:**
java.lang.String - 与资源关联的超链接的标题或说明文字。
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


获取与资源关联的超链接的地址。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

**Returns:**
java.lang.String - 与资源关联的超链接的地址。
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


获取与资源关联的超链接在文档中的具体位置。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

**Returns:**
java.lang.String - 与资源关联的超链接中文档的具体位置。
### getId() {#getId--}
```
public final int getId()
```


获取 Id 的值。

**Returns:**
int - Id 的值。
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


获取指示是否已设置 Inactive 的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


获取 Initials 的值。

**Returns:**
java.lang.String - Initials 的值。
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


获取子资源。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - 子资源。
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


获取 MaterialLabel 的值。

**Returns:**
java.lang.String - MaterialLabel 的一个值。
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


获取 MaxUnits 的值。

**Returns:**
double - MaxUnits 的一个值。
### getName() {#getName--}
```
public final String getName()
```


获取 Name 的值。

**Returns:**
java.lang.String - Name 的一个值。
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


获取 NotesRTF 的值。

**Returns:**
java.lang.String - NotesRTF 的一个值。
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


获取 NotesText 的值。

**Returns:**
java.lang.String - NotesText 的一个值。
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


获取 OutlineCodeCollection 对象。大纲代码的值。

--------------------

需要两个数据项 - 由 FieldID 指定的大纲代码表指针，以及由 ValueID 或 ValueGUID 指定的指向值列表的指针。

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


获取指示是否已设置 Overallocated 的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


获取 OvertimeCost 的值。

**Returns:**
java.math.BigDecimal - OvertimeCost 的一个值。
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


获取 OvertimeRate 的值。

**Returns:**
java.math.BigDecimal - OvertimeRate 的一个值。
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


获取 OvertimeRateFormat 的值。

**Returns:**
int - OvertimeRateFormat 的一个值。
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


获取此容器的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


获取 Phonetics 的值。

**Returns:**
java.lang.String - Phonetics 的一个值。
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


获取此对象的 [RateCollection](../../com.aspose.tasks/ratecollection) 类的实例。每个实例关联的期间和费率集合。

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


获取 SV 的值。

**Returns:**
double - SV 的一个值。
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


获取 StandardRate 的值。

**Returns:**
java.math.BigDecimal - StandardRate 的一个值。
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


获取 StandardRateFormat 的值。

**Returns:**
int - StandardRateFormat 的一个值。
### getStart() {#getStart--}
```
public final Date getStart()
```


获取 Start 的值。

**Returns:**
java.util.Date - Start 的一个值。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


获取此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。

--------------------

仅支持读取 XML 格式。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


返回此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)，其中包含在给定开始和结束日期内的 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 时间分段数据的开始日期。 |
| 结束 | java.util.Date | 时间分段数据的结束日期。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


返回此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例，其中包含在给定开始和结束日期内、指定的 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) 的 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | java.util.Date | 时间分段数据的开始日期。 |
| 结束 | java.util.Date | 时间分段数据的结束日期。 |
| timephasedType | byte | 时间分段数据的类型 ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype))。 |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


获取 Type 的值。

**Returns:**
int - Type 的值。
### getUid() {#getUid--}
```
public final int getUid()
```


获取 Uid 的值。

**Returns:**
int - Uid 的值。
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


获取 WindowsUserAccount 的值。

**Returns:**
java.lang.String - WindowsUserAccount 的值。
### getWork() {#getWork--}
```
public final Duration getWork()
```


获取 Work 的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


获取 WorkVariance 的值。

**Returns:**
double - WorkVariance 的值。
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


获取 Workgroup 的值。

**Returns:**
int - Workgroup 的值。
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


保留供内部使用。

**Returns:**
布尔 - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [Resource](../../com.aspose.tasks/resource) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


获取指示 IsBudget 是否已设置的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


获取指示 IsCostResource 是否已设置的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


获取指示 IsEnterprise 是否已设置的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


获取指示 IsGeneric 是否已设置的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


获取指示 IsNull 是否已设置的值。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


获取指示资源是否为根资源的标志。根资源是一种特殊资源，旨在支持 MS Project 格式的内部实现，不应直接在用户代码中使用。

**Returns:**
boolean - 指示资源是否为根资源的标志。
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


获取指示 IsTeamAssignmentPool 是否已设置的值。

**Returns:**
boolean - 表示 IsTeamAssignmentPool 是否已设置的值。
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


将指定属性映射到此容器中的指定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | 指定的属性键。 [Rsc](../../com.aspose.tasks/rsc) 用于获取属性键。 |
| val | java.util.Date | 该值。 |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


设置 ACWP 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | ACWP 的值。 |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


设置 AccrueAt 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | AccrueAt 的值。 |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


设置 ActiveDirectoryGuid 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | ActiveDirectoryGuid 的值。 |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


设置 ActualCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | ActualCost 的值。 |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


设置 AvailableFrom 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | AvailableFrom 的一个值。 |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


设置 AvailableTo 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | AvailableTo 的一个值。 |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


设置一个值，指示 IsBudget 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示 IsBudget 是否已设置的一个值。 |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


设置 Calendar 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | Calendar 的一个值。 |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


设置一个值，指示 CanLevel 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示 CanLevel 是否已设置的一个值。 |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


设置 Code 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Code 的一个值。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


设置 Cost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | Cost 的一个值。 |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


设置 CostCenter 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | CostCenter 的一个值。 |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


设置 CostPerUse 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | CostPerUse 的一个值。 |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


设置一个值，指示 IsCostResource 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示 IsCostResource 是否已设置的一个值。 |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


设置 EMailAddress 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | EMailAddress 的一个值。 |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


设置一个值，指示 IsEnterprise 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示 IsEnterprise 是否已设置的一个值。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


设置 Finish 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Finish 的一个值。 |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


设置一个值，指示 IsGeneric 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示 IsGeneric 是否已设置的一个值。 |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


设置 Group 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Group 的一个值。 |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


设置 Guid 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Guid 的一个值。 |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


设置与资源关联的超链接的标题或说明文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 资源关联的超链接的标题或说明文字。 |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


设置与资源关联的超链接的地址。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 资源关联的超链接的地址。 |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


设置与资源关联的超链接在文档中的具体位置。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 资源关联的超链接中文档的特定位置。 |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


设置 Id 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Id 的值。 |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


设置一个值，指示 Inactive 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示是否设置了 Inactive 的值。 |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


设置 Initials 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Initials 的值。 |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


设置 MaterialLabel 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | MaterialLabel 的值。 |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


设置 MaxUnits 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | MaxUnits 的值。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置 Name 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Name 的值。 |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


设置 NotesRTF 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | NotesRTF 的值。 |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


设置 NotesText 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | NotesText 的值。 |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


设置一个值，指示 IsNull 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示是否设置了 IsNull 的值。 |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


设置一个值，指示 Overallocated 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | 指示是否设置了 Overallocated 的值。 |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


设置 OvertimeCost 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | OvertimeCost 的值。 |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


设置 OvertimeRate 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | OvertimeRate 的值。 |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


设置 OvertimeRateFormat 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | OvertimeRateFormat 的值。 |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


设置 Phonetics 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Phonetics 的值。 |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


设置 SV 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | SV 的值。 |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


设置 StandardRate 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | StandardRate 的值。 |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


设置 StandardRateFormat 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | StandardRateFormat 的值。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


设置 Start 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Start 的值。 |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


设置一个值，指示 IsTeamAssignmentPool 是否已设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示 IsTeamAssignmentPool 是否已设置的值。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


为此对象设置 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的实例。

--------------------

仅支持读取 XML 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类实例。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


设置 Type 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Type 的值。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


设置 Uid 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Uid 的值。 |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


设置 WindowsUserAccount 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | WindowsUserAccount 的值。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


设置 Work 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work 的值。 |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


设置 WorkVariance 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | WorkVariance 的值。 |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


设置 Workgroup 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Workgroup 的值。 |

### toString() {#toString--}
```
public String toString()
```


返回 [Resource](../../com.aspose.tasks/resource) 类实例的简短字符串表示。该表示的具体细节未指定，可能会更改。

**Returns:**
java.lang.String - 表示资源对象的简短字符串。
