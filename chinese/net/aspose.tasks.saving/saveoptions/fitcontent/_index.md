---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一个值，指示是否应增加行高以适应其内容。"
type: docs
weight: 50
url: /zh/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

获取或设置一个值，指示是否应增加行高以适应其内容。

```csharp
public bool FitContent { get; set; }
```

## 示例

展示如何设置行高是否应增加以适应其内容的选项。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // 将“适应内容”选项设为 true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


