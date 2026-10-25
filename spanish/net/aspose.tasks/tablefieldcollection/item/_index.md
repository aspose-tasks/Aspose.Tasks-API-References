---
title: "TableFieldCollection.Item"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "TableFieldCollection propiedad. Devuelve o establece el elemento en el índice especificado"
type: docs
weight: 30
url: /es/net/aspose.tasks/tablefieldcollection/item/
---
## TableFieldCollection indexer

Devuelve o establece el elemento en el índice especificado.

```csharp
public TableField this[int index] { get; set; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento a obtener o establecer. |

### Valor devuelto

el elemento en el índice especificado.

## Ejemplos

Muestra cómo trabajar con colecciones de campos de tabla.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // iterar sobre los campos de tabla
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// agregar un nuevo campo de tabla
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// insertar un nuevo campo en la posición
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// permite editar el nuevo campo de tabla usando acceso por índice
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// recientemente podemos eliminar el campo
table.TableFields.RemoveAt(idx);

// se puede limpiar la colección de dos maneras
if (deleteOneByOne)
{
    // copiar los campos de tabla en el arreglo y eliminarlos uno por uno
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // o se puede vaciar una colección de campos de tabla completamente
    table.TableFields.Clear();
}
```

### Ver también

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


