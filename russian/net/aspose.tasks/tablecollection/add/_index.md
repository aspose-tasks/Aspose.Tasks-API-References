---
title: "TableCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TableCollection. Добавляет указанный элемент в эту коллекцию."
type: docs
weight: 30
url: /ru/net/aspose.tasks/tablecollection/add/
---
## TableCollection.Add method

Добавляет указанный элемент в эту коллекцию.

```csharp
public void Add(Table item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | Table | указанный элемент для добавления в эту коллекцию. |

## Примеры

Показывает, как работать с коллекциями таблиц.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// перебрать таблицы
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

// добавить новую таблицу
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// коллекцию можно очистить двумя способами
if (deleteOneByOne)
{
    // скопировать таблицы в массив и удалять их по одной
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // или можно полностью очистить коллекцию таблиц
    project.Tables.Clear();
}

// коллекцию можно преобразовать в простой список таблиц
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### См. также

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


