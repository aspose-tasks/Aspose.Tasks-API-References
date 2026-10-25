---
title: "TaskTextStyleEventArgs.Column"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskTextStyleEventArgs 속성. 현재 렌더링된 셀이 속한 ViewColumn을 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/tasktextstyleeventargs/column/
---
## TaskTextStyleEventArgs.Column property

현재 렌더링된 셀이 속한 [`ViewColumn`](../../viewcolumn/)을 가져옵니다.

```csharp
public ViewColumn Column { get; }
```

## 예제

내보낼 보기 열을 추가하는 방법을 보여줍니다.

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // 열을 반복합니다
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// 다음 보기에서 작업 행에 대한 테이블 셀을 렌더링하기 전에 호출되는 메서드:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name=\"args\">이 <see cref=\"T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs\" /> 객체.</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### 또 보기

* class [ViewColumn](../../viewcolumn/)
* class [TaskTextStyleEventArgs](../)
* namespace [Aspose.Tasks.Visualization](../../tasktextstyleeventargs/)
* assembly [Aspose.Tasks](../../../)


