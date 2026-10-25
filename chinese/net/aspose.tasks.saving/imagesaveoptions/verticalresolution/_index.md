---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置以 dpi 为单位的垂直分辨率。"
type: docs
weight: 100
url: /zh/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

获取或设置垂直分辨率（dpi）。

```csharp
public float VerticalResolution { get; set; }
```

## 示例

展示如何设置在转换为图像格式期间使用的像素格式。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### 另见

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


