---
title: "Класс ViewColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.ViewColumn. Представляет столбец в представлении проекта."
type: docs
weight: 3470
url: /ru/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

Представляет столбец в представлении проекта.

```csharp
public abstract class ViewColumn
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | Получает или задает поле столбца. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Получает имя столбца. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Получает или задает выравнивание текста (может быть одним из значений перечисления [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки внешнего вида ячеек столбца. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Получает ширину столбца. |

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


