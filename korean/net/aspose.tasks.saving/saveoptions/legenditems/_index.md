---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져오거나 설정합니다. null인 경우 기본 항목이 렌더링됩니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져오거나 설정합니다. null인 경우 기본 항목이 렌더링됩니다.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## 비고

Gantt 차트 뷰가 렌더링될 때만 적용됩니다.

## 예제

간트 차트 페이지 범례에서 작업 막대를 사용자 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### 또 보기

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


