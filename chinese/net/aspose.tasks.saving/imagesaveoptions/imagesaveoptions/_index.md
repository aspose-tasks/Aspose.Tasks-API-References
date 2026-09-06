---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 构造函数。初始化 ImageSaveOptions 类的新实例，可用于将渲染图像保存为 TIFF、PNG、BMP 或 JPEG 格式"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

初始化一个新的 [`ImageSaveOptions`](../) 类实例，可用于将渲染图像保存为 TIFF、PNG、BMP 或 JPEG 格式。

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | SaveFileFormat | 可以是 TIFF、PNG、BMP 或 JPEG[`SaveFileFormat`](../../savefileformat/)。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当 *saveFormat* 不是有效的图像格式时抛出。有效值为 TIFF、PNG、BMP 或 JPEG。 |

## 示例

展示如何将项目保存为流中的图像。

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // 通过使用 ImageSaveOptions，我们将项目保存为图像格式
    project.Save(stream, options);
}
```

### 另见

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


