---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置非工作时间的颜色"
type: docs
weight: 110
url: /zh/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

获取或设置非工作时间的颜色。

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## 示例

展示如何为非工作时间设置自定义颜色。

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


