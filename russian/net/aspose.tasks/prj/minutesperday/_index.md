---
title: "Prj.MinutesPerDay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Количество минут в дне"
type: docs
weight: 470
url: /ru/net/aspose.tasks/prj/minutesperday/
---
## Prj.MinutesPerDay field

Количество минут в дне.

```csharp
public static readonly Key<int, PrjKey> MinutesPerDay;
```

## Примеры

Показывает, как читать/записывать свойства будних дней проекта.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Установить свойства будних дней
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Отобразить свойства будних дней
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


