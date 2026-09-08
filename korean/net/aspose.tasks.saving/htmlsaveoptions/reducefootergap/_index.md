---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 속성. 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 150
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

마지막 작업과 푸터 사이의 간격을 줄일지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ReduceFooterGap { get; set; }
```

## 예제

HTML 출력 파일에서 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### 또 보기

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


