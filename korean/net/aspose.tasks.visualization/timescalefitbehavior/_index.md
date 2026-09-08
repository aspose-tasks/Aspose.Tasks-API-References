---
title: "열거형 TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior 열거형. 시간축 영역을 페이지 너비에 맞추는 동작을 나타냅니다."
type: docs
weight: 3440
url: /ko/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

시간 눈금 영역을 페이지 너비에 맞추는 데 사용되는 동작을 나타냅니다.

```csharp
public enum TimescaleFitBehavior
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| DefinedInView | `0` | 캘린더 섹션은 렌더링된 보기의 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 속성에 따라 렌더링됩니다. |
| NoScaleToEndDate | `1` | 캘린더 섹션은 페이지에 빈 공간이 있더라도 EndDate까지 정확히 렌더링됩니다. |
| NoScaleToEndOfPage | `2` | 캘린더 섹션은 마지막 페이지의 끝(오른쪽)까지 렌더링됩니다. 따라서 마지막으로 렌더링된 날짜가 EndDate를 초과할 수 있습니다. |
| ScaleToEndOfPage | `3` | 렌더링 엔진은 EndDate가 마지막 페이지의 끝(오른쪽)과 맞춰지도록 날짜를 정렬하려고 시도합니다. 이는 MS Project의 "페이지 설정 \ 보기 \ 시간축을 페이지 끝에 맞추기" 옵션이 활성화된 것과 동일합니다. |

## 예제

TimescaleFitBehavior를 사용하여 Gantt 차트의 시간축을 마지막 페이지 끝에 맞추는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


