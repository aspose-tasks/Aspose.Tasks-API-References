---
title: TaskLink.LinkLagTimeSpan
second_title: Справочник по Aspose.Tasks для .NET API
description: TaskLink свойство. Получает или задает продолжительность задержки в зависимости от LagFormat.
type: docs
weight: 50
url: /ru/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Получает или задает продолжительность задержки в зависимости от LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | При попытке установить значение для TaskLinks, где LagFormat — TimeUnitType.Percent. |

### Примечания

Задержка связи может быть значением в процентах (LagFormat — TimeUnitType.Percent). В этом случае продолжительность рассчитывается в процентах от продолжительности PredTask. В противном случае метод возвращает значение TimeSpan, представляющее задержку TaskLink.

### Смотрите также

* class [TaskLink](../)
* пространство имен [Aspose.Tasks](../../tasklink/)
* сборка [Aspose.Tasks](../../../)


