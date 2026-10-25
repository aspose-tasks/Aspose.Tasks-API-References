---
title: "GanttChartColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartColumn 메서드. 현재 작업을 열 텍스트로 변환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/ganttchartcolumn/getcolumntext/
---
## GanttChartColumn.GetColumnText method

현재 작업을 열 텍스트로 변환합니다.

```csharp
public string GetColumnText(Task task)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | 작업 | 현재 작업. |

### 반환 값

열 텍스트.

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

* class [Task](../../../aspose.tasks/task/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


