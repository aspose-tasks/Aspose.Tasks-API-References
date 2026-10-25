---
title: "Duration.IsEstimated"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Duration. Возвращает значение, указывающее, является ли единица времени оценочной. Флаг, определяющий, является ли данный экземпляр Duration оценочным."
type: docs
weight: 30
url: /ru/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Возвращает значение, указывающее, является ли единица времени оценочной. Флаг, определяющий, является ли данный экземпляр Duration оценочным.

```csharp
public bool IsEstimated { get; }
```

## Примеры

Показывает, как разобрать строку из специально отформатированной строки.

```csharp
var project = new Project();

// примеры длительностей:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// где 1 — количество элементов (день, неделя и т.д.), d — день (h — час, w — неделя) ? — флаг оценки, e — флаг истечения

// попробовать разобрать оценочную длительность
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// попробовать разобрать оценочную длительность
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


