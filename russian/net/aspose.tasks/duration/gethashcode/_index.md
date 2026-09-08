---
title: "Duration.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Возвращает значение хеш‑кода для этого объекта."
type: docs
weight: 90
url: /ru/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Возвращает значение хэш‑кода для этого объекта.

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого экземпляра Duration.

## Примеры

Показывает, как получить хеш‑код длительности.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// Хеш‑код календаря основан на типе единицы времени и начальном значении длительности.
// поэтому последующие хеш‑коды равны.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// но хеш‑коды длительностей 1 и 3 не равны.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


