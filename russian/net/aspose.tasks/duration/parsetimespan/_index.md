---
title: "Duration.ParseTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Разбирает строку длительности в формате PTHMS."
type: docs
weight: 130
url: /ru/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Разбирает строку длительности в формате "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| value | Строка | указанную строку для разбора. |

### Возвращаемое значение

возвращает разобранный экземпляр структуры [`TimeSpan`](../timespan/).

## Примеры

Показывает, как преобразовать строку во временной интервал.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


