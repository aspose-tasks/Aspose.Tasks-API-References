---
title: "TableCollection.Contains"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TableCollection. Devuelve true si el elemento especificado se encuentra en esta colección, de lo contrario false"
type: docs
weight: 50
url: /es/net/aspose.tasks/tablecollection/contains/
---
## TableCollection.Contains method

Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

```csharp
public bool Contains(Table item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | Table | el elemento especificado para buscar. |

### Valor devuelto

true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

## Ejemplos

Muestra cómo trabajar con colecciones de tablas.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// iterar sobre tablas
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// agregar una nueva tabla
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// se puede limpiar la colección de dos maneras
if (deleteOneByOne)
{
    // copiar tablas al arreglo y eliminarlas una por una
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // o se puede limpiar una colección de tablas completamente
    project.Tables.Clear();
}

// la colección puede convertirse en una lista simple de tablas
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Ver también

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


