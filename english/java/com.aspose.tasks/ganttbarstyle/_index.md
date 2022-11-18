---
title: GanttBarStyle
second_title: Aspose.Tasks for Java API Reference
description: Represents a bar style used by MSP in Gantt Chart view.
type: docs
weight: 108
url: /java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Represents a bar style used by MSP in Gantt Chart view.
## Constructors

| Constructor | Description |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | Initializes a new instance of the [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) class. |
## Methods

| Method | Description |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Gets user-defined converter to get text to render on the bottom of the task's bar. |
| [getBottomField()](#getBottomField--) | Gets data to be displayed on the bottom of the bar. |
| [getEndShape()](#getEndShape--) | Gets an end shape of the bar. |
| [getEndShapeColor()](#getEndShapeColor--) | Gets a color of the end shape. |
| [getEndShapeType()](#getEndShapeType--) | Gets a type of the end shape. |
| [getFrom()](#getFrom--) | Gets a start point position of the gantt bar. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Gets user-defined converter to get text to render inside of the task's bar. |
| [getInsideField()](#getInsideField--) | Gets data to be displayed inside of the bar. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Gets user-defined converter to get text to render on the left of the task's bar. |
| [getLeftField()](#getLeftField--) | Gets data to be displayed on the left of the bar. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Gets a fill pattern of the gantt bar. |
| [getMiddleShape()](#getMiddleShape--) | Gets a middle shape of the bar. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Gets a color of the middle shape. |
| [getName()](#getName--) | Gets a name of the style. |
| [getParentStyle()](#getParentStyle--) | Gets parent (or common) style for custom task-specific style. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Gets user-defined converter to get text to render on the right of the task's bar. |
| [getRightField()](#getRightField--) | Gets data to be displayed on the right of the bar. |
| [getRow()](#getRow--) | Gets a row number. |
| [getShowForCategories()](#getShowForCategories--) | Gets task categories for which the style is applied. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Gets Unique Id of a task for which the style is applied. |
| [getStartShape()](#getStartShape--) | Gets a start shape of the bar. |
| [getStartShapeColor()](#getStartShapeColor--) | Gets a color of the start shape. |
| [getStartShapeType()](#getStartShapeType--) | Gets a type of the start shape. |
| [getTo()](#getTo--) | Gets a finish point position of the gantt bar. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Gets user-defined converter to get text to render on the top of the task's bar. |
| [getTopField()](#getTopField--) | Gets data to be displayed on the top of the bar. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Sets user-defined converter to get text to render on the bottom of the task's bar. |
| [setBottomField(int value)](#setBottomField-int-) | Sets data to be displayed on the bottom of the bar. |
| [setEndShape(int value)](#setEndShape-int-) | Sets an end shape of the bar. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Sets a color of the end shape. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Sets a type of the end shape. |
| [setFrom(int value)](#setFrom-int-) | Sets a start point position of the gantt bar. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Sets user-defined converter to get text to render inside of the task's bar. |
| [setInsideField(int value)](#setInsideField-int-) | Sets data to be displayed inside of the bar. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Sets user-defined converter to get text to render on the left of the task's bar. |
| [setLeftField(int value)](#setLeftField-int-) | Sets data to be displayed on the left of the bar. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Sets a fill pattern of the gantt bar. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Sets a middle shape of the bar. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Sets a color of the middle shape. |
| [setName(String value)](#setName-java.lang.String-) | Sets a name of the style. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Sets parent (or common) style for custom task-specific style. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Sets user-defined converter to get text to render on the right of the task's bar. |
| [setRightField(int value)](#setRightField-int-) | Sets data to be displayed on the right of the bar. |
| [setRow(int value)](#setRow-int-) | Sets a row number. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Sets task categories for which the style is applied. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Sets Unique Id of a task for which the style is applied. |
| [setStartShape(int value)](#setStartShape-int-) | Sets a start shape of the bar. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Sets a color of the start shape. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Sets a type of the start shape. |
| [setTo(int value)](#setTo-int-) | Sets a finish point position of the gantt bar. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Sets user-defined converter to get text to render on the top of the task's bar. |
| [setTopField(int value)](#setTopField-int-) | Sets data to be displayed on the top of the bar. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


Initializes a new instance of the [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) class.

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Gets user-defined converter to get text to render on the bottom of the task's bar. Overrides the value of  BottomField ([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) property.

--------------------

Is not persisted to MPP format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Gets data to be displayed on the bottom of the bar. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data to be displayed on the bottom of the bar.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Gets an end shape of the bar.

**Returns:**
int - an end shape of the bar.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Gets a color of the end shape.

**Returns:**
java.awt.Color - a color of the end shape.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Gets a type of the end shape. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - a type of the end shape.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Gets a start point position of the gantt bar. [Field](../../com.aspose.tasks/field).

**Returns:**
int - a start point position of the gantt bar.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Gets user-defined converter to get text to render inside of the task's bar. Overrides the value of  InsideField ([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) property.

--------------------

Is not persisted to MPP format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Gets data to be displayed inside of the bar. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data to be displayed inside of the bar.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Gets user-defined converter to get text to render on the left of the task's bar. Overrides the value of  LeftField ([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) property.

--------------------

Is not persisted to MPP format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Gets data to be displayed on the left of the bar. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data to be displayed on the left of the bar.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Gets a fill pattern of the gantt bar.

**Returns:**
int - a fill pattern of the gantt bar.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Gets a middle shape of the bar.

**Returns:**
int - a middle shape of the bar.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Gets a color of the middle shape.

**Returns:**
java.awt.Color - a color of the middle shape.
### getName() {#getName--}
```
public final String getName()
```


Gets a name of the style.

**Returns:**
java.lang.String - a name of the style.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Gets parent (or common) style for custom task-specific style.

--------------------

Task can have multiple custom styles with different parent styles. For example consider task having custom style with "Critical" parent style and another style with "Normal" parent style. Simply put, if task is critical, the first style is applied. If task becomes non-critical, the second style is applied (this logic is inherited from Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Gets user-defined converter to get text to render on the right of the task's bar. Overrides the value of  RightField ([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) property.

--------------------

Is not persisted to MPP format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Gets data to be displayed on the right of the bar. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data to be displayed on the right of the bar.
### getRow() {#getRow--}
```
public final int getRow()
```


Gets a row number.

--------------------

Can be from 1 to 4 (1 is default value).

**Returns:**
int - a row number.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Gets task categories for which the style is applied. Is applicable for parent (or common) styles of bars in Gantt chart (see  GanttChartView.BarStyles ([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - task categories for which the style is applied.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Gets Unique Id of a task for which the style is applied. Is applicable for task-specific styles of bars in Gantt chart (see  GanttChartView.CustomBarStyles ([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - Unique Id of a task for which the style is applied.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Gets a start shape of the bar.

**Returns:**
int - a start shape of the bar.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Gets a color of the start shape.

**Returns:**
java.awt.Color - a color of the start shape.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Gets a type of the start shape.

**Returns:**
int - a type of the start shape.
### getTo() {#getTo--}
```
public final int getTo()
```


Gets a finish point position of the gantt bar.

**Returns:**
int - a finish point position of the gantt bar.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Gets user-defined converter to get text to render on the top of the task's bar. Overrides the value of  TopField ([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) property.

--------------------

Is not persisted to MPP format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Gets data to be displayed on the top of the bar.

**Returns:**
int - data to be displayed on the top of the bar.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Sets user-defined converter to get text to render on the bottom of the task's bar. Overrides the value of  BottomField ([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) property.

--------------------

Is not persisted to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | user-defined converter to get text to render on the bottom of the task's bar. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Sets data to be displayed on the bottom of the bar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | data to be displayed on the bottom of the bar. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Sets an end shape of the bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | an end shape of the bar. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Sets a color of the end shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | a color of the end shape. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Sets a type of the end shape. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a type of the end shape. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Sets a start point position of the gantt bar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a start point position of the gantt bar. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Sets user-defined converter to get text to render inside of the task's bar. Overrides the value of  InsideField ([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) property.

--------------------

Is not persisted to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | user-defined converter to get text to render inside of the task's bar. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Sets data to be displayed inside of the bar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | data to be displayed inside of the bar. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Sets user-defined converter to get text to render on the left of the task's bar. Overrides the value of  LeftField ([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) property.

--------------------

Is not persisted to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | user-defined converter to get text to render on the left of the task's bar. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Sets data to be displayed on the left of the bar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | data to be displayed on the left of the bar. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Sets a fill pattern of the gantt bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a fill pattern of the gantt bar. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Sets a middle shape of the bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a middle shape of the bar. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Sets a color of the middle shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | a color of the middle shape. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a name of the style.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a name of the style. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Sets parent (or common) style for custom task-specific style.

--------------------

Task can have multiple custom styles with different parent styles. For example consider task having custom style with "Critical" parent style and another style with "Normal" parent style. Simply put, if task is critical, the first style is applied. If task becomes non-critical, the second style is applied (this logic is inherited from Microsoft Project Professional).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | parent (or common) style for custom task-specific style. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Sets user-defined converter to get text to render on the right of the task's bar. Overrides the value of  RightField ([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) property.

--------------------

Is not persisted to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | user-defined converter to get text to render on the right of the task's bar. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Sets data to be displayed on the right of the bar. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | data to be displayed on the right of the bar. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Sets a row number.

--------------------

Can be from 1 to 4 (1 is default value).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a row number. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Sets task categories for which the style is applied. Is applicable for parent (or common) styles of bars in Gantt chart (see  GanttChartView.BarStyles ([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;java.lang.Integer&gt; | task categories for which the style is applied. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Sets Unique Id of a task for which the style is applied. Is applicable for task-specific styles of bars in Gantt chart (see  GanttChartView.CustomBarStyles ([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Integer | Unique Id of a task for which the style is applied. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Sets a start shape of the bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a start shape of the bar. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Sets a color of the start shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | a color of the start shape. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Sets a type of the start shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a type of the start shape. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Sets a finish point position of the gantt bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a finish point position of the gantt bar. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Sets user-defined converter to get text to render on the top of the task's bar. Overrides the value of  TopField ([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) property.

--------------------

Is not persisted to MPP format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | user-defined converter to get text to render on the top of the task's bar. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Sets data to be displayed on the top of the bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | data to be displayed on the top of the bar. |

