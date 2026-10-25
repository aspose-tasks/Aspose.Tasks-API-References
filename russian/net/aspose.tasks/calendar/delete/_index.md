---
title: "Calendar.Delete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Удаляет календарь из проекта"
type: docs
weight: 140
url: /ru/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Удаляет календарь из проекта.

```csharp
public void Delete()
```

## Примеры

Показывает, как удалить календарь из проекта.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// получить календарь по имени
var calendar = project.Calendars.GetByName("Broken Calendar");

// удалить календарь
calendar.Delete();
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


