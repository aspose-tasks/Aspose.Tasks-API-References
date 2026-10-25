---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraXmlSaveOptions 属性。获取或设置指示在导出期间是否应跳过资源对汇总任务的分配的值"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

获取或设置一个值，指示在导出期间是否应跳过资源对汇总任务的分配。

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## 备注

Primavera 软件不支持将资源分配给汇总（WBS）任务。因此，根据 Primavera 的模型，此类分配的导出可能导致文件无效。如果为 true，则在导出期间会跳过对汇总任务的分配。如果为 false（默认值），在导出期间遇到对汇总任务的分配时将抛出异常。

## 示例

展示如何使用 SkipSummaryAssignments 标志。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera 不支持将资源分配给汇总任务。
// 因此，将此类分配导出为 Primavera 格式可能导致文件无法导入到 Primavera。
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### 另见

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


