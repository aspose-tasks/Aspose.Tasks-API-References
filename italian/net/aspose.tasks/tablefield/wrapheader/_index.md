---
title: "TableField.WrapHeader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TableField. Ottiene o imposta un valore che indica se l'intestazione della colonna della tabella può andare a capo su più righe o se deve essere troncata quando supera la larghezza della colonna"
type: docs
weight: 70
url: /it/net/aspose.tasks/tablefield/wrapheader/
---
## TableField.WrapHeader property

Ottiene o imposta un valore che indica se l'intestazione della colonna della tabella può andare a capo su più righe, o se deve essere troncata quando supera la larghezza della colonna.

```csharp
public bool WrapHeader { get; set; }
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


