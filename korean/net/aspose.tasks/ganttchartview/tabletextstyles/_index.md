---
title: "GanttChartView.TableTextStyles"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartView 속성. Gantt 차트 뷰의 테이블 텍스트 스타일 목록을 가져옵니다. TableTextStyle"
type: docs
weight: 160
url: /ko/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Gantt 차트 뷰의 테이블 텍스트 스타일 목록을 가져옵니다. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## 예제

사용자 정의 테이블 텍스트 스타일을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var view = (GanttChartView)project.Views.ToList()[0];

view.TableTextStyles.Clear();
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Red, Field = Field.TaskName });
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Gray, Field = Field.TaskDurationText });
view.TableTextStyles.Add(new TableTextStyle(2, FontStyles.Bold | FontStyles.Italic | FontStyles.Underline)
{
    Color = Color.Blue
});
```

### 또 보기

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


