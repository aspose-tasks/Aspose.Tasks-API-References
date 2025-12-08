---
title: Class TableField
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TableField class. Represents a field of a table in a project
type: docs
weight: 2300
url: /net/aspose.tasks/tablefield/
---
## TableField class

Represents a field of a table in a project.

```csharp
public class TableField
```

## Constructors

| Name | Description |
| --- | --- |
| [TableField](tablefield/)() | Initializes a new instance of the `TableField` class. |

## Properties

| Name | Description |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Gets or sets the alignment of data in a table field. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Gets or sets the alignment of the title in a table field. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Gets or sets the type of a table field. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Gets or sets the title of the field in a table. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Gets or sets the width in points of the field column in a table. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Gets or sets a value indicating whether the table column heading can wrap to multiple lines, or if it should be truncated when it exceeds the column width. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Gets or sets a value indicating whether the column text can wrap to multiple lines, or if it should be truncated when it exceeds the column width. Supported by MSP 2010 version and later. |

## Examples

Shows how to work with Project's view and add column to the default view (which is shown when MPP file is opened in MS Project).

```csharp
// create an empty project without views 
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modify the default view (it's a Gantt chart view).
// Or you can select view by name or by View Screen using project.View collection.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData flag should be used to persist modifications of view's properties.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Shows how to read project tables.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// get the table
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// display all table fields' information
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


