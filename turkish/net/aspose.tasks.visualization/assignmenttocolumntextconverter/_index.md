---
title: "Vekil AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment verisini sütun dizgesi dönüştürücü"
type: docs
weight: 2920
url: /tr/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment verisini sütunun string dönüştürücüsüne çevirir.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| atama | ResourceAssignment | Dönüştürülecek atama. |

### Dönüş Değeri

Sütun için dize verisi.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


