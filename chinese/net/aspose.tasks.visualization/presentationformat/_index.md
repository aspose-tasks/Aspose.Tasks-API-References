---
title: "枚举 PresentationFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PresentationFormat 枚举。演示格式的枚举"
type: docs
weight: 3270
url: /zh/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

演示格式的枚举。

```csharp
public enum PresentationFormat
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| GanttChart | `0` | 甘特图演示格式。 |
| TaskUsage | `1` | 任务使用情况演示格式。 |
| ResourceUsage | `2` | 资源使用情况演示格式。 |
| ResourceSheet | `3` | 资源表演示格式。 |
| TaskSheet | `4` | 任务表演示格式。 |

## 示例

展示如何呈现资源表视图。

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// 将演示格式设置为资源表
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


