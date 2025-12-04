---
title: ResourceAssignment
second_title: Aspose.Tasks for Java API Reference
description: Represents a resource assignment in a project.
type: docs
weight: 248
url: /java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Represents a resource assignment in a project.
## Methods

| Method | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returns the value to which the property is mapped in this container. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Maps the specified property to the specified value in this container. |
| [delete()](#delete--) | Deletes resource assignment from project assignments collection. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Returns a value indicating whether this instance is equal to a specified instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getACWP()](#getACWP--) | Gets a value of ACWP. |
| [getActualCost()](#getActualCost--) | Gets a value of ActualCost. |
| [getActualFinish()](#getActualFinish--) | Gets a value of ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Gets a value of ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Gets a value of ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Gets a value of ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Gets a value of ActualStart. |
| [getActualWork()](#getActualWork--) | Gets a value of ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Gets a value of ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Gets a value of AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Gets a value of AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Gets a value of BCWP. |
| [getBCWS()](#getBCWS--) | Gets a value of BCWS. |
| [getBaselines()](#getBaselines--) | Gets AssignmentBaselineCollection object. |
| [getBookingType()](#getBookingType--) | Gets a value of BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Gets a value of BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Gets a value of BudgetWork. |
| [getCV()](#getCV--) | Gets a value of CV. |
| [getConfirmed()](#getConfirmed--) | Gets a value indicating whether Confirmed is set or not. |
| [getCost()](#getCost--) | Gets a value of Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Gets a value of CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Gets a value of CostVariance. |
| [getCreated()](#getCreated--) | Gets a value of Created. |
| [getDelay()](#getDelay--) | Gets a value of Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets an instance of the ExtendedAttributeCollection class for this object. |
| [getFinish()](#getFinish--) | Gets a value of Finish. |
| [getFinishVariance()](#getFinishVariance--) | Gets a value of FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Gets a value indicating whether FixedMaterial is set or not. |
| [getGuid()](#getGuid--) | Gets unique identifier for this assignment. |
| [getHyperlink()](#getHyperlink--) | Gets a value of Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Gets a value of HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Gets a value of HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Gets a value of LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Gets a value indicating whether LinkedFields is set or not. |
| [getMilestone()](#getMilestone--) | Gets a value indicating whether Milestone is set or not. |
| [getNotesRTF()](#getNotesRTF--) | Gets the text notes in RTF format. |
| [getNotesText()](#getNotesText--) | Gets notes' plain text extracted from RTF data. |
| [getOverallocated()](#getOverallocated--) | Gets a value indicating whether Overallocated is set or not. |
| [getOvertimeCost()](#getOvertimeCost--) | Gets a value of OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Gets a value of OvertimeWork. |
| [getParentProject()](#getParentProject--) | Gets parent project for this assignment. |
| [getPeakUnits()](#getPeakUnits--) | Gets a value of PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Gets a value of PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Gets a value of RateScale. |
| [getRegularWork()](#getRegularWork--) | Gets a value of RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Gets a value of RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Gets a value of RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Gets a value of RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Gets a value of RemainingWork. |
| [getResource()](#getResource--) | The resource assigned to a task. |
| [getResponsePending()](#getResponsePending--) | Gets a value indicating whether ResponsePending is set or not. |
| [getResume()](#getResume--) | Gets a value of Resume. |
| [getSV()](#getSV--) | Gets a value of SV. |
| [getStart()](#getStart--) | Gets a value of Start. |
| [getStartVariance()](#getStartVariance--) | Gets a value of StartVariance. |
| [getStop()](#getStop--) | Gets a value of Stop. |
| [getSummary()](#getSummary--) | Gets a value indicating whether Summary is set or not. |
| [getTask()](#getTask--) | The task to which a resource is assigned. |
| [getTimephasedData()](#getTimephasedData--) | Gets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with the instances of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Returns the instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing instances of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Gets amount of timephased work for the specified date time interval. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Gets amount of timephased work for the specified date time interval. |
| [getUid()](#getUid--) | Gets a value of Uid. |
| [getUnits()](#getUnits--) | Gets a value of Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Gets a value indicating whether UpdateNeeded is set or not. |
| [getVAC()](#getVAC--) | Gets a value of VAC. |
| [getWork()](#getWork--) | Gets a value of Work. |
| [getWorkContour()](#getWorkContour--) | Gets a value of WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Gets a value of WorkVariance. |
| [hasChildren()](#hasChildren--) | Gets a value indicating that this resource assignment has children. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Gets a value indicating whether HasFixedRateUnits is set or not. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Generates a list of time phased data. |
| [setACWP(double value)](#setACWP-double-) | Sets a value of ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Sets a value of ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Sets a value of ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Sets a value of ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Sets a value of ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Sets a value of ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Sets a value of AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Sets a value of AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Sets a value of BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Sets a value of BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Sets a value of BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Sets a value of BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Sets a value of BudgetWork. |
| [setCV(double value)](#setCV-double-) | Sets a value of CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Sets a value indicating whether Confirmed is set or not. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sets a value of Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Sets a value of CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Sets a value of CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Sets a value of Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Sets a value of Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Sets an instance of the ExtendedAttributeCollection class for this object. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sets a value of Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Sets a value of FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Sets a value indicating whether FixedMaterial is set or not. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Sets a value indicating whether HasFixedRateUnits is set or not. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Sets unique identifier for this assignment. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Sets a value of Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Sets a value of HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Sets a value of HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Sets a value of LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Sets a value indicating whether LinkedFields is set or not. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Sets units for assignment of a material resource with variable material consumption. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Sets a value indicating whether Milestone is set or not. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Sets the text notes in RTF format. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Sets notes' plain text extracted from RTF data. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Sets a value indicating whether Overallocated is set or not. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Sets a value of OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Sets a value of PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Sets a value of PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Sets a value of RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Sets a value of RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Sets a value of RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Sets a value of RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Sets a value of RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | The resource assigned to a task. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Sets a value indicating whether ResponsePending is set or not. |
| [setResume(Date value)](#setResume-java.util.Date-) | Sets a value of Resume. |
| [setSV(double value)](#setSV-double-) | Sets a value of SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Sets a value of Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Sets a value of StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Sets a value of Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Sets a value indicating whether Summary is set or not. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | The task to which a resource is assigned. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class. |
| [setUid(int value)](#setUid-int-) | Sets a value of Uid. |
| [setUnits(double value)](#setUnits-double-) | Sets a value of Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Sets a value indicating whether UpdateNeeded is set or not. |
| [setVAC(double value)](#setVAC-double-) | Sets a value of VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Sets a value of Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Sets a value of WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Sets a value of WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Splits task into two parts. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Generates list of time phased data based on the task duration and the scheduled start date. |
| [toString()](#toString--) | Returns short string representation of the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Asn](../../com.aspose.tasks/asn) for getting the property key. |

**Returns:**
T - the value to which the property is mapped in this container.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Asn](../../com.aspose.tasks/asn) for getting the property key. |
| val | T | the value. |

### delete() {#delete--}
```
public final void delete()
```


Deletes resource assignment from project assignments collection.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Returns a value indicating whether this instance is equal to a specified instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | The specified instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class to compare with this instance. |

**Returns:**
boolean - **True** if the specified instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class has the same UID value as this instance; otherwise, **false**.
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
boolean - **True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Gets a value of ACWP.

**Returns:**
double - a value of ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Gets a value of ActualCost.

**Returns:**
java.math.BigDecimal - a value of ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Gets a value of ActualFinish.

**Returns:**
java.util.Date - a value of ActualFinish.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Gets a value of ActualStart.

**Returns:**
java.util.Date - a value of ActualStart.
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
public final AssignmentBaselineCollection getBaselines()
```


Gets AssignmentBaselineCollection object. The collection of baseline values associated with an assignment.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Gets a value indicating whether Confirmed is set or not.

**Returns:**
boolean - a value indicating whether Confirmed is set or not.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Gets a value of Cost.

**Returns:**
java.math.BigDecimal - a value of Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Gets a value of CostRateTableType.

**Returns:**
int - a value of CostRateTableType.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Gets a value of Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets an instance of the ExtendedAttributeCollection class for this object.

--------------------

Reading supported for XML format only.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Gets a value of Finish.

**Returns:**
java.util.Date - a value of Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Gets a value of FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Gets a value indicating whether FixedMaterial is set or not.

**Returns:**
boolean - a value indicating whether FixedMaterial is set or not.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Gets unique identifier for this assignment.

**Returns:**
java.util.UUID - unique identifier for this assignment.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Gets a value of Hyperlink.

**Returns:**
java.lang.String - a value of Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Gets a value of HyperlinkAddress.

**Returns:**
java.lang.String - a value of HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Gets a value of HyperlinkSubAddress.

**Returns:**
java.lang.String - a value of HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Reserved for internal usage.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Gets a value of LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Gets a value indicating whether LinkedFields is set or not.

**Returns:**
boolean - a value indicating whether LinkedFields is set or not.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Gets a value indicating whether Milestone is set or not.

**Returns:**
boolean - a value indicating whether Milestone is set or not.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Gets the text notes in RTF format.

--------------------

Supported for MPP formats only.

**Returns:**
java.lang.String - the text notes in RTF format.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Gets notes' plain text extracted from RTF data.

**Returns:**
java.lang.String - notes' plain text extracted from RTF data.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Gets a value indicating whether Overallocated is set or not.

**Returns:**
boolean - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Gets a value of OvertimeCost.

**Returns:**
java.math.BigDecimal - a value of OvertimeCost.
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


Gets parent project for this assignment.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Gets a value of RateScale.

**Returns:**
int - a value of RateScale.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


The resource assigned to a task.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Gets a value indicating whether ResponsePending is set or not.

**Returns:**
boolean - a value indicating whether ResponsePending is set or not.
### getResume() {#getResume--}
```
public final Date getResume()
```


Gets a value of Resume.

**Returns:**
java.util.Date - a value of Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Gets a value of SV.

**Returns:**
double - a value of SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Gets a value of Start.

**Returns:**
java.util.Date - a value of Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Gets a value of StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Gets a value of Stop.

**Returns:**
java.util.Date - a value of Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Gets a value indicating whether Summary is set or not.

**Returns:**
boolean - a value indicating whether Summary is set or not.
### getTask() {#getTask--}
```
public final Task getTask()
```


The task to which a resource is assigned.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with the instances of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Returns the instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing instances of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | byte | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Gets amount of timephased work for the specified date time interval.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start of the date time interval. |
| end | java.util.Date | End of the date time interval. |

**Returns:**
double - amount of timephased work for the specified date time interval.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Gets amount of timephased work for the specified date time interval.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start of the date time interval. |
| end | java.util.Date | End of the date time interval. |
| timephasedDataType | byte | Type of the timephased data to use. |

**Returns:**
double - amount of timephased work for the specified date time interval.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets a value of Uid.

**Returns:**
int - a value of Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Gets a value of Units.

**Returns:**
double - a value of Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Gets a value indicating whether UpdateNeeded is set or not.

**Returns:**
boolean - a value indicating whether UpdateNeeded is set or not.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Gets a value of VAC.

**Returns:**
double - a value of VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Gets a value of Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Gets a value of WorkContour.

**Returns:**
int - a value of WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Gets a value of WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Gets a value indicating that this resource assignment has children.

**Returns:**
boolean - Always false.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Gets a value indicating whether HasFixedRateUnits is set or not.

**Returns:**
boolean - a value indicating whether HasFixedRateUnits is set or not.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class.

**Returns:**
int - returns a hash code value for this object.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Generates a list of time phased data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The specified start date. |
| time | double | The specified working time. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | The specified working calendar. |
| list | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | The list of time phased data. |
| isWorking | boolean | The specified flag which specifies whether time-phased data is working or not. |
| type | int | The specified time-phased data type. |

**Returns:**
java.util.Date - A maximum date from list or start date if list is empty.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Sets a value of ACWP.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Sets a value of ActualCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Sets a value of ActualFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ActualFinish. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Sets a value of ActualStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ActualStart. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Sets a value indicating whether Confirmed is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Confirmed is set or not. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sets a value of Cost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Sets a value of CostRateTableType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CostRateTableType. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Sets a value of Delay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Sets an instance of the ExtendedAttributeCollection class for this object.

--------------------

Reading supported for XML format only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | an instance of the ExtendedAttributeCollection class for this object. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sets a value of Finish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Sets a value of FinishVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Sets a value indicating whether FixedMaterial is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether FixedMaterial is set or not. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Sets a value indicating whether HasFixedRateUnits is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether HasFixedRateUnits is set or not. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets unique identifier for this assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | unique identifier for this assignment. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Sets a value of Hyperlink.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Sets a value of HyperlinkAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Sets a value of HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Sets a value of LevelingDelay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Sets a value indicating whether LinkedFields is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether LinkedFields is set or not. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Sets units for assignment of a material resource with variable material consumption. The variable material consumption means that as the assignment duration changes, the quantity of materials used changes proportionally.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| units | double | Number of units accrued at the time period. |
| rateScaleType | int | Time period at which the unit value is accrued.

--------------------

For example, to set '123/month', SetUnitsScaled(123D, RateScaleType.Month) should be called. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Sets a value indicating whether Milestone is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Milestone is set or not. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Sets the text notes in RTF format.

--------------------

Supported for MPP formats only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the text notes in RTF format. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Sets notes' plain text extracted from RTF data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | notes' plain text extracted from RTF data. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Sets a value indicating whether Overallocated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Overallocated is set or not. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Sets a value of OvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of OvertimeCost. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Sets a value of RateScale.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of RateScale. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


The resource assigned to a task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | the resource assigned to a task. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Sets a value indicating whether ResponsePending is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ResponsePending is set or not. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Sets a value of Resume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Sets a value of SV.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Sets a value of Start.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Sets a value of StartVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Sets a value of Stop.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Sets a value indicating whether Summary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Summary is set or not. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


The task to which a resource is assigned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | the task to which a resource is assigned. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Sets a value of Units.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Sets a value indicating whether UpdateNeeded is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether UpdateNeeded is set or not. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Sets a value of VAC.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Sets a value of Work.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Sets a value of WorkContour.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Sets a value of WorkVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Splits task into two parts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The beginning of work interruption to split based on. |
| finish | java.util.Date | The end of work interruption to split based on. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | The calendar to split based on. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Generates list of time phased data based on the task duration and the scheduled start date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | The calendar to generate time phased data from. |

### toString() {#toString--}
```
public String toString()
```


Returns short string representation of the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents assignment object.
