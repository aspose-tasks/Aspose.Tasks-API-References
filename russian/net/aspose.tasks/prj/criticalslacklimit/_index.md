---
title: "Prj.CriticalSlackLimit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Задачи считаются критическими в MS Project, если общий запас времени меньше или равен этому количеству дней"
type: docs
weight: 140
url: /ru/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Задачи считаются критическими в MS Project, если общий резерв меньше или равен этому количеству дней.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Примеры

Показывает, как читать/записывать свойство Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


