---
title: "Enum Timescale"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Timescale 열거형. 프로젝트를 그래픽 형식으로 내보낼 때 Gantt 차트 작업 사용량 또는 리소스 사용량 뷰에서 시간 눈금을 렌더링하는 방법을 지정하는 옵션을 정의합니다."
type: docs
weight: 3430
url: /ko/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

프로젝트를 그래픽 형식으로 내보낼 때 Gantt 차트, 작업 사용량 또는 리소스 사용량 보기에서 시간 눈금을 렌더링하는 방법을 지정하는 옵션을 정의합니다.

```csharp
public enum Timescale
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| DefinedInView | `0` | 프로젝트 뷰 속성에 정의된 시간 눈금 설정을 사용합니다: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). 뷰 데이터를 포함하는 형식에 대해 유효합니다. 예를 들어, MPP 형식에서 읽은 프로젝트가 해당됩니다. |
| Days | `1` | 세부 수준이 최소 하루인 미리 정의된 2계층 시간 눈금. |
| ThirdsOfMonths | `10` | 세부 수준이 한 달의 3분의 1인 미리 정의된 2계층 시간 눈금. |
| Months | `30` | 세부 수준이 최소 한 달인 미리 정의된 2계층 시간 눈금. |

## 예제

프로젝트를 SVG 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // 문서가 저장될 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />을 설정합니다.
                            PresentationFormat = PresentationFormat.GanttChart,

                            // 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다.
                            FitContent = true,

                            // 렌더링할 최소 시간 기간을 설정합니다. 기본값은 <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>입니다.
                            Timescale = Timescale.ThirdsOfMonths,

                            // 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다.
                            // 현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


