---
title: "Table.ShowAddNewColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Table. Ottiene o imposta un valore che indica se mostrare l'interfaccia Add New Column. Supportato dalla versione MSP 2010 e successive"
type: docs
weight: 70
url: /it/net/aspose.tasks/table/showaddnewcolumn/
---
## Table.ShowAddNewColumn property

Ottiene o imposta un valore che indica se mostrare l'interfaccia 'Add New Column'. Supportata dalla versione MSP 2010 e successive.

```csharp
public bool ShowAddNewColumn { get; set; }
```

## Esempi

Mostra come definire una nuova tabella (utilizzata per le visualizzazioni).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// ottieni una tabella da modificare
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// regola alcune proprietà
// imposta un valore che indica se l'altezza della riga di intestazione della tabella può essere regolata
table.AdjustHeaderRowHeight = true;

// imposta il formato data della tabella.
table.DateFormat = DateFormat.DateDdMmYyyy;

// imposta un valore che indica se la prima colonna di una tabella è bloccata o modificabile
table.LockFirstColumn = true;

// imposta l'altezza della riga in una tabella, dove l'altezza della riga è il numero di righe di testo
table.RowHeight = 10;

// imposta un valore che indica se mostrare l'interfaccia 'Aggiungi Nuova Colonna'
table.ShowAddNewColumn = true;

// imposta un valore che indica se il progetto mostra il nome della tabella nell'elenco a discesa Tabelle nella scheda Visualizza del Ribbon
table.ShowInMenu = true;

// consente di salvare la tabella aggiornata
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


