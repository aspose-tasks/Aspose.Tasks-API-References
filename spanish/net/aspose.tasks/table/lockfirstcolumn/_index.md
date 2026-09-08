---
title: "Table.LockFirstColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Table. Obtiene o establece un valor que indica si la primera columna de una tabla está bloqueada o es editable"
type: docs
weight: 40
url: /es/net/aspose.tasks/table/lockfirstcolumn/
---
## Table.LockFirstColumn property

Obtiene o establece un valor que indica si la primera columna de una tabla está bloqueada o es editable.

```csharp
public bool LockFirstColumn { get; set; }
```

## Ejemplos

Muestra cómo definir una tabla nueva (usando para vistas).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// obtener una tabla para editar
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// ajustar algunas propiedades
// establecer un valor que indique si la altura de la fila de encabezado de la tabla puede ajustarse
table.AdjustHeaderRowHeight = true;

// establecer el formato de fecha de la tabla.
table.DateFormat = DateFormat.DateDdMmYyyy;

// establecer un valor que indique si la primera columna de una tabla está bloqueada o es editable
table.LockFirstColumn = true;

// establecer la altura de la fila en una tabla, donde la altura de la fila es el número de líneas de texto
table.RowHeight = 10;

// establece un valor que indique si se muestra la interfaz 'Agregar nueva columna'
table.ShowAddNewColumn = true;

// establecer un valor que indique si el proyecto muestra el nombre de la tabla en la lista desplegable Tablas en la pestaña Vista de la cinta de opciones
table.ShowInMenu = true;

// permite guardar la tabla actualizada
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


