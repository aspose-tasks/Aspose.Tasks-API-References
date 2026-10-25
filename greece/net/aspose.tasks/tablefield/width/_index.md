---
title: "TableField.Width"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TableField ιδιότητα. Λαμβάνει ή ορίζει το πλάτος σε σημεία της στήλης του πεδίου σε έναν πίνακα"
type: docs
weight: 60
url: /el/net/aspose.tasks/tablefield/width/
---
## TableField.Width property

Λαμβάνει ή ορίζει το πλάτος σε σημεία της στήλης πεδίου σε έναν πίνακα.

```csharp
public int Width { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους πίνακες του έργου.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// λάβετε τον πίνακα
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// εμφανίστε όλες τις πληροφορίες των πεδίων του πίνακα
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

### Δείτε επίσης

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


