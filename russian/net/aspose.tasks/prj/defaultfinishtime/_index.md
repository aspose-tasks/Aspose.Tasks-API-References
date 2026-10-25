---
title: "Prj.DefaultFinishTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Время завершения по умолчанию для новых задач"
type: docs
weight: 230
url: /ru/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

Время завершения по умолчанию для новых задач.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Примеры

Показывает, как читать/записывать свойство Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


