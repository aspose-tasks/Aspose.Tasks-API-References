---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. JPEG 품질을 가져오거나 설정합니다. 허용값 범위는 0..100입니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

JPEG 품질을 가져오거나 설정합니다. 허용값 범위는 0..100입니다.

```csharp
public int JpegQuality { get; set; }
```

## 예제

출력 JPEG 파일의 JPEG 품질을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// JPEG 품질을 조정하려면 ImageSaveOptions.JpegQuality 속성을 사용할 수 있습니다.
// 허용되는 값 범위는 0..100입니다.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### 또 보기

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


