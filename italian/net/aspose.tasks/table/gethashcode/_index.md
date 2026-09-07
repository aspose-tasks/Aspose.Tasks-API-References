---
title: "Table.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Table. Restituisce un codice hash per questa Table"
type: docs
weight: 130
url: /it/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Restituisce un codice hash per questa Tabella.

```csharp
public override int GetHashCode()
```

### Valore di ritorno

Restituisce un valore di hash code per questo oggetto.

## Esempi

Mostra come ottenere un codice hash di una tabella.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Il codice hash di una tabella è uguale all'UID della tabella 
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Vedi anche

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


