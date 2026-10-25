---
title: "Делегат AssignmentToColumnTextConverter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конвертер строк данных ResourceAssignment в столбцы"
type: docs
weight: 2920
url: /ru/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Данные ResourceAssignment в конвертер строк столбца.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | ResourceAssignment | Назначение для конвертации. |

### Возвращаемое значение

Строковые данные для столбца.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


