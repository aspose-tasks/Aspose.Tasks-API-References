---
title: "클래스 PageLegendItem"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PageLegendItem 클래스. 간트 차트 페이지 범례의 항목을 나타냅니다."
type: docs
weight: 3220
url: /ko/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Gantt 차트 페이지 범례의 항목을 나타냅니다.

```csharp
public sealed class PageLegendItem
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | `PageLegendItem` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | 항목의 유형을 가져옵니다. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | 항목의 텍스트 레이블을 가져옵니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


