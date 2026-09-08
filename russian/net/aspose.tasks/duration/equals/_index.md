---
title: "Duration.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту"
type: docs
weight: 80
url: /ru/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public bool Equals(Duration other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | Продолжительность | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает **True**, если другой экземпляр Duration имеет такие же значения TimeSpan и TimeUnit, как у этого экземпляра; в противном случае **false**.

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

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


