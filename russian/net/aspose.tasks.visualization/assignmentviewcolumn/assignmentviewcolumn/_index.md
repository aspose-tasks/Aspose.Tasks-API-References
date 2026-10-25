---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор AssignmentViewColumn. Инициализирует новый экземпляр класса AssignmentViewColumn."
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Инициализирует новый экземпляр класса AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя столбца. |
| ширина | Int32 | Ширина столбца в пикселях. |
| конвертер | AssignmentToColumnTextConverter | Конвертер данных назначения в текст столбца. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


