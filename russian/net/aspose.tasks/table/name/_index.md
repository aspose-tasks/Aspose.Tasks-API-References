---
title: "Table.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Table. Возвращает или задает имя объекта Table"
type: docs
weight: 50
url: /ru/net/aspose.tasks/table/name/
---
## Table.Name property

Получает или задает имя объекта Table.

```csharp
public string Name { get; set; }
```

## Примеры

Показывает, как определить новую таблицу (используется для представлений).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// получить таблицу для редактирования
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// настроить некоторые свойства
// установить значение, указывающее, можно ли регулировать высоту строки заголовка таблицы
table.AdjustHeaderRowHeight = true;

// установить формат даты таблицы.
table.DateFormat = DateFormat.DateDdMmYyyy;

// установить значение, указывающее, заблокирован ли первый столбец таблицы или доступен для редактирования
table.LockFirstColumn = true;

// установить высоту строки в таблице, где высота строки определяется количеством строк текста
table.RowHeight = 10;

// устанавливает значение, указывающее, показывать ли интерфейс «Добавить новый столбец»
table.ShowAddNewColumn = true;

// установить значение, указывающее, отображает ли проект имя таблицы в раскрывающемся списке Таблицы на вкладке Вид ленты
table.ShowInMenu = true;

// позволяет сохранить обновлённую таблицу
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


