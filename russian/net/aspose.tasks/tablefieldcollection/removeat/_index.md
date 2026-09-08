---
title: "TableFieldCollection.RemoveAt"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TableFieldCollection. Удаляет элемент по указанному индексу"
type: docs
weight: 120
url: /ru/net/aspose.tasks/tablefieldcollection/removeat/
---
## TableFieldCollection.RemoveAt method

Удаляет элемент по указанному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | указанный нулевой индекс, по которому следует удалить элемент. |

## Примеры

Показывает, как работать с коллекциями полей таблицы.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // перебрать поля таблицы
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// добавить новое поле таблицы
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// вставить новое поле в указанную позицию
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// позволяет редактировать новое поле таблицы, используя доступ по индексу
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// в последнее время мы можем удалить поле
table.TableFields.RemoveAt(idx);

// коллекцию можно очистить двумя способами
if (deleteOneByOne)
{
    // скопировать поля таблицы в массив и удалять их по одному
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // или можно полностью очистить коллекцию полей таблицы
    table.TableFields.Clear();
}
```

### См. также

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


