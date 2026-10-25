---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Получает или задает длительность задержки в зависимости от LagFormat"
type: docs
weight: 50
url: /ru/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Получает или задает длительность задержки в зависимости от LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | При попытке установить значение для TaskLinks, где LagFormat имеет значение TimeUnitType.Percent. |

## Примечания

Задержка ссылки может быть процентным значением (LagFormat — это TimeUnitType.Percent). В этом случае длительность рассчитывается как процент от длительности PredTask. В противном случае метод возвращает значение TimeSpan, представляющее задержку TaskLink.

### См. также

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


