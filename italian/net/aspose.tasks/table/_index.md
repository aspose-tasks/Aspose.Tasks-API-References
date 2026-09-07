---
title: "Classe Table"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Table. Rappresenta una tabella in Project."
type: docs
weight: 2320
url: /it/net/aspose.tasks/table/
---
## Table class

Rappresenta una tabella in Project

```csharp
public class Table
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Table](table/)() | Inizializza una nuova istanza della classe `Table`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga di intestazione della tabella può essere regolata. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Ottiene o imposta il formato data della tabella. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Ottiene o imposta un valore che indica se la prima colonna di una tabella è bloccata o modificabile. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Ottiene o imposta il nome di un oggetto Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Ottiene o imposta l'altezza della riga in una tabella, dove l'altezza della riga è il numero di linee di testo. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Ottiene o imposta un valore che indica se mostrare l'interfaccia 'Add New Column'. Supportata dalla versione MSP 2010 e successive. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se il progetto mostra il nome della tabella nell'elenco a discesa Tabelle nella scheda Visualizza del Ribbon. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Ottiene una collezione TableFields che rappresenta i campi nella tabella. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Ottiene o imposta il tipo di tabella per la tabella specificata. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Ottiene l'identificatore univoco di una tabella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Restituisce un codice hash per questa Tabella. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


