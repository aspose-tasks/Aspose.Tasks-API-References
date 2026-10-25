---
title: "CalendarCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Добавляет новый базовый календарь в этот объект CalendarCollection и возвращает добавленный календарь"
type: docs
weight: 20
url: /ru/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Добавляет новый базовый календарь в этот объект CalendarCollection и возвращает добавленный календарь.

```csharp
public Calendar Add(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя календаря. |

### Возвращаемое значение

Добавлен объект [`Calendar`](../../calendar/).

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Выбрасывается, когда имя календаря равно null. |

## Примеры

Показывает, как создать стандартный календарь.

```csharp
var project = new Project();

// Определите календарь и сделайте его стандартным
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Добавляет новый календарь с указанным базовым календарем в этот объект CalendarCollection и возвращает добавленный календарь.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Указанное имя. |
| baseCalendar | Calendar | Указанный базовый календарь. |

### Возвращаемое значение

Добавлен объект [`Calendar`](../../calendar/).

## Примеры

Показывает, как добавить новые календари.

```csharp
var project = new Project();

// Новые календари могут быть добавлены в коллекцию календарей проекта с помощью перегрузок метода Add коллекции.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


