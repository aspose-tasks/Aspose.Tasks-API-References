---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 생성자. 렌더링된 이미지를 TIFF, PNG, BMP 또는 JPEG 형식으로 저장하는 데 사용할 수 있는 ImageSaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

새 인스턴스를 초기화합니다. [`ImageSaveOptions`](../) 클래스는 렌더링된 이미지를 TIFF, PNG, BMP 또는 JPEG 형식으로 저장하는 데 사용할 수 있습니다.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| saveFormat | SaveFileFormat | TIFF, PNG, BMP 또는 JPEG[`SaveFileFormat`](../../savefileformat/)일 수 있습니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *saveFormat*이(가) 유효한 이미지 형식이 아닐 경우 발생합니다. 유효한 값은 TIFF, PNG, BMP 또는 JPEG입니다. |

## 예제

프로젝트를 스트림에 이미지로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions를 사용하여 프로젝트를 이미지 형식으로 저장합니다.
    project.Save(stream, options);
}
```

### 또 보기

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


