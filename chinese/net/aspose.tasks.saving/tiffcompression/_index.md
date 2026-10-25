---
title: "枚举 TiffCompression"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.TiffCompression 枚举。指定在将页面保存为 TIFF 格式时使用的压缩类型"
type: docs
weight: 2250
url: /zh/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

指定将页面保存为 TIFF 格式时应用的压缩类型。

```csharp
public enum TiffCompression
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `1` | 指定不进行压缩。 |
| Rle | `2` | 指定 RLE 压缩方案。 |
| Ccitt3 | `3` | 指定 CCITT3 压缩方案。 |
| Ccitt4 | `4` | 指定 CCITT4 压缩方案。 |
| Lzw | `5` | 指定 LZW 压缩方案。 |

## 示例

展示如何通过使用 RLE 压缩模式以 TIFF 格式渲染。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// 使用 Rle 压缩保存项目
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


