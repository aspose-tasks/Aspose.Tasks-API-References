---
title: "Clase TableFieldCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TableFieldCollection. Contiene una lista de objetos TableField. Implementa la interfaz IListTableField."
type: docs
weight: 2350
url: /es/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Contiene una lista de objetos [`TableField`](../tablefield/). Implementa la interfaz IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Determina el índice del elemento especificado en esta colección. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Inserta el elemento especificado en el índice especificado. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Elimina la primera aparición de un objeto específico de esta colección. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Elimina un elemento en el índice especificado. |

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

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


