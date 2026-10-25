---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. DPI 단위의 수직 해상도를 가져오거나 설정합니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

수직 해상도를 dpi 단위로 가져오거나 설정합니다.

```csharp
public float VerticalResolution { get; set; }
```

## 예제

이미지 형식으로 변환하는 동안 사용되는 픽셀 형식을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### 또 보기

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


