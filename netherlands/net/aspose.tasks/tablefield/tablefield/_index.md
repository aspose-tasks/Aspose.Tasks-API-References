---
title: "TableField.TableField"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableField-constructor. Initialiseert een nieuw exemplaar van de TableField-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/tablefield/tablefield/
---
## TableField constructor

Initialiseert een nieuw exemplaar van de [`TableField`](../) klasse.

```csharp
public TableField()
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

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


