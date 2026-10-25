---
title: "类 PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PrimaveraXmlSaveOptions 类。允许在将项目保存为 Primavera XML 格式时指定其他选项"
type: docs
weight: 2160
url: /zh/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

允许在将项目保存为 Primavera XML 格式时指定附加选项。

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | 初始化 `PrimaveraXmlSaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | 获取或设置一个值，指示是否保存根任务。 |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | 获取或设置一个值，指示在导出期间是否应跳过资源对汇总任务的分配。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |

## 示例

展示如何导出到 Primavera XML 文件。

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### 另见

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


