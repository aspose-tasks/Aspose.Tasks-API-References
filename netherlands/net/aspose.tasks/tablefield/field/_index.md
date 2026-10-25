---
title: "TableField.Field"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableField-eigenschap. Haalt het type van een tabelveld op of stelt dit in"
type: docs
weight: 40
url: /nl/net/aspose.tasks/tablefield/field/
---
## TableField.Field property

Haalt op of stelt het type van een tabelveld in.

```csharp
public Field Field { get; set; }
```

## Voorbeelden

Toont hoe projecttabellen te lezen.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// haal de tabel op
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// geef alle informatie van tabelvelden weer
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

### Zie ook

* enum [Field](../../field/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


