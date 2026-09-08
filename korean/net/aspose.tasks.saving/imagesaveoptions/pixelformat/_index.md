---
title: "ImageSaveOptions.PixelFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. 이미지의 각 픽셀에 대한 색상 데이터 형식을 가져오거나 설정합니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

이미지의 각 픽셀에 대한 색상 데이터 형식을 가져오거나 설정합니다.

```csharp
public PixelFormat PixelFormat { get; set; }
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


