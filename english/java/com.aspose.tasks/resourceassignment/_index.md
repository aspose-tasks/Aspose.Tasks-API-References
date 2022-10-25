---
title: ResourceAssignment
second_title: Aspose.Tasks for Java API Reference
description: Represents a resource assignment in a project.
type: docs
weight: 225
url: /java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent
```
public class ResourceAssignment extends IContainer<Integer> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent
```

Represents a resource assignment in a project.
## Methods

| Method | Description |
| --- | --- |
| [delete()](#delete--) | Deletes resource assignment from project assignments collection. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Returns a value indicating whether this instance is equal to a specified instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [&lt;T&gt;get(Key&lt;T,Integer&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--) | Returns the value to which the property is mapped in this container. |
| [getBaselines()](#getBaselines--) | Gets AssignmentBaselineCollection object. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets an instance of the ExtendedAttributeCollection class for this object. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Sets an instance of the ExtendedAttributeCollection class for this object. |
| [getGuid()](#getGuid--) | Gets unique identifier for this assignment. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Sets unique identifier for this assignment. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Gets parent project for this assignment. |
| [getResource()](#getResource--) | The resource assigned to a task. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | The resource assigned to a task. |
| [getTask()](#getTask--) | The task to which a resource is assigned. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | The task to which a resource is assigned. |
| [getTimephasedData()](#getTimephasedData--) | Gets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class. |
| [getTimephasedData(Date start, Date end, int timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-int-) | Returns the instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing instances of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with the instances of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [hasChildren()](#hasChildren--) | Gets a value indicating that this resource assignment has children. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Generates a list of time phased data. |
| [&lt;T&gt;set(Key&lt;T,Integer&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-) | Maps the specified property to the specified value in this container. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Splits task into two parts. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Generates list of time phased data based on the task duration and the scheduled start date. |
| [toString()](#toString--) | Returns short string representation of the instance of the [ResourceAssignment](../../com.aspose.tasks/resourceassignment) class. |
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
### &lt;T&gt;get(Key&lt;T,Integer&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--}
```
public final T <T>get(Key<T,Integer> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Asn](../../com.aspose.tasks/asn) for getting the property key.

 T : the type of the mapped value. |

**Returns:**
T - the value to which the property is mapped in this container.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


Gets AssignmentBaselineCollection object. The collection of baseline values associated with an assignment.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets an instance of the ExtendedAttributeCollection class for this object.

--------------------

Reading supported for XML format only.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
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

### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Gets unique identifier for this assignment.

**Returns:**
java.util.UUID - unique identifier for this assignment.
### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets unique identifier for this assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | unique identifier for this assignment. |

### getItems() {#getItems--}
```
public final System.Collections.Generic.IGenericEnumerable<IExtendedAttributeParent> getItems()
```


Reserved for internal usage.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets parent project for this assignment.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getResource() {#getResource--}
```
public final Resource getResource()
```


The resource assigned to a task.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


The resource assigned to a task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | the resource assigned to a task. |

### getTask() {#getTask--}
```
public final Task getTask()
```


The task to which a resource is assigned.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


The task to which a resource is assigned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | the task to which a resource is assigned. |

### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class.
### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class. |

### getTimephasedData(Date start, Date end, int timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-int-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, int timephasedType)
```


Returns the instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing instances of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | int | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with the instances of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) class within given start and end dates of [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Gets a value indicating that this resource assignment has children.

**Returns:**
boolean - Always false.
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
### &lt;T&gt;set(Key&lt;T,Integer&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-}
```
public final void <T>set(Key<T,Integer> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Asn](../../com.aspose.tasks/asn) for getting the property key. |
| val | T | the value.

 T : the type of the mapped value. |

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
