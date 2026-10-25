---
title: "Table.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Table-methode. Retourneert een hashcode voor deze Table"
type: docs
weight: 130
url: /nl/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Retourneert een hashcode voor deze tabel.

```csharp
public override int GetHashCode()
```

### Retourwaarde

Retourneert een hashcode‑waarde voor dit object.

## Voorbeelden

Toont hoe je een hashcode van een tabel krijgt.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// De hashcode van een tabel is gelijk aan de UID van de tabel 
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Zie ook

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


