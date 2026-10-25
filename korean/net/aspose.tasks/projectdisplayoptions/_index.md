---
title: "클래스 ProjectDisplayOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectDisplayOptions 클래스. 프로젝트 인스턴스의 표시 옵션을 나타냅니다."
type: docs
weight: 1450
url: /ko/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

프로젝트 인스턴스에 대한 표시 옵션을 나타냅니다.

```csharp
public class ProjectDisplayOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | `ProjectDisplayOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | 숫자 값과 시간 약어 앞에 공백을 추가할지 여부를 나타내는 값을 가져오거나 설정합니다 (예: 1 wk vs 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | 일 레이블 표시 방식을 가져오거나 설정합니다. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | 시간 레이블 표시 방식을 가져오거나 설정합니다. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | 분 레이블 표시 방식을 가져오거나 설정합니다. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | 월 레이블 표시 방식을 가져오거나 설정합니다. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | 전체 프로젝트에 대한 요약 정보를 단일 행에 표시하고 Gantt 차트 보기 상단에 자체 요약 작업 막대를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | 프로젝트가 수동으로 일정이 지정된 작업과 가능한 일정 충돌을 식별할 때 제안을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 이 옵션은 Project 2010 버전 이후에 사용할 수 있습니다. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Project가 수동으로 예약된 작업과 가능한 일정 충돌을 식별할 때 경고를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 이 옵션은 Project 2010 버전 이상에서 사용할 수 있습니다. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | 하이퍼링크에 밑줄을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | 주 레이블 표시 방법을 가져오거나 설정합니다. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | 연 레이블 표시 방법을 가져오거나 설정합니다. |

## 예제

프로젝트의 표시 옵션 사용 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Project가 수동으로 예약된 작업과 가능한 일정 충돌을 식별할 때 경고를 표시할지 여부를 나타내는 값을 설정합니다.
// 이 옵션은 Project 2010 버전 이상에서 사용할 수 있습니다.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// 숫자 값과 시간 약어 앞에 공백을 추가할지 여부를 나타내는 값 (예: 1 wk vs 1wk).
project.DisplayOptions.AddSpaceBeforeLabel = true;

// 분 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// 시간 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// 일 레이블 표시 방법을 설정합니다.
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// 주 레이블 표시 방법을 설정합니다.
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// 월 레이블이 표시되는 방식을 설정합니다.
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// 연도 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// 전체 프로젝트에 대한 요약 정보를 Gantt 차트 보기 상단에 자체 요약 작업 막대와 함께 단일 행에 표시할지 여부를 나타내는 값을 설정합니다.
project.DisplayOptions.ShowProjectSummaryTask = true;

// Project가 수동으로 예약된 작업과 가능한 일정 충돌을 식별할 때 제안을 표시할지 여부를 나타내는 값을 설정합니다.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// 하이퍼링크에 밑줄을 표시할지 여부를 나타내는 값을 설정합니다.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


