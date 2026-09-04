---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API 参考"
description: "项目视图类。"
type: docs
weight: 19
url: /zh/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

项目的视图类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | 初始化 AssignmentViewColumn 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | 将当前资源分配转换为列文本。 |
| [getField()](#getField--) | 返回列字段。 |
| [setField(int value)](#setField-int-) | 设置列字段。 |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


初始化 AssignmentViewColumn 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列的名称。 |
| width | int | 列的宽度（像素）。 |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | 将分配数据转换为列文本的转换器。 |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


将当前资源分配转换为列文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 当前分配。 |

**Returns:**
java.lang.String - 列文本。
### getField() {#getField--}
```
public int getField()
```


返回列字段。`Field`。

**Returns:**
int - 列字段值。
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


设置列字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 列字段值。 |

