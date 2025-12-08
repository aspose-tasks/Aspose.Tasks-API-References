---
title: Class AssignmentViewColumn
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.AssignmentViewColumn class. Projects view class
type: docs
weight: 2880
url: /net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Project's view class.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Constructors

| Name | Description |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Initializes a new instance of the AssignmentViewColumn class. |

## Properties

| Name | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Column field. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Gets the column name. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Gets or sets alignment of the text (can be one of the values of the [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Gets or sets the callback which can be used to customize the appearance of the column's cells. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Gets the column width. |

## Methods

| Name | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Converts current resource assignment to the column text. |

## Examples

Shows how to add columns for assignment views.

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

### See Also

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


