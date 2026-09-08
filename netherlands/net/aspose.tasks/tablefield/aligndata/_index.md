---
title: "TableField.AlignData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableField property. Haalt de uitlijning van gegevens in een tabelveld op of stelt deze in"
type: docs
weight: 20
url: /nl/net/aspose.tasks/tablefield/aligndata/
---
## TableField.AlignData property

Haalt op of stelt de uitlijning van gegevens in een tabelveld in.

```csharp
public HorizontalStringAlignment AlignData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


