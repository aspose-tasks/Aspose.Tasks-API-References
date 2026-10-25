---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目保存为 Primavera xml 格式时指定附加选项。"
type: docs
weight: 212
url: /zh/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

允许在将项目保存为 Primavera xml 格式时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | 初始化 [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | 获取一个值，指示是否保存根任务。 |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | 获取一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。 |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | 设置一个值，指示是否保存根任务。 |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | 设置一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。 |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


初始化 [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) 类的新实例。

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


获取一个值，指示是否保存根任务。

**Returns:**
boolean - 指示是否保存根任务的值。
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


获取一个值，指示在导出时是否应跳过资源分配到汇总任务的操作。

Primavera 软件不支持将资源分配给汇总（WBS）任务。因此，根据 Primavera 的模型，此类分配的导出可能导致文件无效。如果为 true，则在导出时会跳过对汇总任务的分配。如果为 false（默认值），在导出时遇到对汇总任务的分配将抛出异常。

**Returns:**
boolean - 指示在导出时是否应跳过资源分配到汇总任务的值。
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


设置一个值，指示是否保存根任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否保存根任务的值。 |

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

