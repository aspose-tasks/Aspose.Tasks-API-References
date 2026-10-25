---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 비작업 시간 색상을 가져오거나 설정합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

비작업 시간 색상을 가져오거나 설정합니다.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## 예제

비작업 시간에 대한 사용자 정의 색상을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


