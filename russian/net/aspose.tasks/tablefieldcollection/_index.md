---
title: "Класс TableFieldCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TableFieldCollection. Содержит список объектов TableField. Реализует интерфейс IListTableField."
type: docs
weight: 2350
url: /ru/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Содержит список объектов [`TableField`](../tablefield/). Реализует интерфейс IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Определяет индекс указанного элемента в этой коллекции. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Вставляет указанный элемент в указанный индекс. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Удаляет элемент по указанному индексу. |

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

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


