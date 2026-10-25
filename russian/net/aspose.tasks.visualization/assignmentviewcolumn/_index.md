---
title: "Класс AssignmentViewColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.AssignmentViewColumn. Класс представления проектов"
type: docs
weight: 2930
url: /ru/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Класс представления проекта.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Инициализирует новый экземпляр класса AssignmentViewColumn. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Поле столбца. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Получает имя столбца. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Получает или задает выравнивание текста (может быть одним из значений перечисления [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки внешнего вида ячеек столбца. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Получает ширину столбца. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Преобразует текущее назначение ресурса в текст столбца. |

## Примеры

Показывает, как добавить столбцы для представлений назначений.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### См. также

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


