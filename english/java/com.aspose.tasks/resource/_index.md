---
title: Resource
second_title: Aspose.Tasks for Java API Reference
description: Represents a resource in a project.
type: docs
weight: 224
url: /java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent
```
public class Resource extends IContainer<Integer> implements System.IEquatable<Resource>, IExtendedAttributeParent
```

Represents a resource in a project.
## Methods

| Method | Description |
| --- | --- |
| [delete()](#delete--) | Deletes a resource and its assignments from project. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Returns a value indicating whether this instance is equal to a specified instance of the [Resource](../../com.aspose.tasks/resource) class. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [&lt;T&gt;get(Key&lt;T,Integer&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--) | Returns the value to which the property is mapped in this container. |
| [getAssignments()](#getAssignments--) | Gets a collection of resource assignments for this object. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Gets a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class. |
| [getBaselines()](#getBaselines--) | Gets a BaselineCollection instance for this object. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets the values of an extended attribute. |
| [getItems()](#getItems--) | Gets child resources. |
| [getOutlineCode()](#getOutlineCode--) | Gets an OutlineCodeCollection object. |
| [getParentProject()](#getParentProject--) | Gets parent project for this container. |
| [getRates()](#getRates--) | Gets a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object. |
| [getTimephasedData()](#getTimephasedData--) | Gets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object. |
| [getTimephasedData(Date start, Date end, int timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-int-) | Returns an instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object with the  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) for this object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-))values within given start and end dates. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [Resource](../../com.aspose.tasks/resource) class. |
| [isRoot()](#isRoot--) | Gets the flag indicating whether resource is a root resource. |
| [&lt;T&gt;set(Key&lt;T,Integer&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-) | Maps the specified property to the specified value in this container. |
| [set(Key&lt;Date,Integer&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-) | Maps the specified property to the specified value in this container. |
| [toString()](#toString--) | Returns short string representation of the instance of the [Resource](../../com.aspose.tasks/resource) class. |
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
### &lt;T&gt;get(Key&lt;T,Integer&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--}
```
public final T <T>get(Key<T,Integer> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key.

 T : the type of the mapped value. |

**Returns:**
T - the value to which the property is mapped in this container.
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
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Gets a BaselineCollection instance for this object. The baseline values for a resource.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets the values of an extended attribute.

--------------------

Two pieces of data are necessary - a pointer back to the extended attribute table which is specified either by the unique ID or the Field ID, and the value which is specified either with the value, or a pointer back to the value list.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getItems() {#getItems--}
```
public final System.Collections.Generic.IGenericEnumerable<IExtendedAttributeParent> getItems()
```


Gets child resources.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - child resources.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Gets an OutlineCodeCollection object. The value of an outline code.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets parent project for this container.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Gets a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object. The collection of periods and rates associated with each one.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.

--------------------

Reading supported for XML format only.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
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

### getTimephasedData(Date start, Date end, int timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-int-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, int timephasedType)
```


Returns an instance of the [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object with the  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | int | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) for this object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-))values within given start and end dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the timephased data. |
| end | java.util.Date | The end date for the timephased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
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
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Gets the flag indicating whether resource is a root resource. Root resource is a special resource which is intended to support internals of MS Project's formats and is not intended to be used directly from the user's code.

**Returns:**
boolean - the flag indicating whether resource is a root resource.
### &lt;T&gt;set(Key&lt;T,Integer&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-}
```
public void <T>set(Key<T,Integer> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key. |
| val | T | the value. |

### set(Key&lt;Date,Integer&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-}
```
public final void set(Key<Date,Integer> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Integer&gt; | the specified property key. [Rsc](../../com.aspose.tasks/rsc) for getting the property key. |
| val | java.util.Date | the value. |

### toString() {#toString--}
```
public String toString()
```


Returns short string representation of the instance of the [Resource](../../com.aspose.tasks/resource) class. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents resource object.
