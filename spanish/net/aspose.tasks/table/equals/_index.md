---
title: "Table.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Table. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 120
url: /es/net/aspose.tasks/table/equals/
---
## Table.Equals method

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto para comparar con esta instancia. |

### Valor devuelto

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de tablas.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// La igualdad de las tablas se verifica contra el UID de la tabla.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Ver también

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


