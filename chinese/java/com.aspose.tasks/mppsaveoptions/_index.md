---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目数据保存为 MPP 时指定其他选项。"
type: docs
weight: 149
url: /zh/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

允许在将项目数据保存为 MPP 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | 初始化 [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getClearVba()](#getClearVba--) | 获取一个值，指示在将项目保存为 MPP 格式时是否移除现有的 VBA 宏数据。 |
| [getProtectionPassword()](#getProtectionPassword--) | 获取用于保护生成的 MPP 文件的密码。 |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | 获取一个值，指示在保存为 MPP 时是否移除无效的资源分配。 |
| [getWriteFilters()](#getWriteFilters--) | 获取一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。 |
| [getWriteGroups()](#getWriteGroups--) | 获取一个值，指示在将项目保存为 MPP 格式时是否写入组数据。 |
| [getWriteVba()](#getWriteVba--) | 获取一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。 |
| [getWriteViewData()](#getWriteViewData--) | 获取一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。 |
| [setClearVba(boolean value)](#setClearVba-boolean-) | 设置一个值，指示在将项目保存为 MPP 格式时是否移除现有的 VBA 宏数据。 |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | 设置用于保护生成的 MPP 文件的密码。 |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | 设置一个值，指示在保存为 MPP 时是否移除无效的资源分配。 |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | 设置一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。 |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | 设置一个值，指示在将项目保存为 MPP 格式时是否写入组数据。 |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | 设置一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。 |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | 设置一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。 |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


初始化 [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) 类的新实例。

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


获取一个值，指示在将项目保存为 MPP 格式时是否移除现有的 VBA 宏数据。

**Returns:**
boolean - 一个值，指示在将项目保存为 MPP 格式时是否删除现有的 VBA 宏数据。
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


获取用于保护生成的 MPP 文件的密码。目前支持 MS Project 2010 及更高版本的格式。

--------------------

空值表示项目文件未受保护。

**Returns:**
java.lang.String - 用于保护生成的 MPP 文件的密码。
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


获取一个值，指示在保存为 MPP 时是否移除无效的资源分配。

--------------------

MS Project 为每个任务创建一个空的资源分配。将此标志设为 true 可在保存时将其删除。

**Returns:**
boolean - 一个值，指示在保存为 MPP 时是否删除无效的资源分配。
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


获取一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。

--------------------

过滤器数据包括 Project.TaskFilters 和 Project.ResourceFilters 集合。

--------------------

目前支持 MSP 2010 或更高版本的格式。

**Returns:**
boolean - 一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


获取一个值，指示在将项目保存为 MPP 格式时是否写入组数据。

--------------------

分组数据包括 Project.TaskGroups 和 Project.ResourceGroups 集合。

**Returns:**
boolean - 一个值，指示在将项目保存为 MPP 格式时是否写入分组数据。
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


获取一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。目前支持写入 VbaModule.SourceCode。

**Returns:**
boolean - 一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


获取一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。

--------------------

视图数据包括 Project.Views、Filters 和 Tables 集合。

**Returns:**
boolean - 一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


设置一个值，指示在将项目保存为 MPP 格式时是否移除现有的 VBA 宏数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示在将项目保存为 MPP 格式时是否删除现有的 VBA 宏数据。 |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


设置用于保护生成的 MPP 文件的密码。目前支持 MS Project 2010 及更高版本的格式。

--------------------

空值表示项目文件未受保护。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于保护生成的 MPP 文件的密码。 |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


设置一个值，指示在保存为 MPP 时是否移除无效的资源分配。

--------------------

MS Project 为每个任务创建一个空的资源分配。将此标志设为 true 可在保存时将其删除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示在保存为 MPP 时是否删除无效的资源分配。 |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


设置一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。

--------------------

过滤器数据包括 Project.TaskFilters 和 Project.ResourceFilters 集合。

--------------------

目前支持 MSP 2010 或更高版本的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。 |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


设置一个值，指示在将项目保存为 MPP 格式时是否写入组数据。

--------------------

分组数据包括 Project.TaskGroups 和 Project.ResourceGroups 集合。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示在将项目保存为 MPP 格式时是否写入分组数据。 |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


设置一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。目前支持写入 VbaModule.SourceCode。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。 |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


设置一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。

--------------------

视图数据包括 Project.Views、Filters 和 Tables 集合。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。 |

