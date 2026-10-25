---
title: "Duration.op_Inequality"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту."
type: docs
weight: 150
url: /ru/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| a | Продолжительность | Первая длительность. |
| b | Продолжительность | Вторая длительность. |

### Возвращаемое значение

значение, указывающее, не равен ли этот экземпляр указанному объекту

## Примеры

Показывает, как проверить равенство длительностей.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// равенство длительности проверяется относительно базового TimeSpan
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


