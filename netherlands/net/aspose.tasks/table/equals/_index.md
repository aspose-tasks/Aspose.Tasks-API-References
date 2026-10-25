---
title: "Table.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Table-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object"
type: docs
weight: 120
url: /nl/net/aspose.tasks/table/equals/
---
## Table.Equals method

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het object om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe je tabelgelijkheid controleert.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// De gelijkheid van tabellen wordt gecontroleerd ten opzichte van de UID van de tabel.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Zie ook

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


