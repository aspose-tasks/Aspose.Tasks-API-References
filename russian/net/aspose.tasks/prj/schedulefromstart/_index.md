---
title: "Prj.ScheduleFromStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, следует ли рассчитывать график проекта от даты начала вперёд"
type: docs
weight: 630
url: /ru/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Определяет, рассчитывать ли график проекта вперёд от даты начала.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
```

## Примеры

Показывает, как перенести расписание проекта от даты завершения вместо даты начала.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Теперь рассчитываются все даты задач (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). Чтобы получить критический путь, необходимо вычислить запасы (можно вызвать в отдельном потоке, но только после расчёта всех ранних/поздних дат).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


