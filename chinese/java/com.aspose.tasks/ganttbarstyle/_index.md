---
title: "GanttBarStyle"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示 MSP 在甘特图视图中使用的条形样式。"
type: docs
weight: 109
url: /zh/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

表示 MSP 在甘特图视图中使用的条形样式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | 初始化 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | 获取用户定义的转换器，以获取在任务栏底部渲染的文本。 |
| [getBottomField()](#getBottomField--) | 获取显示在栏底部的数据。 |
| [getEndShape()](#getEndShape--) | 获取栏的结束形状。 |
| [getEndShapeColor()](#getEndShapeColor--) | 获取结束形状的颜色。 |
| [getEndShapeType()](#getEndShapeType--) | 获取结束形状的类型。 |
| [getFrom()](#getFrom--) | 获取甘特栏的起始点位置。 |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | 获取用户定义的转换器，以获取在任务栏内部渲染的文本。 |
| [getInsideField()](#getInsideField--) | 获取显示在栏内部的数据。 |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | 获取用户定义的转换器，以获取在任务栏左侧渲染的文本。 |
| [getLeftField()](#getLeftField--) | 获取显示在栏左侧的数据。 |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | 获取甘特栏的填充图案。 |
| [getMiddleShape()](#getMiddleShape--) | 获取栏的中间形状。 |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | 获取中间形状的颜色。 |
| [getName()](#getName--) | 获取样式的名称。 |
| [getParentStyle()](#getParentStyle--) | 获取自定义任务特定样式的父（或通用）样式。 |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | 获取用户定义的转换器，以获取在任务栏右侧渲染的文本。 |
| [getRightField()](#getRightField--) | 获取显示在栏右侧的数据。 |
| [getRow()](#getRow--) | 获取行号。 |
| [getShowForCategories()](#getShowForCategories--) | 获取样式应用的任务类别。 |
| [getShowForTaskUid()](#getShowForTaskUid--) | 获取样式应用的任务的唯一标识符。 |
| [getStartShape()](#getStartShape--) | 获取栏的起始形状。 |
| [getStartShapeColor()](#getStartShapeColor--) | 获取起始形状的颜色。 |
| [getStartShapeType()](#getStartShapeType--) | 获取起始形状的类型。 |
| [getTo()](#getTo--) | 获取甘特条的结束点位置。 |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | 获取用户定义的转换器，以获取在任务条顶部渲染的文本。 |
| [getTopField()](#getTopField--) | 获取显示在条顶部的数据。 |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | 设置用户定义的转换器，以获取在任务条底部渲染的文本。 |
| [setBottomField(int value)](#setBottomField-int-) | 设置显示在条底部的数据。 |
| [setEndShape(int value)](#setEndShape-int-) | 设置条的结束形状。 |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | 设置结束形状的颜色。 |
| [setEndShapeType(int value)](#setEndShapeType-int-) | 设置结束形状的类型。 |
| [setFrom(int value)](#setFrom-int-) | 设置甘特条的起始点位置。 |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | 设置用户定义的转换器，以获取在任务条内部渲染的文本。 |
| [setInsideField(int value)](#setInsideField-int-) | 设置显示在条内部的数据。 |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | 设置用户定义的转换器，以获取在任务条左侧渲染的文本。 |
| [setLeftField(int value)](#setLeftField-int-) | 设置显示在条左侧的数据。 |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | 设置甘特条的填充图案。 |
| [setMiddleShape(int value)](#setMiddleShape-int-) | 设置条的中间形状。 |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | 设置中间形状的颜色。 |
| [setName(String value)](#setName-java.lang.String-) | 设置样式的名称。 |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | 设置自定义任务特定样式的父（或通用）样式。 |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | 设置用户定义的转换器，以获取在任务条右侧渲染的文本。 |
| [setRightField(int value)](#setRightField-int-) | 设置显示在条右侧的数据。 |
| [setRow(int value)](#setRow-int-) | 设置行号。 |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | 设置样式适用的任务类别。 |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | 设置样式适用的任务的唯一标识。 |
| [setStartShape(int value)](#setStartShape-int-) | 设置条形的起始形状。 |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | 设置起始形状的颜色。 |
| [setStartShapeType(int value)](#setStartShapeType-int-) | 设置起始形状的类型。 |
| [setTo(int value)](#setTo-int-) | 设置甘特条的结束点位置。 |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | 设置用户定义的转换器，以获取在任务条顶部渲染的文本。 |
| [setTopField(int value)](#setTopField-int-) | 设置显示在条形顶部的数据。 |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


初始化 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) 类的新实例。

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


获取用户定义的转换器，以获取在任务条底部渲染的文本。覆盖 `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


获取显示在条形底部的数据。 [Field](../../com.aspose.tasks/field)。

**Returns:**
int - 显示在条形底部的数据。
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


获取栏的结束形状。

**Returns:**
int - 条形的结束形状。
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


获取结束形状的颜色。

**Returns:**
java.awt.Color - 结束形状的颜色。
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


获取结束形状的类型。 [GanttBarType](../../com.aspose.tasks/ganttbartype)。

**Returns:**
int - 结束形状的类型。
### getFrom() {#getFrom--}
```
public final int getFrom()
```


获取甘特条的起始点位置。 [Field](../../com.aspose.tasks/field)。

**Returns:**
int - 甘特条的起始点位置。
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


获取用户定义的转换器，以获取在任务条内部渲染的文本。覆盖 `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


获取显示在条形内部的数据。 [Field](../../com.aspose.tasks/field)。

**Returns:**
int - 显示在条形内部的数据。
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


获取用户定义的转换器，以获取在任务条左侧渲染的文本。覆盖 `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


获取显示在条形左侧的数据。 [Field](../../com.aspose.tasks/field)。

**Returns:**
int - 显示在条形左侧的数据。
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


获取甘特栏的填充图案。

**Returns:**
int - 甘特条的填充图案。
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


获取栏的中间形状。

**Returns:**
int - 条形的中间形状。
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


获取中间形状的颜色。

**Returns:**
java.awt.Color - 中间形状的颜色。
### getName() {#getName--}
```
public final String getName()
```


获取样式的名称。

**Returns:**
java.lang.String - 样式的名称。
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


获取自定义任务特定样式的父（或通用）样式。

--------------------

任务可以拥有多个具有不同父样式的自定义样式。例如，考虑任务具有一个父样式为 "Critical" 的自定义样式和另一个父样式为 "Normal" 的样式。简而言之，如果任务是关键的，则应用第一个样式；如果任务变为非关键的，则应用第二个样式（此逻辑继承自 Microsoft Project Professional）。

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


获取用户定义的转换器，以获取在任务条右侧渲染的文本。覆盖 `RightField`([getRightField()](../../com.aspose/tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose/tasks/ganttbarstyle\#setRightField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


获取显示在条右侧的数据。 [Field](../../com.aspose/tasks/field)。

**Returns:**
int - 显示在条右侧的数据。
### getRow() {#getRow--}
```
public final int getRow()
```


获取行号。

--------------------

可以是 1 到 4（1 为默认值）。

**Returns:**
int - 行号。
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


获取样式适用的任务类别。适用于甘特图中条的父（或通用）样式（参见 `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose/tasks/ganttchartview\#getBarStyles--))）。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 样式适用的任务类别。
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


获取样式适用的任务的唯一标识。适用于甘特图中条的特定任务样式（参见 `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose/tasks/ganttchartview\#getCustomBarStyles--))）。

**Returns:**
java.lang.Integer - 样式适用的任务的唯一标识。
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


获取栏的起始形状。

**Returns:**
int - 条的起始形状。
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


获取起始形状的颜色。

**Returns:**
java.awt.Color - 起始形状的颜色。
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


获取起始形状的类型。

**Returns:**
int - 起始形状的类型。
### getTo() {#getTo--}
```
public final int getTo()
```


获取甘特条的结束点位置。

**Returns:**
int - 甘特条的结束点位置。
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


获取用户定义的转换器，以获取在任务条顶部渲染的文本。覆盖 `TopField`([getTopField()](../../com.aspose/tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose/tasks/ganttbarstyle\#setTopField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


获取显示在条顶部的数据。

**Returns:**
int - 显示在条顶部的数据。
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


设置用户定义的转换器，以获取在任务条底部渲染的文本。覆盖 `BottomField`([getBottomField()](../../com.aspose/tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose/tasks/ganttbarstyle\#setBottomField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | 用户定义的转换器，以获取在任务条底部渲染的文本。 |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


设置显示在条底部的数据。 [Field](../../com.aspose/tasks/field)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 显示在条底部的数据。 |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


设置条的结束形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 条的结束形状。 |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


设置结束形状的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 结束形状的颜色。 |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


设置结束形状的类型。 [GanttBarType](../../com.aspose/tasks/ganttbartype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 结束形状的类型。 |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


设置甘特条的起始点位置。 [Field](../../com.aspose.tasks/field)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 甘特条的起始点位置。 |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


设置用户定义的转换器以获取在任务条内部渲染的文本。覆盖 `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | 用户定义的转换器以获取在任务条内部渲染的文本。 |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


设置在条内部显示的数据。 [Field](../../com.aspose.tasks/field)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在条内部显示的数据。 |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


设置用户定义的转换器以获取在任务条左侧渲染的文本。覆盖 `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | 用户定义的转换器以获取在任务条左侧渲染的文本。 |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


设置在条左侧显示的数据。 [Field](../../com.aspose.tasks/field)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在条左侧显示的数据。 |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


设置甘特条的填充图案。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 甘特条的填充图案。 |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


设置条的中间形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 条的中间形状。 |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


设置中间形状的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 中间形状的颜色。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置样式的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 样式的名称。 |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


设置自定义任务特定样式的父（或通用）样式。

--------------------

任务可以拥有多个具有不同父样式的自定义样式。例如，考虑任务具有一个父样式为 "Critical" 的自定义样式和另一个父样式为 "Normal" 的样式。简而言之，如果任务是关键的，则应用第一个样式；如果任务变为非关键的，则应用第二个样式（此逻辑继承自 Microsoft Project Professional）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | 自定义任务特定样式的父（或通用）样式。 |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


设置用户定义的转换器以获取在任务条右侧渲染的文本。覆盖 `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | 用户定义的转换器以获取在任务条右侧渲染的文本。 |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


设置在条右侧显示的数据。 [Field](../../com.aspose.tasks/field)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在条右侧显示的数据。 |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


设置行号。

--------------------

可以是 1 到 4（1 为默认值）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 行号。 |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


设置样式适用的任务类别。适用于甘特图中条的父（或通用）样式（参见 `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;java.lang.Integer&gt; | 样式适用的任务类别。 |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


设置样式适用的任务的唯一标识。适用于甘特图中条的任务特定样式（参见 `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Integer | 样式适用的任务的唯一标识。 |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


设置条形的起始形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 条的起始形状。 |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


设置起始形状的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 起始形状的颜色。 |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


设置起始形状的类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 起始形状的类型。 |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


设置甘特条的结束点位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 甘特条的结束点位置。 |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


设置用户定义的转换器以获取在任务栏顶部渲染的文本。覆盖 `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) 属性的值。

--------------------

不会持久化到 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | 用于获取在任务栏顶部渲染的文本的用户定义转换器。 |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


设置显示在条形顶部的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 显示在条形顶部的数据。 |

