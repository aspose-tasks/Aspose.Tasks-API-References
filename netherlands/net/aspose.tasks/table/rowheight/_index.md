---
title: "Table.RowHeight"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Table-eigenschap. Haalt de rijhoogte op of stelt deze in een tabel in, waarbij de rijhoogte het aantal tekstregels is"
type: docs
weight: 60
url: /nl/net/aspose.tasks/table/rowheight/
---
## Table.RowHeight property

Haalt op of stelt de rijhoogte in een tabel in, waarbij de rijhoogte het aantal tekstregels is.

```csharp
public int RowHeight { get; set; }
```

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

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


