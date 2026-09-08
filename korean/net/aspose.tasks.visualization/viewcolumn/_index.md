---
title: "클래스 ViewColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ViewColumn 클래스. 프로젝트 보기에서 열을 나타냅니다."
type: docs
weight: 3470
url: /ko/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

프로젝트 보기에서 열을 나타냅니다.

```csharp
public abstract class ViewColumn
```

## 속성

| 이름 | 설명 |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | 열 필드를 가져오거나 설정합니다. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 열 이름을 가져옵니다. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 텍스트 정렬을 가져오거나 설정합니다([`HorizontalStringAlignment`](../horizontalstringalignment/) 열거형의 값 중 하나일 수 있음). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 열 셀의 모양을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 열 너비를 가져옵니다. |

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


