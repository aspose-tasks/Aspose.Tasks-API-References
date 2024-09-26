---
title: TableField.WrapText
second_title: Aspose.Tasks for .NET API Reference
description: TableField property. Gets or sets a value indicating whether the column text can wrap to multiple lines or if it should be truncated when it exceeds the column width. Supported by MSP 2010 version and later
type: docs
weight: 80
url: /net/aspose.tasks/tablefield/wraptext/
---
## TableField.WrapText property

Gets or sets a value indicating whether the column text can wrap to multiple lines, or if it should be truncated when it exceeds the column width. Supported by MSP 2010 version and later.

```csharp
public bool WrapText { get; set; }
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

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


