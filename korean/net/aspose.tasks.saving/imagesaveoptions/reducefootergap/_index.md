---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

마지막 작업과 푸터 사이의 간격을 줄일지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ReduceFooterGap { get; set; }
```

## 예제

마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// ReduceFooterGap 속성을 사용하여 작업 목록과 푸터 사이의 간격을 줄입니다.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### 또 보기

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


