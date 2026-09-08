---
title: "Project.GetDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает объект Duration с указанным количеством единиц и форматом длительности по умолчанию, определённым в настройках проекта DurationFormat."
type: docs
weight: 1100
url: /ru/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Возвращает объект [`Duration`](../../duration/) с указанным количеством единиц и форматом длительности по умолчанию, определённым в настройках проекта [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | Double | указанное количество единиц. |

### Возвращаемое значение

Объект Duration.

## Примечания

Этот метод следует использовать осторожно, поскольку он возвращает разные длительности в зависимости от настройки Project.DurationFormat. Например, GetWork(1.0) вернёт 1 час, когда Project.DurationFormat установлен в TimeUnitType.Hour, или 1 день, если Project.DurationFormat установлен в TimeUnitType.Day.

## Примеры

Показывает, как создать экземпляр &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; с форматом длительности проекта по умолчанию, используя методы фабрики проекта.

```csharp
var project = new Project();

// получить длительность с форматом проекта по умолчанию.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### См. также

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Возвращает объект [`Duration`](../../duration/) с указанным количеством единиц [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | Double | указанное количество единиц. |
| timeUnit | TimeUnitType | указанное значение TimeUnitType. |

### Возвращаемое значение

Объект Duration.

## Примеры

Показывает, как создать экземпляр &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; с помощью методов фабрики проекта.

```csharp
var project = new Project();

// получить длительность с форматом проекта по умолчанию.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### См. также

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Возвращает объект [`Duration`](../../duration/) с указанным значением TimeSpan и указанным значением [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| timeSpan | TimeSpan | указанное значение TimeSpan. |
| timeUnit | TimeUnitType | указанное значение TimeUnitType. |

### Возвращаемое значение

Объект Duration.

### См. также

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


