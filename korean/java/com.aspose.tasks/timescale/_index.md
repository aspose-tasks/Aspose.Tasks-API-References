---
title: "Timescale"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 그래픽 형식으로 내보낼 때 Gantt 차트 작업 사용량 또는 리소스 사용량 보기에서 타임스케일을 렌더링하는 방법을 지정하는 옵션을 정의합니다."
type: docs
weight: 323
url: /ko/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

프로젝트를 그래픽 형식으로 내보낼 때 Gantt 차트, 작업 사용 또는 리소스 사용 보기에서 시간 눈금을 렌더링하는 방법을 지정하는 옵션을 정의합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [Days](#Days) | 최소 세부 수준이 하루인 사전 정의된 2단계 타임스케일. |
| [DefinedInView](#DefinedInView) | 프로젝트 보기 속성에 정의된 타임스케일 설정을 사용합니다: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | 최소 세부 수준이 한 달인 사전 정의된 2단계 타임스케일. |
| [ThirdsOfMonths](#ThirdsOfMonths) | 세부 수준이 한 달의 1/3인 사전 정의된 2단계 타임스케일. |
### Days {#Days}
```
public static final int Days
```


최소 세부 수준이 하루인 사전 정의된 2단계 타임스케일.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


프로젝트 보기 속성에 정의된 타임스케일 설정을 사용합니다: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). 뷰 데이터가 포함된 형식에 대해 유효합니다. 예를 들어, MPP 형식에서 읽은 프로젝트가 해당됩니다.

--------------------

뷰에 타임스케일 설정이 지정되지 않은 경우, 사전 정의된 Timescale.Days 설정이 대신 사용됩니다.

### Months {#Months}
```
public static final int Months
```


최소 세부 수준이 한 달인 사전 정의된 2단계 타임스케일.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


세부 수준이 한 달의 1/3인 사전 정의된 2단계 타임스케일.

