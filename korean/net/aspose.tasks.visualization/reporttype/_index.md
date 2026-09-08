---
title: "Enum ReportType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ReportType enum. 프로젝트 그래픽 보고서 유형"
type: docs
weight: 3330
url: /ko/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

프로젝트 그래픽 보고서 유형입니다.

```csharp
public enum ReportType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| ProjectOverview | `0` | 프로젝트의 시작 및 종료 날짜, 완료된 기간 비율, 최상위 작업의 완료 비율 및 다가오는 마일스톤을 표시합니다. |
| CostOverview | `1` | 프로젝트의 시작 및 종료 날짜, 현재 예정된 비용 및 남은 비용, 완료 비율 및 최상위 작업의 비용 값을 표시합니다. |
| WorkOverview | `2` | 각 최상위 작업에 대한 기준선, 실제, 남은 작업량과 작업 리소스의 작업량을 표시합니다. |
| ResourceOverview | `3` | 리소스별 기준선, 실제 및 남은 작업량을 표시합니다. |
| ResourceCostOverview | `4` | 리소스별 기준선, 실제 및 남은 비용을 표시합니다. |
| CriticalTasks | `5` | 중요한 프로젝트 작업을 표시합니다. |
| LateTasks | `6` | 지연된 프로젝트 작업을 표시합니다. |
| Milestones | `7` | 지연된, 다가오는 및 완료된 마일스톤을 표시합니다. |
| UpcomingTask | `8` | 현재 주에 마감되는 작업과 현재 주에 시작되는 작업을 표시합니다. |
| CostOverruns | `9` | 작업 및 리소스별 비용 변동을 표시합니다. |
| TaskCostOverview | `10` | 모든 최상위 작업의 기준선, 실제 및 남은 비용을 표시합니다. |
| OverallocatedResources | `11` | 과다 할당된 리소스의 남은 작업 시간을 표시합니다. |
| SlippingTasks | `12` | 기준 종료 날짜 이후에 완료될 예정인 작업을 표시합니다 (기준이 설정되어 있어야 합니다). |
| BestPracticeAnalyzer | `13` | 실제 작업이 없는 작업, 할당되지 않은 작업, 기간이 8시간 미만인 작업 및 리소스에 할당된 요약을 표시합니다. |
| Burndown | `14` | 작업 소진 차트와 작업 항목 소진 차트를 포함합니다. 작업 소진 차트는 사람들이 완료한 작업량, 프로젝트 종료일 이전에 완료될 예정인 작업량, 그리고 현재 시점에서 완료될 것으로 예상되는 작업량의 기준선 추정치를 보여줍니다. 작업 항목 소진 차트는 완료된 작업 수, 남은 작업 수, 그리고 현재 시점에서 완료될 것으로 예상되는 작업 수의 기준선 추정치를 보여줍니다. |
| CashFlow | `15` | 모든 최상위 작업에 대한 분기별 비용 및 누적 비용을 표시합니다. |

## 예제

프로젝트 번다운 보고서를 PDF 형식으로 지정된 스트림에 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


