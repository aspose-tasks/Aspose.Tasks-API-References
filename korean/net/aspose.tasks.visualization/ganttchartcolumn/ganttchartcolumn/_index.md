---
title: "GanttChartColumn.GanttChartColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartColumn 생성자. GanttChartColumn 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/ganttchartcolumn/ganttchartcolumn/
---
## GanttChartColumn(string, int, TaskToColumnTextConverter, Field) {#constructor_3}

GanttChartColumn 클래스의 새 인스턴스를 초기화합니다.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter, Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열의 너비(픽셀). |
| 변환기 | TaskToColumnTextConverter | 작업 데이터를 열 텍스트로 변환하는 변환기. |
| 필드 | 필드 | 열 필드. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, TaskToColumnTextConverter) {#constructor_2}

GanttChartColumn 클래스의 새 인스턴스를 초기화합니다.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열의 너비(픽셀). |
| 변환기 | TaskToColumnTextConverter | 작업 데이터를 열 텍스트로 변환하는 변환기. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(int, Field) {#constructor}

GanttChartColumn 클래스의 새 인스턴스를 초기화합니다.

```csharp
public GanttChartColumn(int width, Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 너비 | Int32 | 열 너비(픽셀). |
| 필드 | 필드 | 열 필드. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, Field) {#constructor_1}

GanttChartColumn 클래스의 새 인스턴스를 초기화합니다.

```csharp
public GanttChartColumn(string name, int width, Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열 너비(픽셀). |
| 필드 | 필드 | 열 필드. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


