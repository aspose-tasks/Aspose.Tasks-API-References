---
title: "Project.GetWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает объект Duration с указанным значением Double и форматом работы по умолчанию"
type: docs
weight: 1130
url: /ru/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Возвращает объект [`Duration`](../../duration/) с указанным значением Double и форматом работы по умолчанию.

```csharp
public Duration GetWork(double val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | Double | указанное значение double. |

### Возвращаемое значение

Объект Duration.

## Примечания

Этот метод следует использовать с осторожностью, поскольку он возвращает разные длительности в зависимости от настройки Project.WorkFormat. Например, GetWork(1.0) вернёт 1 час, когда Project.WorkFormat установлен в TimeUnitType.Hour, или 1 день, если Project.WorkFormat установлен в TimeUnitType.Day.

## Примеры

Показывает, как получить работу с форматом работы по умолчанию.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// создать значение работы с форматом работы проекта по умолчанию
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### См. также

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


