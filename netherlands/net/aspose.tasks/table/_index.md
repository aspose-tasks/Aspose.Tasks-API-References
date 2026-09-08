---
title: "Klasse Table"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Table klasse. Vertegenwoordigt een tabel in Project."
type: docs
weight: 2320
url: /nl/net/aspose.tasks/table/
---
## Table class

Stelt een tabel in Project voor.

```csharp
public class Table
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Table](table/)() | Initialiseert een nieuw exemplaar van de `Table` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de hoogte van de koprij van de tabel kan worden aangepast. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Haalt op of stelt het datumformaat van de tabel in. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de eerste kolom van een tabel vergrendeld of bewerkbaar is. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Haalt op of stelt de naam van een Table-object in. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Haalt op of stelt de rijhoogte in een tabel in, waarbij de rijhoogte het aantal tekstregels is. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de 'Add New Column'-interface moet worden weergegeven. Ondersteund vanaf versie MSP 2010 en later. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of het project de tabelnaam toont in de vervolgkeuzelijst Tabellen op het tabblad Weergave van het lint. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Haalt een TableFields-collectie op die de velden in de tabel vertegenwoordigt. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Haalt op of stelt het tabeltype in voor de opgegeven tabel. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Haalt de unieke identifier van een tabel op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Retourneert een hashcode voor deze tabel. |

## Voorbeelden

Toont hoe een nieuwe tabel te definiëren (voor weergaven).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// haal een tabel op om te bewerken
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// pas enkele eigenschappen aan
// stel een waarde in die aangeeft of de hoogte van de koprij van de tabel kan worden aangepast
table.AdjustHeaderRowHeight = true;

// stel het datumformaat van de tabel in.
table.DateFormat = DateFormat.DateDdMmYyyy;

// stel een waarde in die aangeeft of de eerste kolom van een tabel vergrendeld of bewerkbaar is.
table.LockFirstColumn = true;

// stel de rijhoogte in een tabel in, waarbij de rijhoogte het aantal tekstregels is.
table.RowHeight = 10;

// stelt een waarde in die aangeeft of de 'Nieuwe kolom toevoegen'-interface moet worden weergegeven.
table.ShowAddNewColumn = true;

// stel een waarde in die aangeeft of het project de tabelnaam toont in de vervolgkeuzelijst Tabellen op het tabblad Beeld van het lint.
table.ShowInMenu = true;

// laat de bijgewerkte tabel opslaan
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


