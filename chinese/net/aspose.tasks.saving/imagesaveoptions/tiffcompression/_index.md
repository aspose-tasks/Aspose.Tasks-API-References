---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置在将生成的图像保存为 TIFF 格式时使用的压缩类型"
type: docs
weight: 90
url: /zh/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

获取或设置将生成的图像保存为 TIFF 格式时使用的压缩类型。

```csharp
public TiffCompression TiffCompression { get; set; }
```

## 备注

仅在保存为 TIFF 时生效。默认值为 `LZW`。

## 示例

展示如何设置输出 TIFF 文件的 TIFF 压缩。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// 为了操作 TIFF 压缩，我们可以使用 ImageSaveOptions.TiffCompression 属性。
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### 另见

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


