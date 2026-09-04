---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示从 Primavera 格式加载的项目的简要信息。"
type: docs
weight: 204
url: /zh/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

表示从 Primavera 格式加载的项目的简要信息。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | 获取项目的导出标志。 |
| [getName()](#getName--) | 获取项目的名称。 |
| [getShortName()](#getShortName--) | 获取项目的短名称（项目 ID）。 |
| [getUid()](#getUid--) | 获取项目的 Uid。 |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


获取项目的导出标志。当在 Primavera 中选择项目进行导出时，其 ExportFlag 为 true。某些未明确选择导出的项目可能由于与已导出项目的关联而被导出到 XER 文件。

**Returns:**
boolean - 项目的导出标志。
### getName() {#getName--}
```
public final String getName()
```


获取项目的名称。

**Returns:**
java.lang.String - 项目的名称。
### getShortName() {#getShortName--}
```
public final String getShortName()
```


获取项目的短名称（项目 ID）。

**Returns:**
java.lang.String - 项目的短名称（项目 ID）。
### getUid() {#getUid--}
```
public final int getUid()
```


获取项目的 Uid。

**Returns:**
int - 项目的 Uid。
