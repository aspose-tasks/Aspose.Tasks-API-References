---
title: "열거형 TiffCompression"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.TiffCompression 열거형. 페이지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 지정합니다."
type: docs
weight: 2250
url: /ko/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

페이지를 TIFF 형식으로 저장할 때 적용할 압축 유형을 지정합니다.

```csharp
public enum TiffCompression
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `1` | 압축을 적용하지 않음을 지정합니다. |
| Rle | `2` | RLE 압축 방식을 지정합니다. |
| Ccitt3 | `3` | CCITT3 압축 방식을 지정합니다. |
| Ccitt4 | `4` | CCITT4 압축 방식을 지정합니다. |
| Lzw | `5` | LZW 압축 방식을 지정합니다. |

## 예제

RLE 압축 모드를 사용하여 TIFF 형식으로 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// RLE 압축으로 프로젝트를 저장합니다
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


