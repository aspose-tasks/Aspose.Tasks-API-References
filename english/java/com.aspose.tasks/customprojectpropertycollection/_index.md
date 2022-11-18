---
title: CustomProjectPropertyCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of custom project properties.
type: docs
weight: 61
url: /java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Represents a collection of custom project properties.
## Constructors

| Constructor | Description |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Initializes a new instance of the [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) class. |
## Methods

| Method | Description |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Creates a new custom property. |
| [add(String name, double value)](#add-java.lang.String-double-) | Creates a new custom property. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Creates a new custom property. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Creates a new custom property. |
| [clear()](#clear--) | Clears the PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [remove(String name)](#remove-java.lang.String-) | Removes a property with the specified name from the collection. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Initializes a new instance of the [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) class.

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Creates a new custom property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the property. |
| value | boolean | The newly created property object value. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Creates a new custom property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the property. |
| value | double | The newly created property object value. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Creates a new custom property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the property. |
| value | java.lang.String | The newly created property object value. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Creates a new custom property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the property. |
| value | java.util.Date | The newly created property object value. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Clears the PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Gets a value indicating whether this collection is read-only; otherwise, false.

**Returns:**
boolean - a value indicating whether this collection is read-only; otherwise, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Removes a property with the specified name from the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |

**Returns:**
boolean - True if the element is successfully found and removed; otherwise, false.
