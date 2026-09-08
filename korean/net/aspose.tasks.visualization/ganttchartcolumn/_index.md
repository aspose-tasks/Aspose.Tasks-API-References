---
title: "클래스 GanttChartColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.GanttChartColumn 클래스. 프로젝트 보기 클래스"
type: docs
weight: 3090
url: /ko/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

프로젝트 보기 클래스

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | GanttChartColumn 클래스의 새 인스턴스를 초기화합니다. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | GanttChartColumn 클래스의 새 인스턴스를 초기화합니다. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | GanttChartColumn 클래스의 새 인스턴스를 초기화합니다. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | GanttChartColumn 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | 열 필드. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 열 이름을 가져옵니다. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 텍스트 정렬을 가져오거나 설정합니다([`HorizontalStringAlignment`](../horizontalstringalignment/) 열거형의 값 중 하나일 수 있음). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 열 셀의 모양을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 열 너비를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | 현재 작업을 열 텍스트로 변환합니다. |

## 예제

내보낼 Gantt 차트 보기 열을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// 열을 반복합니다
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### 또 보기

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


