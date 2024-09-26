---
title: TableField.AlignData
second_title: Aspose.Tasks for .NET API Reference
description: TableField property. Gets or sets the alignment of data in a table field
type: docs
weight: 20
url: /net/aspose.tasks/tablefield/aligndata/
---
## TableField.AlignData property

Gets or sets the alignment of data in a table field.

```csharp
public HorizontalStringAlignment AlignData { get; set; }
```

## Examples

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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


