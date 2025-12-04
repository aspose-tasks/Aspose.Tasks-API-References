---
title: ResourceViewColumn
second_title: Aspose.Tasks for Java API Reference
description: Projects view class used in ResourceUsage view and ResourceSheet view.
type: docs
weight: 260
url: /java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Project's view class used in ResourceUsage view and ResourceSheet view.
## Constructors

| Constructor | Description |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class. |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class. |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class. |
## Methods

| Method | Description |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Converts current resource to the column text. |
| [getField()](#getField--) | Returns column field. |
| [setField(int value)](#setField-int-) | Sets column field. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column's name. |
| width | int | Column's width in pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resource data to column text converter. |
| field | int | Column field. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column's name. |
| width | int | Column's width in pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resource data to column text converter. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Initializes a new instance of the [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | int | Column width in pixels. |
| field | int | Column field. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Converts current resource to the column text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Current resource. |

**Returns:**
java.lang.String - The column text.
### getField() {#getField--}
```
public int getField()
```


Returns column field. `Field`.

**Returns:**
int - column field value.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Sets column field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | column field value. |

