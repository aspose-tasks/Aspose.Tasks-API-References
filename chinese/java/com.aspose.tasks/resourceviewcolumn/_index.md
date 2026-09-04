---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API 参考"
description: "在 ResourceUsage 视图和 ResourceSheet 视图中使用的 Projects 视图类。"
type: docs
weight: 261
url: /zh/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

项目视图类，用于 ResourceUsage 视图和 ResourceSheet 视图。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | 初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。 |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | 初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。 |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | 初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | 将当前资源转换为列文本。 |
| [getField()](#getField--) | 返回列字段。 |
| [setField(int value)](#setField-int-) | 设置列字段。 |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列的名称。 |
| width | int | 列的宽度（像素）。 |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | 资源数据到列文本的转换器。 |
| 字段 | int | 列字段。 |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列的名称。 |
| width | int | 列的宽度（像素）。 |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | 资源数据到列文本的转换器。 |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


初始化 [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| width | int | 列宽（像素）。 |
| 字段 | int | 列字段。 |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


将当前资源转换为列文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | 当前资源。 |

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

