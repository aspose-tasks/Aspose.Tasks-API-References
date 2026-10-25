---
title: "Calendar.PrimaveraProperties"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает объект, содержащий специфические для Primavera свойства календаря, считанные из форматов Primavera"
type: docs
weight: 100
url: /ru/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Получает объект, содержащий свойства, специфичные для Primavera, для календаря, считанного из форматов Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Примеры

Показывает, как прочитать проект из файла Primavera и изучить специфические для Primavera свойства календаря.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Возвращает проект со специальным UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### См. также

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


