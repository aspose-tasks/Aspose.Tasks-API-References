---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод AssignmentViewColumn. Преобразует текущее назначение ресурса в текст столбца"
type: docs
weight: 30
url: /ru/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Преобразует текущее назначение ресурса в текст столбца.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | ResourceAssignment | Текущее назначение. |

### Возвращаемое значение

Текст столбца.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


