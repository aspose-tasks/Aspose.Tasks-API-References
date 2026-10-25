---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目保存为 Primavera XER 格式时指定附加选项。"
type: docs
weight: 208
url: /zh/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

允许在将项目保存为 Primavera XER 格式时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | 初始化一个新的 [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | 获取在活动 ID 重编号中使用的增量。 |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | 获取在活动 ID 重编号中使用的前缀。 |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | 获取在活动 ID 重编号中使用的后缀。 |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | 获取一个值，指示是否需要重新编号活动 ID。 |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | 获取一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。 |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | 设置在活动 ID 重编号中使用的增量。 |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | 设置在活动 ID 重编号中使用的前缀。 |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | 设置在活动 ID 重编号中使用的后缀。 |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | 设置一个值，指示是否需要重新编号活动 ID。 |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | 设置一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。 |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


初始化一个新的 [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) 类实例。

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


获取在活动 ID 重编号中使用的增量。

**Returns:**
int - 在活动 ID 重编号中使用的增量。
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


获取在活动 ID 重编号中使用的前缀。

**Returns:**
java.lang.String - 在活动 ID 重编号中使用的前缀。
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


获取在活动 ID 重编号中使用的后缀。

**Returns:**
int - 在活动 ID 重编号中使用的后缀。
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


获取一个值，指示是否需要重新编号活动 ID。

**Returns:**
boolean - 指示是否需要重新编号活动 ID 的值。
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


获取一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。

Primavera 软件不支持将资源分配给汇总（WBS）任务。因此，根据 Primavera 的模型，此类分配的导出可能导致文件无效。如果为 true，则在导出时会跳过对汇总任务的分配。如果为 false（默认值），在导出时遇到对汇总任务的分配将抛出异常。

**Returns:**
boolean - 指示在导出时是否应跳过资源分配到汇总任务的值。
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


设置在活动 ID 重编号中使用的增量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在活动 ID 重编号中使用的增量。 |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


设置在活动 ID 重编号中使用的前缀。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 在活动 ID 重编号中使用的前缀。 |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


设置在活动 ID 重编号中使用的后缀。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在活动 ID 重编号中使用的后缀。 |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


设置一个值，指示是否需要重新编号活动 ID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否需要重新编号活动 ID 的值。 |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


设置一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。

Primavera 软件不支持将资源分配给汇总（WBS）任务。因此，根据 Primavera 的模型，此类分配的导出可能导致文件无效。如果为 true，则在导出时会跳过对汇总任务的分配。如果为 false（默认值），在导出时遇到对汇总任务的分配将抛出异常。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在导出时是否应跳过资源分配到汇总任务的值。 |

