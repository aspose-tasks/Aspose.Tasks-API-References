---
title: "Sınıf AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.AssignmentViewColumn sınıfı. Projeler görünüm sınıfı"
type: docs
weight: 2930
url: /tr/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Projenin görünüm sınıfı.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | AssignmentViewColumn sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Sütun alanı. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Sütun adını alır. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Metnin hizalamasını alır veya ayarlar ([`HorizontalStringAlignment`](../horizontalstringalignment/) enum değerlerinden biri olabilir). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Sütun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır veya ayarlar. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Sütun genişliğini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Mevcut kaynak atamasını sütun metnine dönüştürür. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


