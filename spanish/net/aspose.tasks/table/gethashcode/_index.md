---
title: "Table.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Table. Devuelve un código hash para esta Table"
type: docs
weight: 130
url: /es/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Devuelve un código hash para esta Tabla.

```csharp
public override int GetHashCode()
```

### Valor devuelto

Devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una tabla.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// El código hash de una tabla es igual al UID de la tabla
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Ver también

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


