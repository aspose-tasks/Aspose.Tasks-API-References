---
title: "CalendarCollection.Remove"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Удаляет календарь из Project CalendarCollection"
type: docs
weight: 60
url: /ru/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Удаляет Calendar из Project CalendarCollection.

```csharp
public bool Remove(Calendar item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | Calendar | Календарь для удаления. |

### Возвращаемое значение

Если удалён, возвращает true, иначе возвращает false.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, когда календарь нельзя удалить. |

## Примеры

Показывает, как заменить календарь в коллекции.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// добавить новый календарь
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


