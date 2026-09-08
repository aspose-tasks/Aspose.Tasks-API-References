---
title: "Класс Table"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Table. Представляет таблицу в Project."
type: docs
weight: 2320
url: /ru/net/aspose.tasks/table/
---
## Table class

Представляет таблицу в Project

```csharp
public class Table
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Table](table/)() | Инициализирует новый экземпляр класса `Table`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Получает или задает значение, указывающее, можно ли изменить высоту строки заголовка таблицы. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Получает или задает формат даты таблицы. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Получает или задает значение, указывающее, заблокирован ли первый столбец таблицы или доступен для редактирования. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Получает или задает имя объекта Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Получает или задает высоту строки в таблице, где высота строки измеряется количеством строк текста. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Получает или задает значение, указывающее, показывать ли интерфейс «Add New Column». Поддерживается версиями MSP 2010 и новее. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли проект имя таблицы в выпадающем списке Tables на вкладке View ленты. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Получает коллекцию TableFields, представляющую поля таблицы. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Получает или задает тип таблицы для указанной таблицы. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Получает уникальный идентификатор таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Возвращает хеш-код для этой таблицы. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


