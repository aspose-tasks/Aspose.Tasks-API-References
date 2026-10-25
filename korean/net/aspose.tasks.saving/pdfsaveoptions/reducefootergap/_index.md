---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

마지막 작업과 푸터 사이의 간격을 줄일지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ReduceFooterGap { get; set; }
```

## 예제

PDF 출력 파일에서 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### 또 보기

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


