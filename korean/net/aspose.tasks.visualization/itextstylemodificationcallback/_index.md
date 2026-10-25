---
title: "인터페이스 ITextStyleModificationCallback"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ITextStyleModificationCallback 인터페이스. TextStyle이 테이블 셀에 적용되기 전에 호출되는 콜백을 나타냅니다."
type: docs
weight: 3160
url: /ko/net/aspose.tasks.visualization/itextstylemodificationcallback/
---
## ITextStyleModificationCallback interface

TextStyle이 테이블 셀에 적용되기 전에 호출되는 콜백을 나타냅니다.

```csharp
public interface ITextStyleModificationCallback
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [BeforeTaskTextStyleApplied](../../aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/)(TaskTextStyleEventArgs) | 다음 보기에서 작업 행에 대한 테이블 셀을 렌더링하기 전에 호출되는 메서드: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


