---
title: "Класс TableCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TableCollection. Содержит список объектов Table. Реализует интерфейс ICollectionTable"
type: docs
weight: 2330
url: /ru/net/aspose.tasks/tablecollection/
---
## TableCollection class

Содержит список объектов [`Table`](../table/). Реализует интерфейс ICollection&lt;Table&gt;.

```csharp
public class TableCollection : ICollection<Table>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Преобразует коллекцию таблиц в список объектов [`Table`](../table/). |

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

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


