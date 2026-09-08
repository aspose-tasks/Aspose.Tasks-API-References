---
title: "Класс TaskTextStyleEventArgs"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.TaskTextStyleEventArgs. Этот класс представляет набор данных, связанных с отрисовкой содержимого ячеек таблицы."
type: docs
weight: 3390
url: /ru/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

Этот класс представляет набор данных, связанных с отображением содержимого ячейки таблицы.

```csharp
public class TaskTextStyleEventArgs
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | Получает или задает TextStyle, который будет использоваться для рисования содержимого ячейки. Этот объект можно использовать для настройки внешнего вида ячейки таблицы. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | Получает [`ViewColumn`](../viewcolumn/), к которой принадлежит текущая отрисовываемая ячейка. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | Получает [`Task`](./task/), соответствующую текущей отрисовываемой строке. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


