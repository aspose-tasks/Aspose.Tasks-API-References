---
title: "TableField.WrapText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableField-eigenschap. Haalt een waarde op of stelt een waarde in die aangeeft of de kolomtekst kan worden afgebroken over meerdere regels of dat deze moet worden afgekapt wanneer deze de kolombreedte overschrijdt. Ondersteund vanaf versie MSP 2010 en later"
type: docs
weight: 80
url: /nl/net/aspose.tasks/tablefield/wraptext/
---
## TableField.WrapText property

Haalt een waarde op of stelt deze in die aangeeft of de kolomtekst kan worden afgebroken over meerdere regels, of dat deze moet worden afgekapt wanneer deze de kolombreedte overschrijdt. Ondersteund door versie MSP 2010 en later.

```csharp
public bool WrapText { get; set; }
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


