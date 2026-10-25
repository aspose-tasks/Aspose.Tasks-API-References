---
title: "Clase Table"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Table clase. Representa una tabla en Project"
type: docs
weight: 2320
url: /es/net/aspose.tasks/table/
---
## Table class

Representa una tabla en Project

```csharp
public class Table
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Table](table/)() | Inicializa una nueva instancia de la clase `Table`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Obtiene o establece un valor que indica si la altura de la fila de encabezado de la tabla puede ajustarse. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Obtiene o establece el formato de fecha de la tabla. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Obtiene o establece un valor que indica si la primera columna de una tabla está bloqueada o es editable. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Obtiene o establece el nombre de un objeto Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Obtiene o establece la altura de la fila en una tabla, donde la altura de la fila es el número de líneas de texto. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Obtiene o establece un valor que indica si se muestra la interfaz 'Add New Column'. Compatible con la versión MSP 2010 y posteriores. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si el proyecto muestra el nombre de la tabla en la lista desplegable Tables en la pestaña Ver de la cinta de opciones. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Obtiene una colección TableFields que representa los campos de la tabla. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Obtiene o establece el tipo de tabla para la tabla especificada. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Obtiene el identificador único de una tabla. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Devuelve un código hash para esta Tabla. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


