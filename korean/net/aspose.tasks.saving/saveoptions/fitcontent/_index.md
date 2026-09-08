---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool FitContent { get; set; }
```

## 예제

행 높이를 내용에 맞게 늘릴지 여부 옵션을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // 옵션 fit content를 true로 설정합니다
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


