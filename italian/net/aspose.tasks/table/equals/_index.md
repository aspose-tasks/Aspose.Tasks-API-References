---
title: "Table.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Table. Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato"
type: docs
weight: 120
url: /it/net/aspose.tasks/table/equals/
---
## Table.Equals method

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza della tabella.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// L'uguaglianza delle tabelle viene verificata rispetto all'UID della tabella.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Vedi anche

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


