---
title: "Prj.WorkFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Формат, используемый для отображения продолжительности задачи"
type: docs
weight: 790
url: /ru/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Формат, используемый для отображения длительности задачи.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Примеры

Показывает, как получить продолжительность с форматом работы по умолчанию.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// создать значение работы с форматом работы проекта по умолчанию
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


