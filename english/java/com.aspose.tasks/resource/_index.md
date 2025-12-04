---
title: Resource
second_title: Aspose.Tasks for Java API Reference
description: Represents a resource in a project.
type: docs
weight: 247
url: /java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Represents a resource in a project.
## Methods

| Method | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returns the value to which the property is mapped in this container. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Maps the specified property to the specified value in this container. |
| [canLevel()](#canLevel--) | Gets a value indicating whether CanLevel is set or not. |
| [delete()](#delete--) | Deletes a resource and its assignments from project. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Returns a value indicating whether this instance is equal to a specified instance of the [Resource](../../com.aspose.tasks/resource) class. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getACWP()](#getACWP--) | Gets a value of ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Gets a value of AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Gets a value of ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Gets a value of ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Gets a value of ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Gets a value of ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Gets a value of ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Gets a value of ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Gets a value of ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Gets a value of AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Gets a value of AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Gets a collection of resource assignments for this object. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Gets a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class. |
| [getAvailableFrom()](#getAvailableFrom--) | Gets a value of AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Gets a value of AvailableTo. |
| [getBCWP()](#getBCWP--) | Gets a value of BCWP. |
| [getBCWS()](#getBCWS--) | Gets a value of BCWS. |
| [getBaselines()](#getBaselines--) | Gets a BaselineCollection instance for this object. |
| [getBookingType()](#getBookingType--) | Gets a value of BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Gets a value of BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Gets a value of BudgetWork. |
| [getCV()](#getCV--) | Gets a value of CV. |
| [getCalendar()](#getCalendar--) | Gets a value of Calendar. |
| [getCode()](#getCode--) | Gets a value of Code. |
| [getCost()](#getCost--) | Gets a value of Cost. |
| [getCostCenter()](#getCostCenter--) | Gets a value of CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Gets a value of CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Gets a value of CostVariance. |
| [getCreated()](#getCreated--) | Gets a value of Created. |
| [getEMailAddress()](#getEMailAddress--) | Gets a value of EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets the values of an extended attribute. |
| [getFinish()](#getFinish--) | Gets a value of Finish. |
| [getGroup()](#getGroup--) | Gets a value of Group. |
| [getGuid()](#getGuid--) | Gets a value of Guid. |
| [getHyperlink()](#getHyperlink--) | Gets the title or explanatory text of a hyperlink associated with a resource. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Gets the address for a hyperlink associated with a resource. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Gets the specific location in a document in a hyperlink associated with a resource. |
| [getId()](#getId--) | Gets a value of Id. |
| [getInactive()](#getInactive--) | Gets a value indicating whether Inactive is set or not. |
| [getInitials()](#getInitials--) | Gets a value of Initials. |
| [getItems()](#getItems--) | Gets child resources. |
| [getMaterialLabel()](#getMaterialLabel--) | Gets a value of MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Gets a value of MaxUnits. |
| [getName()](#getName--) | Gets a value of Name. |
| [getNotesRTF()](#getNotesRTF--) | Gets a value of NotesRTF. |
| [getNotesText()](#getNotesText--) | Gets a value of NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Gets an OutlineCodeCollection object. |
| [getOverallocated()](#getOverallocated--) | Gets a value indicating whether Overallocated is set or not. |
| [getOvertimeCost()](#getOvertimeCost--) | Gets a value of OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Gets a value of OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Gets a value of OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Gets a value of OvertimeWork. |
| [getParentProject()](#getParentProject--) | Gets parent project for this container. |
| [getPeakUnits()](#getPeakUnits--) | Gets a value of PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Gets a value of PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Gets a value of Phonetics. |
| [getRates()](#getRates--) | Gets a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object. |
| [getRegularWork()](#getRegularWork--) | Gets a value of RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Gets a value of RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Gets a value of RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Gets a value of RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Gets a value of RemainingWork. |
| [getSV()](#getSV--) | Gets a value of SV. |
| [getStandardRate()](#getStandardRate--) | Gets a value of StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Gets a value of StandardRateFormat. |
| [getStart()](#getStart--) | Gets a value of Start. |
| [getTimephasedData()](#getTimephasedData--) | Gets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) for this object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Returns an instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object with the `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Gets a value of Type. |
| [getUid()](#getUid--) | Gets a value of Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Gets a value of WindowsUserAccount. |
| [getWork()](#getWork--) | Gets a value of Work. |
| [getWorkVariance()](#getWorkVariance--) | Gets a value of WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Gets a value of Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [Resource](../../com.aspose.tasks/resource) class. |
| [isBudget()](#isBudget--) | Gets a value indicating whether IsBudget is set or not. |
| [isCostResource()](#isCostResource--) | Gets a value indicating whether IsCostResource is set or not. |
| [isEnterprise()](#isEnterprise--) | Gets a value indicating whether IsEnterprise is set or not. |
| [isGeneric()](#isGeneric--) | Gets a value indicating whether IsGeneric is set or not. |
| [isNull()](#isNull--) | Gets a value indicating whether IsNull is set or not. |
| [isRoot()](#isRoot--) | Gets the flag indicating whether resource is a root resource. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Gets a value indicating whether IsTeamAssignmentPool is set or not. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Maps the specified property to the specified value in this container. |
| [setACWP(double value)](#setACWP-double-) | Sets a value of ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Sets a value of AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Sets a value of ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Sets a value of ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Sets a value of ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Sets a value of ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Sets a value of AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Sets a value of AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Sets a value of AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Sets a value of AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Sets a value of BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Sets a value of BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Sets a value of BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsBudget is set or not. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Sets a value of BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Sets a value of BudgetWork. |
| [setCV(double value)](#setCV-double-) | Sets a value of CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Sets a value of Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Sets a value indicating whether CanLevel is set or not. |
| [setCode(String value)](#setCode-java.lang.String-) | Sets a value of Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sets a value of Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Sets a value of CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Sets a value of CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsCostResource is set or not. |
| [setCostVariance(double value)](#setCostVariance-double-) | Sets a value of CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Sets a value of Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Sets a value of EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsEnterprise is set or not. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sets a value of Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsGeneric is set or not. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Sets a value of Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Sets a value of Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Sets the title or explanatory text of a hyperlink associated with a resource. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Sets the address for a hyperlink associated with a resource. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Sets the specific location in a document in a hyperlink associated with a resource. |
| [setId(int value)](#setId-int-) | Sets a value of Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Sets a value indicating whether Inactive is set or not. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Sets a value of Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Sets a value of MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Sets a value of MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Sets a value of Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Sets a value of NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Sets a value of NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsNull is set or not. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Sets a value indicating whether Overallocated is set or not. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Sets a value of OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Sets a value of OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Sets a value of OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Sets a value of PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Sets a value of PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Sets a value of Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Sets a value of RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Sets a value of RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Sets a value of RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Sets a value of RemainingWork. |
| [setSV(double value)](#setSV-double-) | Sets a value of SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Sets a value of StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Sets a value of StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Sets a value of Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Sets a value indicating whether IsTeamAssignmentPool is set or not. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object. |
| [setType(int value)](#setType-int-) | Sets a value of Type. |
| [setUid(int value)](#setUid-int-) | Sets a value of Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Sets a value of WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Sets a value of Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Sets a value of WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Sets a value of Workgroup. |
| [toString()](#toString--) | Returns short string representation of the instance of the [Resource](../../com.aspose.tasks/resource) class. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key. |

**Returns:**
T - the value to which the property is mapped in this container.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key. |
| val | T | the value. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Gets a value indicating whether CanLevel is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Deletes a resource and its assignments from project.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Returns a value indicating whether this instance is equal to a specified instance of the [Resource](../../com.aspose.tasks/resource) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | The specified instance of the [Resource](../../com.aspose.tasks/resource) class to compare with this instance. |

**Returns:**
boolean - **True** if the specified instance of the [Resource](../../com.aspose.tasks/resource) class has the same Uid value as this instance; otherwise, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with this instance. |

**Returns:**
boolean - **True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Gets a value of ACWP.

**Returns:**
double - a value of ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Gets a value of AccrueAt.

**Returns:**
int - a value of AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Gets a value of ActiveDirectoryGuid.

**Returns:**
java.lang.String - a value of ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Gets a value of ActualCost.

**Returns:**
java.math.BigDecimal - a value of ActualCost.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Gets a value of ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - a value of ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Gets a value of ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Gets a value of ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Gets a value of ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Gets a value of ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Gets a value of AssignmentOwner.

**Returns:**
java.lang.String - a value of AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Gets a value of AssignmentOwnerGuid.

**Returns:**
java.lang.String - a value of AssignmentOwnerGuid.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Gets a collection of resource assignments for this object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Gets a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class. The collection of periods during which a resource is available.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Gets a value of AvailableFrom.

**Returns:**
java.util.Date - a value of AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Gets a value of AvailableTo.

**Returns:**
java.util.Date - a value of AvailableTo.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Gets a value of BCWP.

**Returns:**
double - a value of BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Gets a value of BCWS.

**Returns:**
double - a value of BCWS.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Gets a BaselineCollection instance for this object. The baseline values for a resource.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Gets a value of BookingType.

**Returns:**
int - a value of BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Gets a value of BudgetCost.

**Returns:**
java.math.BigDecimal - a value of BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Gets a value of BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Gets a value of CV.

**Returns:**
double - a value of CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Gets a value of Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Gets a value of Code.

**Returns:**
java.lang.String - a value of Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Gets a value of Cost.

**Returns:**
java.math.BigDecimal - a value of Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Gets a value of CostCenter.

**Returns:**
java.lang.String - a value of CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Gets a value of CostPerUse.

**Returns:**
java.math.BigDecimal - a value of CostPerUse.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Gets a value of CostVariance.

**Returns:**
double - a value of CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Gets a value of Created.

**Returns:**
java.util.Date - a value of Created.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Gets a value of EMailAddress.

**Returns:**
java.lang.String - a value of EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets the values of an extended attribute.

--------------------

Two pieces of data are necessary - a pointer back to the extended attribute table which is specified either by the unique ID or the Field ID, and the value which is specified either with the value, or a pointer back to the value list.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Gets a value of Finish.

**Returns:**
java.util.Date - a value of Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Gets a value of Group.

**Returns:**
java.lang.String - a value of Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets a value of Guid.

**Returns:**
java.lang.String - a value of Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Gets the title or explanatory text of a hyperlink associated with a resource.

**Returns:**
java.lang.String - the title or explanatory text of a hyperlink associated with a resource.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Gets the address for a hyperlink associated with a resource.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Returns:**
java.lang.String - the address for a hyperlink associated with a resource.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Gets the specific location in a document in a hyperlink associated with a resource.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Returns:**
java.lang.String - the specific location in a document in a hyperlink associated with a resource.
### getId() {#getId--}
```
public final int getId()
```


Gets a value of Id.

**Returns:**
int - a value of Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Gets a value indicating whether Inactive is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Gets a value of Initials.

**Returns:**
java.lang.String - a value of Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Gets child resources.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - child resources.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Gets a value of MaterialLabel.

**Returns:**
java.lang.String - a value of MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Gets a value of MaxUnits.

**Returns:**
double - a value of MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Gets a value of Name.

**Returns:**
java.lang.String - a value of Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Gets a value of NotesRTF.

**Returns:**
java.lang.String - a value of NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Gets a value of NotesText.

**Returns:**
java.lang.String - a value of NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Gets an OutlineCodeCollection object. The value of an outline code.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Gets a value indicating whether Overallocated is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Gets a value of OvertimeCost.

**Returns:**
java.math.BigDecimal - a value of OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Gets a value of OvertimeRate.

**Returns:**
java.math.BigDecimal - a value of OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Gets a value of OvertimeRateFormat.

**Returns:**
int - a value of OvertimeRateFormat.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Gets a value of OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets parent project for this container.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Gets a value of PeakUnits.

**Returns:**
double - a value of PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Gets a value of PercentWorkComplete.

**Returns:**
int - a value of PercentWorkComplete.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Gets a value of Phonetics.

**Returns:**
java.lang.String - a value of Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Gets a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object. The collection of periods and rates associated with each one.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Gets a value of RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Gets a value of RemainingCost.

**Returns:**
java.math.BigDecimal - a value of RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Gets a value of RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - a value of RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Gets a value of RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Gets a value of RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


Gets a value of SV.

**Returns:**
double - a value of SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Gets a value of StandardRate.

**Returns:**
java.math.BigDecimal - a value of StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Gets a value of StandardRateFormat.

**Returns:**
int - a value of StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Gets a value of Start.

**Returns:**
java.util.Date - a value of Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.

--------------------

Reading supported for XML format only.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) for this object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the timephased data. |
| end | java.util.Date | The end date for the timephased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Returns an instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object with the `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | byte | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Gets a value of Type.

**Returns:**
int - a value of Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets a value of Uid.

**Returns:**
int - a value of Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Gets a value of WindowsUserAccount.

**Returns:**
java.lang.String - a value of WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Gets a value of Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Gets a value of WorkVariance.

**Returns:**
double - a value of WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Gets a value of Workgroup.

**Returns:**
int - a value of Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Reserved for internal usage.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [Resource](../../com.aspose.tasks/resource) class.

**Returns:**
int - returns a hash code value for this object.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Gets a value indicating whether IsBudget is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Gets a value indicating whether IsCostResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Gets a value indicating whether IsEnterprise is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Gets a value indicating whether IsGeneric is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Gets a value indicating whether IsNull is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Gets the flag indicating whether resource is a root resource. Root resource is a special resource which is intended to support internals of MS Project's formats and is not intended to be used directly from the user's code.

**Returns:**
boolean - the flag indicating whether resource is a root resource.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Gets a value indicating whether IsTeamAssignmentPool is set or not.

**Returns:**
boolean - a value indicating whether IsTeamAssignmentPool is set or not.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key. |
| val | java.util.Date | the value. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Sets a value of ACWP.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Sets a value of AccrueAt.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Sets a value of ActiveDirectoryGuid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Sets a value of ActualCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of ActualCost. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Sets a value of ActualOvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Sets a value of ActualOvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Sets a value of ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualOvertimeWorkProtected. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Sets a value of ActualWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Sets a value of ActualWorkProtected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Sets a value of AssignmentOwner.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Sets a value of AssignmentOwnerGuid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of AssignmentOwnerGuid. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Sets a value of AvailableFrom.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Sets a value of AvailableTo.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of AvailableTo. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Sets a value of BCWP.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Sets a value of BCWS.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Sets a value of BookingType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BookingType. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Sets a value indicating whether IsBudget is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsBudget is set or not. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Sets a value of BudgetCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Sets a value of BudgetWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Sets a value of CV.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Sets a value indicating whether CanLevel is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether CanLevel is set or not. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Sets a value of Code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sets a value of Cost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Sets a value of CostCenter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Sets a value of CostPerUse.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Sets a value indicating whether IsCostResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsCostResource is set or not. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Sets a value of CostVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Sets a value of Created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Created. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Sets a value of EMailAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Sets a value indicating whether IsEnterprise is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsEnterprise is set or not. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sets a value of Finish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Sets a value indicating whether IsGeneric is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsGeneric is set or not. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Sets a value of Group.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Sets the title or explanatory text of a hyperlink associated with a resource.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the title or explanatory text of a hyperlink associated with a resource. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Sets the address for a hyperlink associated with a resource.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the address for a hyperlink associated with a resource. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Sets the specific location in a document in a hyperlink associated with a resource.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the specific location in a document in a hyperlink associated with a resource. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Sets a value of Id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Sets a value indicating whether Inactive is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Inactive is set or not. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Sets a value of Initials.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Sets a value of MaterialLabel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Sets a value of MaxUnits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Sets a value of NotesRTF.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Sets a value of NotesText.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Sets a value indicating whether IsNull is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsNull is set or not. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Sets a value indicating whether Overallocated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Overallocated is set or not. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Sets a value of OvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Sets a value of OvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Sets a value of OvertimeRateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of OvertimeRateFormat. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Sets a value of OvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Sets a value of PeakUnits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Sets a value of PercentWorkComplete.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of PercentWorkComplete. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Sets a value of Phonetics.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Phonetics. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Sets a value of RegularWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Sets a value of RemainingCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Sets a value of RemainingOvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Sets a value of RemainingOvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Sets a value of RemainingWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RemainingWork. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Sets a value of SV.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Sets a value of StandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Sets a value of StandardRateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Sets a value of Start.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Sets a value indicating whether IsTeamAssignmentPool is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IsTeamAssignmentPool is set or not. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.

--------------------

Reading supported for XML format only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Sets a value of Type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Sets a value of WindowsUserAccount.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Sets a value of Work.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Sets a value of WorkVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Sets a value of Workgroup.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Returns short string representation of the instance of the [Resource](../../com.aspose.tasks/resource) class. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents resource object.
