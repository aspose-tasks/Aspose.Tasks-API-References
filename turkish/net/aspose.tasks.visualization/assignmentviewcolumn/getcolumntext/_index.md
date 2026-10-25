---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AssignmentViewColumn yöntemi. Mevcut kaynak atamasını sütun metnine dönüştürür"
type: docs
weight: 30
url: /tr/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Mevcut kaynak atamasını sütun metnine dönüştürür.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| atama | ResourceAssignment | Mevcut atama. |

### Dönüş Değeri

Sütun metni.

## Örnekler

Atama görünümleri için sütunların nasıl ekleneceğini gösterir.

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

### Ayrıca Bakınız

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


