---
title: "ITextStyleModificationCallback.BeforeTaskTextStyleApplied"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ITextStyleModificationCallback. Метод, который вызывается перед отрисовкой ячейки таблицы для строки задачи в следующих представлениях: Gantt Chart, Task Sheet, Task Usage"
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/
---
## ITextStyleModificationCallback.BeforeTaskTextStyleApplied method

Метод, вызываемый перед отрисовкой ячейки таблицы для строки задачи в следующих представлениях: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

```csharp
public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| args | TaskTextStyleEventArgs | Объект [`TaskTextStyleEventArgs`](../../tasktextstyleeventargs/). |

## Примеры

Показывает, как добавить столбцы представления для экспорта.

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

    // итерация по столбцам
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
    /// Метод, вызываемый перед отрисовкой ячейки таблицы для строки задачи в следующих представлениях:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name=\"args\">Объект <see cref=\"T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs\" />.</param>
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

### См. также

* class [TaskTextStyleEventArgs](../../tasktextstyleeventargs/)
* interface [ITextStyleModificationCallback](../)
* namespace [Aspose.Tasks.Visualization](../../itextstylemodificationcallback/)
* assembly [Aspose.Tasks](../../../)


