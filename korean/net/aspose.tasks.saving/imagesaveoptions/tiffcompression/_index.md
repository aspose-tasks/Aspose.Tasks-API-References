---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. 생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 가져오거나 설정합니다"
type: docs
weight: 90
url: /ko/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

생성된 이미지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 가져오거나 설정합니다.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## 비고

TIFF로 저장할 때만 효과가 있습니다. 기본값은 `LZW`입니다.

## 예제

출력 TIFF 파일의 TIFF 압축을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// TIFF 압축을 조작하려면 ImageSaveOptions.TiffCompression 속성을 사용할 수 있습니다.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### 또 보기

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


