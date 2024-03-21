---
title: AssignmentViewColumn
second_title: Aspose.Tasks for Java API Reference
description: Projects view class.
type: docs
weight: 19
url: /java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Project's view class.
## Constructors

| Constructor | Description |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Initializes a new instance of the AssignmentViewColumn class. |
## Methods

| Method | Description |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Converts current resource assignment to the column text. |
| [getField()](#getField--) | Returns column field. |
| [setField(int value)](#setField-int-) | Sets column field. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Initializes a new instance of the AssignmentViewColumn class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column's name. |
| width | int | Column's width in pixels. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Assignment data to column text converter. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Converts current resource assignment to the column text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Current assignment. |

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

