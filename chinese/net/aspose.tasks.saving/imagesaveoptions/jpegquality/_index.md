---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置 JPEG 质量。允许的取值范围是 0..100"
type: docs
weight: 40
url: /zh/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

获取或设置 JPEG 质量。允许的取值范围是 0..100。

```csharp
public int JpegQuality { get; set; }
```

## 示例

展示如何设置输出 JPEG 文件的 JPEG 质量。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// 为了操作 JPEG 质量，可以使用 ImageSaveOptions.JpegQuality 属性。
// 允许的取值范围是 0..100。
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### 另见

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


