---
title: "TableField.TableField"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore TableField. Inizializza una nuova istanza della classe TableField"
type: docs
weight: 10
url: /it/net/aspose.tasks/tablefield/tablefield/
---
## TableField constructor

Inizializza una nuova istanza della classe [`TableField`](../).

```csharp
public TableField()
```

## Esempi

Mostra come leggere le tabelle del progetto.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// ottieni la tabella
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// visualizza le informazioni di tutti i campi della tabella
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

### Vedi anche

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


