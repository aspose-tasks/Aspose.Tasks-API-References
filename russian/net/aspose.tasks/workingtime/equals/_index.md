---
title: "WorkingTime.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод WorkingTime. Проверяет, что объекты равны."
type: docs
weight: 40
url: /ru/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Проверяет, что объекты равны.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Второй объект для сравнения. |

### Возвращаемое значение

True, если объекты равны, false в противном случае.

## Примеры

Показывает, как проверить равенство рабочего времени.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Равенство календарей проверяется по датам начала и окончания рабочего времени.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### См. также

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


